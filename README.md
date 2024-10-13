# Proyecto de Registro y Login de Usuarios

Este proyecto es una aplicación web básica para el registro y login de usuarios, utilizando Express.js y MariaDB como base de datos. El proyecto sigue el modelo MVC (Modelo-Vista-Controlador) y usa las plantillas Pug para las vistas.

## Requisitos

Antes de ejecutar el proyecto, asegúrate de tener instalados los siguientes requisitos:

- Node.js (versión recomendada: 14 o superior)
- MariaDB (version 20.17)
- Nodemon
- Dialogflow CX

## Configuración del entorno

_Clona el repositorio en tu máquina local:_
Accede a la carpeta del proyecto:

cd LAYLA
Instala las dependencias necesarias para nodejs usando npm:

npm install

Configuración de la Base de Datos

Configura las credenciales de acceso a la base de datos en el archivo config para que el proyecto pueda conectarse a la base de datos:

Asegúrate de que los detalles de tu base de datos (usuario, contraseña, host) estén configurados en el archivo config.js.
Ejecuta las migraciones o scripts SQL necesarios para crear las tablas de usuario.

Ejecución del Proyecto
Para iniciar el servidor, usa Nodemon (si no está instalado, puedes instalarlo globalmente con npm install -g nodemon):

nodemon index.js
El servidor se ejecutará en el puerto local 2800. Puedes acceder a la aplicación en tu navegador usando:

npm run server

http://localhost:2800
Estructura del Proyecto
index.js: El archivo principal que arranca la aplicación.
controllers/: Contiene los controladores que manejan la lógica de negocio.
routes/: Define las rutas de la aplicación.
views/: Contiene las vistas Pug utilizadas para renderizar las páginas web.
public/: Archivos estáticos como CSS, imágenes, etc.
config/: Configuración de la conexión a la base de datos.
Funcionalidades
Registro de nuevos usuarios con validación de datos.
Inicio de sesión para usuarios existentes.
Almacenamiento de información de usuarios en una base de datos MariaDB.
Contribuciones

## Integración de Dialogflow en la Aplicación

Este proyecto incluye la integración de un agente de Dialogflow para interactuar con los usuarios mediante un chat embebido en la página web. A continuación se describe cómo se ha configurado el agente y cómo personalizar su apariencia.

_Agente prosper_:

Es un agente especializado en el procesamiento de lenguaje natural que puede ser utilizado en diferentes casos y que ofrece la posibilidad de adaptarse, en este caso se le proporcionan un data source que contiene informacion de educacion financiera y de productos de banorte.
Necesitas implementar la api no autentificada proporcionada en codigo html por dialogflow CX

### Configuración de Dialogflow

Para integrar el agente de Dialogflow en la página web, se han utilizado los siguientes elementos:

Cómo ejecutar para implementar primer agente
Para el primer agente del intermedio.html llamado prosper 0.3 se utilizó la cuenta que nos administro el staff de google

Cómo ejecutar para implementar segundo agente

Para el segundo agente llamado Super proper test se utilizó la cuenta personal
