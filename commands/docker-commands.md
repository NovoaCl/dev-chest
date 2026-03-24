# Docker:

| Description                                                                             |          Command          |
| --------------------------------------------------------------------------------------- | :-----------------------: |
| Inicializa un repositorio local nuevo.                                                  |        `git init`         |
| Crea una copia local de un repositorio remoto.                                          |     `git clone <url>`     |
| Muestra el status de los archivos en el directorio de trabajo y el area de preparación. |       `git status`        |
| Agrega un archivo especifico al area de preparación.                                    |     `git add <file>`      |
| Agrega todas las modificaciones del directorio.                                         |        `git add .`        |
| Registra los cambios como un commit nuevo con un mensaje descriptivo.                   | `git commit -m "message"` |
| Muestra las diferencias entre el directorio de trabajo y el área de preparación.        |        `git diff`         |


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

