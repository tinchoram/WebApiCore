# WebApi .NET Core

Este proyecto es una API RESTful desarrollada en .NET Core que permite la gesti�n de productos en una base de datos SQL Server. Implementa operaciones CRUD (Crear, Leer, Actualizar, Eliminar) para los productos y est� dise�ada para ser multiplataforma y escalable.

## Tecnolog�as utilizadas

- .NET Core
- Entity Framework Core
- SQL Server
- Swagger para la documentaci�n de la API (usando Swashbuckle)

## Estructura del proyecto

- **Controllers**: Contiene el `ProductsController`, que maneja los endpoints para las operaciones CRUD.
- **Models**: Incluye el modelo `Product`.
- **Data**: Define `AppDbContext`, el contexto de Entity Framework Core.

## Instalaci�n

1. Clona el repositorio y abre el proyecto en Visual Studio o Visual Studio Code.
2. Aseg�rate de tener SQL Server en ejecuci�n y crea una base de datos llamada `webapicore`.
3. Configura la cadena de conexi�n en `appsettings.json`:
   ```json
   {
     "ConnectionStrings": {
       "DefaultConnection": "Server=localhost;Database=webapicore;User Id=tu_usuario;Password=tu_contrase�a;TrustServerCertificate=True;"
     }
   }