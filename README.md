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
Pero para desplde
