# Desing Document: API REST CONTACTOS
API REST para gestionar contactos en una DB utilizando FastAPI

## 1. Descripcion
Ejemplo de una API REST para gestionar contactos en una DB utiliando FastAPI.

## 2.Objetivo
Realizar un ejemplo de diseño de una API REST de un tipo CRUD y su porterior codificacion utilizando el framework [FASTAPI](http://fastapi.tlangolo.com/)

## 3.Diseño de la DB
Para este ejemplo se utilizara el gestor de bases de datos [SQLite3](http://sqlite.org). con las siguientes tablas:

### 3.1 Tablas: Contactos
Diseño de la tabla para almacenar contactos

|N°|CAMPO|TIPO|RESTRICCIONES|DESCRIPCION|
|--|--|--|--|--|
|1|id_contactos|int|PRIMARY KEY|Llave primaria de la tabla|
|2|	nombre|	varchar(100)|	Not Null|	Nombre del contacto|
|3	|primer_apellido	|varchar(50)	|Not Null	|Primer Apellido del contacto|
|4|	segundo_apellido|	varchar(50)|	Not Null	|Segundo Apellido del contacto|
|5	|email	|varchar(100)	|Not Null	|Email del contacto|
|6	|telefono|	varchar(13)|	Not Null|	Telefono del contacto|

### 3.2
CREATE TABLE IF NOT EXISTS contactos ( id_contacto INTEGER PRIMARY KEY, nombre VARCHAR(100) NOT NULL, primer_apellido VARCHAR(50) NOT NULL, segundo_apellido VARCHAR(50) NOT NULL, email VARCHAR(100) NOT NULL, telefono VARCHAR(13) NOT NULL );

## 4. Diseño del Endpoint
Diseño del endpoint para el recurso contactos
### 4.1 Mostrar todos los contactos
Endpoint para obtener todos los contactos


|N°|Propiedad|Descripcion|
|--|--|--|
|1|Description|Endpoint para obtener todos los contactos|
|2|Summary|Endpoint todos los contactos|
|3|Method| GET|

