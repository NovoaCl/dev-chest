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




# Docker Command Reference / Referencia de Comandos de Docker

### 1. Installation & Configuration

**Description:** Commands to install, configure, and verify Docker installation.

| Description                    | Commands                       |
| ------------------------------ | ------------------------------ |
| Check Docker version           | `docker --version`             |
| Check Docker Compose version   | `docker compose version`       |
| Start Docker service           | `sudo systemctl start docker`  |
| Enable Docker to start on boot | `sudo systemctl enable docker` |
| Verify Docker installation     | `docker info`                  |

---

### 2. Image Management

**Description:** Commands to manage Docker images including building, pulling, pushing, and listing.

| Description                    | Commands                                |
| ------------------------------ | --------------------------------------- |
| List local Docker images       | `docker images`                         |
| Pull an image from Docker Hub  | `docker pull <image>`                   |
| Build an image from Dockerfile | `docker build -t <image_name>:<tag> .`  |
| Tag an image                   | `docker tag <image> <repository>:<tag>` |
| Push an image to a repository  | `docker push <repository>:<tag>`        |
| Remove an image                | `docker rmi <image>`                    |
| Inspect an image               | `docker inspect <image>`                |

---

### 3. Container Management

**Description:** Commands to create, run, stop, and manage Docker containers.

| Description                          | Commands                                        |
| ------------------------------------ | ----------------------------------------------- |
| List running containers              | `docker ps`                                     |
| List all containers                  | `docker ps -a`                                  |
| Run a new container                  | `docker run -d --name <container_name> <image>` |
| Run a container interactively        | `docker run -it <image> /bin/bash`              |
| Stop a container                     | `docker stop <container>`                       |
| Start a container                    | `docker start <container>`                      |
| Restart a container                  | `docker restart <container>`                    |
| Remove a container                   | `docker rm <container>`                         |
| Execute a command inside a container | `docker exec -it <container> <command>`         |
| View container logs                  | `docker logs <container>`                       |

---

### 4. Networks

**Description:** Commands to create, inspect, and manage Docker networks.

| Description                           | Commands                                          |
| ------------------------------------- | ------------------------------------------------- |
| List Docker networks                  | `docker network ls`                               |
| Inspect a network                     | `docker network inspect <network>`                |
| Create a custom network               | `docker network create <network_name>`            |
| Connect a container to a network      | `docker network connect <network> <container>`    |
| Disconnect a container from a network | `docker network disconnect <network> <container>` |
| Remove a network                      | `docker network rm <network>`                     |

---

### 5. Volumes

**Description:** Commands to manage Docker volumes for persistent data storage.

| Description                   | Commands                                            |
| ----------------------------- | --------------------------------------------------- |
| List Docker volumes           | `docker volume ls`                                  |
| Inspect a volume              | `docker volume inspect <volume>`                    |
| Create a new volume           | `docker volume create <volume_name>`                |
| Remove a volume               | `docker volume rm <volume>`                         |
| Run a container with a volume | `docker run -v <volume>:/path/in/container <image>` |

---

### 6. Docker Compose

**Description:** Commands to manage multi-container applications with Docker Compose.

| Description                                  | Commands                 |
| -------------------------------------------- | ------------------------ |
| Start services defined in docker-compose.yml | `docker compose up`      |
| Start in detached mode                       | `docker compose up -d`   |
| Stop services                                | `docker compose down`    |
| View service logs                            | `docker compose logs`    |
| Build services                               | `docker compose build`   |
| Restart services                             | `docker compose restart` |
| Remove containers, networks, and volumes     | `docker compose down -v` |

---

### 7. Inspection & Monitoring

**Description:** Commands to inspect container states, resource usage, and statistics.

| Description                   | Commands                     |
| ----------------------------- | ---------------------------- |
| Inspect container details     | `docker inspect <container>` |
| Display container statistics  | `docker stats`               |
| View container resource usage | `docker top <container>`     |
| Monitor real-time logs        | `docker logs -f <container>` |

---

### 8. Cleanup & Maintenance

**Description:** Commands to clean unused resources and maintain the Docker environment.

| Description                         | Commands                           |
| ----------------------------------- | ---------------------------------- |
| Remove all stopped containers       | `docker container prune`           |
| Remove unused images                | `docker image prune`               |
| Remove unused volumes               | `docker volume prune`              |
| Remove unused networks              | `docker network prune`             |
| Remove all unused resources         | `docker system prune`              |
| Remove everything including volumes | `docker system prune -a --volumes` |

---

### 9. Advanced Utilities

**Description:** Additional commands and options for advanced Docker management.

| Description                    | Commands                                    |
| ------------------------------ | ------------------------------------------- |
| Export a container filesystem  | `docker export <container> > container.tar` |
| Import a container as an image | `docker import container.tar <image_name>`  |
| Save an image to a tar file    | `docker save -o <file.tar> <image>`         |
| Load an image from a tar file  | `docker load -i <file.tar>`                 |
| Attach to a running container  | `docker attach <container>`                 |
| Pause a container              | `docker pause <container>`                  |
| Unpause a container            | `docker unpause <container>`                |

---

## Versión en Español

### 1. Instalación y Configuración

**Descripción:** Comandos para instalar, configurar y verificar Docker.

| Descripción                            | Comandos                       |
| -------------------------------------- | ------------------------------ |
| Ver versión de Docker                  | `docker --version`             |
| Ver versión de Docker Compose          | `docker compose version`       |
| Iniciar servicio Docker                | `sudo systemctl start docker`  |
| Habilitar Docker al iniciar el sistema | `sudo systemctl enable docker` |
| Verificar instalación de Docker        | `docker info`                  |

---

### 2. Gestión de Imágenes

**Descripción:** Comandos para manejar imágenes Docker: construir, descargar, subir y listar.

| Descripción                       | Comandos                                  |
| --------------------------------- | ----------------------------------------- |
| Listar imágenes locales           | `docker images`                           |
| Descargar imagen desde Docker Hub | `docker pull <imagen>`                    |
| Construir imagen desde Dockerfile | `docker build -t <nombre_imagen>:<tag> .` |
| Etiquetar imagen                  | `docker tag <imagen> <repositorio>:<tag>` |
| Subir imagen a un repositorio     | `docker push <repositorio>:<tag>`         |
| Eliminar una imagen               | `docker rmi <imagen>`                     |
| Inspeccionar imagen               | `docker inspect <imagen>`                 |

---

### 3. Gestión de Contenedores

**Descripción:** Comandos para crear, ejecutar, detener y administrar contenedores Docker.

| Descripción                              | Comandos                                            |
| ---------------------------------------- | --------------------------------------------------- |
| Listar contenedores en ejecución         | `docker ps`                                         |
| Listar todos los contenedores            | `docker ps -a`                                      |
| Ejecutar un nuevo contenedor             | `docker run -d --name <nombre_contenedor> <imagen>` |
| Ejecutar contenedor de forma interactiva | `docker run -it <imagen> /bin/bash`                 |
| Detener un contenedor                    | `docker stop <contenedor>`                          |
| Iniciar un contenedor                    | `docker start <contenedor>`                         |
| Reiniciar un contenedor                  | `docker restart <contenedor>`                       |
| Eliminar un contenedor                   | `docker rm <contenedor>`                            |
| Ejecutar comando dentro de un contenedor | `docker exec -it <contenedor> <comando>`            |
| Ver logs de un contenedor                | `docker logs <contenedor>`                          |

---

### 4. Redes

**Descripción:** Comandos para crear, inspeccionar y gestionar redes Docker.

| Descripción                          | Comandos                                       |
| ------------------------------------ | ---------------------------------------------- |
| Listar redes Docker                  | `docker network ls`                            |
| Inspeccionar una red                 | `docker network inspect <red>`                 |
| Crear red personalizada              | `docker network create <nombre_red>`           |
| Conectar un contenedor a una red     | `docker network connect <red> <contenedor>`    |
| Desconectar un contenedor de una red | `docker network disconnect <red> <contenedor>` |
| Eliminar una red                     | `docker network rm <red>`                      |

---

### 5. Volúmenes

**Descripción:** Comandos para manejar volúmenes Docker y persistencia de datos.

| Descripción                     | Comandos                                               |
| ------------------------------- | ------------------------------------------------------ |
| Listar volúmenes                | `docker volume ls`                                     |
| Inspeccionar un volumen         | `docker volume inspect <volumen>`                      |
| Crear un volumen                | `docker volume create <nombre_volumen>`                |
| Eliminar un volumen             | `docker volume rm <volumen>`                           |
| Ejecutar contenedor con volumen | `docker run -v <volumen>:/ruta/en/contenedor <imagen>` |

---

### 6. Docker Compose

**Descripción:** Comandos para manejar aplicaciones multi-contenedor.

| Descripción                              | Comandos                 |
| ---------------------------------------- | ------------------------ |
| Iniciar servicios de docker-compose.yml  | `docker compose up`      |
| Iniciar en modo detached                 | `docker compose up -d`   |
| Detener servicios                        | `docker compose down`    |
| Ver logs de servicios                    | `docker compose logs`    |
| Construir servicios                      | `docker compose build`   |
| Reiniciar servicios                      | `docker compose restart` |
| Eliminar contenedores, redes y volúmenes | `docker compose down -v` |

---

### 7. Inspección y Monitoreo

**Descripción:** Comandos para inspeccionar contenedores y monitorear recursos.

| Descripción                            | Comandos                      |
| -------------------------------------- | ----------------------------- |
| Inspeccionar detalles de un contenedor | `docker inspect <contenedor>` |
| Mostrar estadísticas de contenedores   | `docker stats`                |
| Ver uso de recursos de un contenedor   | `docker top <contenedor>`     |
| Monitorear logs en tiempo real         | `docker logs -f <contenedor>` |

---

### 8. Limpieza y Mantenimiento

**Descripción:** Comandos para limpiar recursos no usados y mantener Docker.

| Descripción                           | Comandos                           |
| ------------------------------------- | ---------------------------------- |
| Eliminar contenedores detenidos       | `docker container prune`           |
| Eliminar imágenes no usadas           | `docker image prune`               |
| Eliminar volúmenes no usados          | `docker volume prune`              |
| Eliminar redes no usadas              | `docker network prune`             |
| Eliminar todos los recursos no usados | `docker system prune`              |
| Eliminar todo incluyendo volúmenes    | `docker system prune -a --volumes` |

---

### 9. Utilidades Avanzadas

**Descripción:** Comandos adicionales para manejo avanzado de Docker.

| Descripción                             | Comandos                                       |
| --------------------------------------- | ---------------------------------------------- |
| Exportar filesystem de un contenedor    | `docker export <contenedor> > contenedor.tar`  |
| Importar contenedor como imagen         | `docker import contenedor.tar <nombre_imagen>` |
| Guardar imagen en archivo tar           | `docker save -o <archivo.tar> <imagen>`        |
| Cargar imagen desde archivo tar         | `docker load -i <archivo.tar>`                 |
| Adjuntarse a un contenedor en ejecución | `docker attach <contenedor>`                   |
| Pausar un contenedor                    | `docker pause <contenedor>`                    |
| Reanudar un contenedor                  | `docker unpause <contenedor>`                  |

---