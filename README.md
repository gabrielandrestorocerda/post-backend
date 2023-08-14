# README

# DESCRIPCIÓN

post-backend es una API desarrollada para post-frontend y que permite gestionar los post que se trabajan desde la app del frontend a partir de la prueba solicitada por el equipo de TCIT, ésta no tiene ningún fin lucrativo y tiene por objetivo demostrar las capacidades y conocimiento sobre Ruby on Rails para el candidato Gabriel Toro.

# DEPENDENCIAS

Antes de ejecutar la aplicación, asegúrese de haber instalado las siguientes dependencias, de lo contrario, no se asegurará el funcionamiento correcto de la aplicación:

    - Ruby >= 3.1.3 (instalar con [rbenv](https://github.com/rbenv/rbenv) o [rvm](https://help.dreamhost.com/hc/es/articles/217185247-Administrador-de-versiones-de-Ruby-Ruby-Version-Manager-RVM-))
    - Rails >= 7.0.7
    - PostgreSQL >= 9

# CONFIGURACIÓN

    - Instalar ruby 3.1.3 utilizando rbenv y/o rvm 
	- Ejecutar bundle install
	- Crear un archivo .env debajo de la carpeta vendor y en ese archivo pegar lo siguiente:
		DATABASE_HOST=localhost
		DATABASE_PORT=5432
		DATABASE_USERNAME=<tu usuario creado en postgres>
		DATABASE_PASSWORD=<contraseña asociada a dicho usuario>
    - Configurar las variables de entorno para ingresar el usuario y contraseña ingresado en postgres
	- Ejecutar rails db:create
	- Ejecutar rails db:migrate
	- Ejecutar rails db:seed (este paso es solo si se quiere probar la app con datos)
    - Ejecutar rails s --port 3001 (esto levantará el servidor en el puerto 3001)
    
# OBSERVACIONES A TENER EN CUENTA

Debido al tiempo dado para desarrollar la aplicación, se enfocó en generar solo las funcionalidades básicas necesarias para rendir la prueba, sin embargo,
en un caso normal, se agregarían más cosas como validaciones por ejemplo tanto en el lado del frontend y backend, scopes para consultas de base de datos en
el backend, etc.