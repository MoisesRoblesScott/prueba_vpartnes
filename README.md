Dentro del archivo comprimido se encuentran dos carpetas y un archivo SQL que es la base de datos.

1) Carpeta Front:
Para la ejecución del proyecto es necesario, primero abrir una ventana terminal y ubicarse en la raíz del proyecto y ejecutar el comando composer update. 
La prueba frontend se realizó utilizando el framework laravel, jquery y bootstrap. Pude a ver utilizado el framework JavaScript vue js ya que ese es mi fuerte y el que más utilizo, pero decidí utilizar jquery por la simplicidad de la prueba y poder realizarla en el menor tiempo posible.

2) Carpeta BackEnd:
Aquí encontrara las Apis Rest que se solicitaron en la prueba, se utilizo MVC, lenguaje de programacion PHP con framework laravel.

Para la ejecución del proyecto es necesario, primero abrir una ventana terminal y ubicarse en la raíz del proyecto y ejecutar el comando *composer update* 

En a raíz del proyecto se encuentra un archivo llamado .env, en dicho archivo se encuentra la configuración para conectarse a la base de datos.

En la línea DB_DATABASE se debe colocar el nombre de la base de datos.
En DB_USERNAME es el usuario de la base de datos, por defecto siempre es root, si tiene un usuario diferente entonces remplazar root por el nombre del usuario,
En DB_PASSWORD es la contraseña de la base de datos, si su base de datos no tiene contraseña dejarlo vacío. 

Luego deberá ejecutar el servidor interno de laravel con el comando *php artisan serve* 
te generara una ruta parecida a esta: http://127.0.0.1:8000

A continuación, dejare las urls específicas de las Apis creadas:

•	http://127.0.0.1:8000/api/peticiones/listar  
  Regresa el listado de tikect

•	http://127.0.0.1:8000/api/peticiones/crear
parámetros para la creación: nombre_usuario y estado
 
•	 http://127.0.0.1:8000/api/peticiones/actualizar
   parámetros para el update: id, nombre_usuario y estado
   
•	http://127.0.0.1:8000api/peticiones/eliminar/<<id_tikect>>
  se debe enviar el id del tikect

•	http://127.0.0.1:8000/api/peticiones/filtro/<<parametro_de_busqueda>>
  se debe enviar el nombre del usuario
  
 Las pruebas de las apis se realizaron con el programa postman.
 
para revisar la logica desarrollada, se encuentra en el controlador en la siguiente ruta del proyecto. \app\Http\Controllers\ApisController.php
el archivo de rutas se encuentra en \routes\api.php
