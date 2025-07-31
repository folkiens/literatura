# Proyecto Literatura

Bienvenido al proyecto literatura, una aplicación Java basada en Spring Boot que te permite gestionar libros y autores de manera eficiente y fácil.

## Descripción del Proyecto

El proyecto literatura está diseñado para ayudar a los amantes de la literatura a buscar, registrar y listar libros y autores. También ofrece funcionalidades avanzadas como listar autores vivos en un determinado año y listar libros por idioma.

### Funcionamiento del Programa

1. **Obtención de Datos**: El programa toma libros de la API [GutenDex](https://gutendex.com/).
2. **Conversión a Objetos Java**: Los datos obtenidos de la API se convierten en objetos Java utilizando la clase `JsonParser`.
3. **Procesamiento**: Los datos se procesan para asegurarse de que los libros y autores no se dupliquen en la base de datos.
4. **Almacenamiento**: Los libros y autores procesados se guardan en una base de datos SQL compatible (PostgreSQL, MySQL, MariaDB, SQL Server).

### Desafío de Alura

Este proyecto es una solución al desafío del challenge de Alura, donde se nos retó a crear una aplicación para gestionar una base de datos de libros y autores utilizando tecnologías modernas.

## Características 

- **Buscar libro por título**: Encuentra libros por su título.
- **Listar libros registrados**: Muestra todos los libros registrados en la base de datos.
- **Listar autores registrados**: Muestra todos los autores registrados en la base de datos.
- **Listar autores vivos en un determinado año**: Encuentra autores que estaban vivos en un año específico.
- **Listar libros por idioma**: Filtra libros por su idioma.

## Tecnologías Utilizadas

- **Java 11+**
- **Spring Boot 2.6.4**
- **Spring Data JPA**
- **PostgreSQL**, **MySQL**, **MariaDB**, **SQL Server**, **H2**
- **Jackson**
- **Maven**

## Instalación y Ejecución

Sigue estos pasos para configurar y ejecutar el proyecto en tu máquina local.

### Prerrequisitos

- Java 11 o superior
- Maven 3.6 o superior
- Una base de datos SQL (PostgreSQL, MySQL, MariaDB, SQL Server, H2)


### Configurar tu base de datos en el archivo application.properties
```
spring.datasource.url=jdbc:postgresql://localhost:5432/nombre_de_tu_base_de_datos
spring.datasource.username=tu_usuario
spring.datasource.password=tu_contraseña
spring.jpa.hibernate.ddl-auto=update
```

### Ejecuta LiteraturaApplication en tu IDE
Al ejecutar la aplicación, se mostrará un menú en la consola con las siguientes opciones:
```
Bienvenidos a literatura
Elija una opción:
1 - Buscar libro por título
2 - Listar libros registrados
3 - Listar autores registrados
4 - Listar autores vivos en un determinado año
5 - Listar libros por idioma
0 - Salir
```
Selecciona la opción deseada ingresando el número correspondiente y sigue las instrucciones en pantalla.





