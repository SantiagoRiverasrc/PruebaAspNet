# PruebaAspNet
CRUD creado con el ambiente de desarrollo de ASP.Net Core 6.0, usando el patrón de arquitectura MVC(Modelo-Vista-Controlador) + Razor + SQLServer + EntityFramework.

Para poder ejecutar el proyecto se debe de descomprimir el archivo Prueba.zip, le saldra una carpeta llamada Prueba la cual ustede debe ejecutar en el Visual Studio.
Pero antes de realizar esta manipulación es obligatorio tener la base de datos creada debido a que se esta utilizando una ORM. Esta debe ser en MicrosoftSQLServer.

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


Ya al tener lista la base de datos, se puede correr el proyecto. Ahora para que este se pueda conectar a la base de datos y poder realizar ciertas interacciones se debe de ir al archivo appsettings.json y cambiar en la parte que dice 'Server' la url del servidor predeterminado por el que tienes tu en el LOCAL.

[![Explicaci-n1.png](https://i.postimg.cc/BnkJsDQk/Explicaci-n1.png)](https://postimg.cc/bZx79Zn9)

