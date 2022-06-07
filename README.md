# Parte-practica-docker-examen

## Introducción 
Primero de todo, tener en cuenta que tenemos el docker instalado con el jdk etc, empezariamos descargándose el docker file, el archivo.war que contiene todo lo relacionado nuestra aplicación y el archivo.sql

![imagen](https://user-images.githubusercontent.com/91564971/172449627-5196b266-2925-4449-9797-e83d61874644.png)

## Configuración del archivo docker-compose.yml.
Una vez descargado todos los archivos necesarios procederemos a configurar el docker file, en mi caso solo tuve que modificar la versión de mi sql ya que previamente venia por defecto en la versión 5.0, por lo que para evitar errores, lo puse en la versión correcta, que es la versión 8.0.29.

![imagen](https://user-images.githubusercontent.com/91564971/172450297-80a84c8e-7aa4-4417-bdaa-7d01ddd44c37.png)

## Pasos para el despliegue de la aplicación.
Para desplegar la aplicación lo primero que haremos es ver que docker esta funcionando correctamente, para ello usaremos el comando 'sudo systemctl status docker' y veremos que sale 'active'.

![imagen](https://user-images.githubusercontent.com/91564971/172451188-be299425-c6ae-4851-8647-7e03ae01fefb.png)

Una vez comprobado que el docker funciona correctamente usaremos el comando 'docker ps' para ver la imagenes que tenemos activas.

![imagen](https://user-images.githubusercontent.com/91564971/172451637-f876922a-3e68-42a4-8c7a-ce716294198c.png)

Como podremos observar sale que tenemos 3 imagenes subidas y exactamente son las de nuestro proyecto porque estaba haciendo pruebas de si me funcionaba.
Pero para poder llegar hasta ahí lo que hice fue dirigirme a la carpeta donde están los archivos dockerfile, el sql y el .war

![imagen](https://user-images.githubusercontent.com/91564971/172452515-04b23169-3928-46c5-971f-a798bc9cb699.png)

En mi caso estan en 'Escritorio/Docker', una vez dirigidos en la ruta de los archivos ejecutamos el siguiente comando 'sudo docker compose up -d'

![imagen](https://user-images.githubusercontent.com/91564971/172452798-5a88aa0c-30ec-4b1a-8691-8a1a8a839f2e.png)

Una vez ejecutado este comando comprobará que todo está en orden y que se ha subido correctamente.
Por tanto en la siguiente imagen podemos ver que se han subido como las tres imagenes.

![imagen](https://user-images.githubusercontent.com/91564971/172453012-37e4e886-b7bb-4a5e-9954-947dde6eb75a.png)

## conclusiones

Como conclusiones he tenido problemas para poder entrar al localhost:8080 porque el ubuntu está recién instalado y todavía me falta configurarlo un poco
más y por ello me da el siguiente error para acceder al localhost

![imagen](https://user-images.githubusercontent.com/91564971/172455795-22b13112-56f9-4580-a29d-eaa0ad62490f.png)

Otro error por el cual no he podido subir la imagen a docker hub es debido a este error

![imagen](https://user-images.githubusercontent.com/91564971/172456294-d90bb368-d4e0-48b7-96d4-fb8ad90d93f3.png)

Por alguna razón la cual desconozco no me deja loguearme por ende no puedo subir mis imagenes a docker hub











