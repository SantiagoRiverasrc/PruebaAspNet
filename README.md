# PruebaAspNet
CRUD creado con el ambiente de desarrollo de ASP.Net Core 6.0, usando el patrón de arquitectura MVC(Modelo-Vista-Controlador) + Razor + SQLServer + EntityFramework.

Para poder ejecutar el proyecto se debe de descomprimir el archivo Prueba.zip, le saldra una carpeta llamada Prueba la cual ustede debe ejecutar en el Visual Studio.
Pero antes de realizar esta manipulación se necesita tener la base de datos creada debido a que se esta utilizando una ORM. Esta debe ser en SQLServer.

Ejecutar el comando para la creación de la base de datos:

```
Create database TaskData
```

Pararse en la base de datos TaskData y crear la tabla principal Tarea:

```
Create table Tarea(
  Id int identity(1,1) primary key,
  Descripcion varchar(350),
  FechaCreacion datetime,
  Completado bit default 0
)
````
