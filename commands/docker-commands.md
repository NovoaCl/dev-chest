## Docker basic commands:

| Description                                             |            Command            |
| ------------------------------------------------------- | :---------------------------: |
| Crea y arranca un contenedor nuevo desde una imagen.    |     `docker run <imagen>`     |
| Lista los contenedores en ejecución.                    |          `docker ps`          |
| Lista todos los contenedores (incluidos los detenidos). |        `docker ps -a`         |
| Detiene un contenedor en ejecución.                     |  `docker stop <contenedor>`   |
| Inicia un contenedor detenido.                          |  `docker start <contenedor>`  |
| Reinicia un contenedor.                                 | `docker restart <contenedor>` |
| Elimina un contenedor.                                  |   `docker rm <contenedor>`    |
| Lista las imágenes descargadas.                         |        `docker images`        |
| Elimina una imagen.                                     |     `docker rmi <imagen>`     |
| Descarga una imagen desde Docker Hub.                   |    `docker pull <imagen>`     |

Gestión e Interacción
docker exec -it <contenedor> <comando>: Ejecuta un comando dentro de un contenedor en ejecución (ej. docker exec -it mi_contenedor bash).
docker logs -f <contenedor>: Muestra los registros (logs) en tiempo real.
docker inspect <contenedor/imagen>: Muestra información detallada en formato JSON.
docker cp <ruta1> <contenedor>:<ruta2>: Copia archivos/carpetas entre el host y el contenedor.
DataCamp
DataCamp
+4
Construcción de Imágenes (Build)
docker build -t <nombre> .: Construye una imagen a partir del Dockerfile en el directorio actual.
docker commit <contenedor> <nueva_imagen>: Crea una nueva imagen a partir de los cambios de un contenedor.
Hostinger
Hostinger
+1
Limpieza y Redes
docker system prune: Elimina todos los contenedores detenidos, redes no usadas e imágenes sin nombre (dangling).
docker network ls: Lista las redes de Docker.
Imagina Formación
Imagina Formación
+4
Nota: Muchos comandos requieren sudo en sistemas Linux si no se ha configurado el grupo Docker.

Docker:
. docker run -it -d ubuntu: corre un contenedor con ubuntu
. docker pull postgres: tira la imagen de postgreSQL
. docker ps: lista los contenedores activos.
. docker exec -it <CONTAINER ID>: para ingresar y ver sus archivos
.docker run --name postgres_db \
 -e POSTGRES_DB=my_database \
 -e POSTGRES_USER=postgres \
 -e POSTGRES_PASSWORD=mysecretpassword \
 -p 5432:5432 \
 -d postgres:15
Crea un contenedor y su base de datos.
