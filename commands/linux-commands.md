# Linux Command Reference / Referencia de Comandos de Linux

### 1. File System Navigation

**Description:** Commands to navigate and explore the Linux file system.

| Description                     | Commands         |
| ------------------------------- | ---------------- |
| Print current working directory | `pwd`            |
| List files and directories      | `ls`             |
| List all files including hidden | `ls -a`          |
| List files with detailed info   | `ls -l`          |
| Change directory                | `cd <directory>` |
| Move up one directory           | `cd ..`          |
| Move to home directory          | `cd ~`           |

---

### 2. File & Directory Management

**Description:** Commands to create, copy, move, and remove files and directories.

| Description                     | Commands                       |
| ------------------------------- | ------------------------------ |
| Create a new directory          | `mkdir <directory>`            |
| Create parent directories       | `mkdir -p <path>`              |
| Remove a directory              | `rmdir <directory>`            |
| Remove directory recursively    | `rm -r <directory>`            |
| Copy a file                     | `cp <source> <destination>`    |
| Copy directory recursively      | `cp -r <source> <destination>` |
| Move or rename a file/directory | `mv <source> <destination>`    |
| Remove a file                   | `rm <file>`                    |
| Display file content            | `cat <file>`                   |
| View content page by page       | `less <file>`                  |
| View content with scroll        | `more <file>`                  |

---

### 3. Permissions & Users

**Description:** Commands to manage file permissions, ownership, and user accounts.

| Description              | Commands                  |
| ------------------------ | ------------------------- |
| Change file permissions  | `chmod 755 <file>`        |
| Change file owner        | `chown user:group <file>` |
| Display file permissions | `ls -l`                   |
| Switch user              | `su - <username>`         |
| Check current user       | `whoami`                  |
| List users logged in     | `w` or `who`              |

---

### 4. Processes & Performance

**Description:** Commands to monitor and manage running processes.

| Description               | Commands        |
| ------------------------- | --------------- |
| Show running processes    | `ps aux`        |
| Real-time process monitor | `top`           |
| Advanced monitor          | `htop`          |
| Kill a process by PID     | `kill <PID>`    |
| Kill process forcefully   | `kill -9 <PID>` |
| Show system uptime        | `uptime`        |
| View process tree         | `pstree`        |

---

### 5. Networking

**Description:** Commands to check network configuration and connectivity.

| Description                       | Commands        |
| --------------------------------- | --------------- |
| Display IP addresses              | `ip addr`       |
| Show routing table                | `ip route`      |
| Ping a host                       | `ping <host>`   |
| Check open ports                  | `netstat -tuln` |
| Check connectivity to remote host | `curl -I <url>` |
| Download a file from URL          | `wget <url>`    |
| Test network speed                | `speedtest-cli` |
| Display active connections        | `ss -tuln`      |

---

### 6. Compression & Archives

**Description:** Commands to compress and extract files.

| Description          | Commands                           |
| -------------------- | ---------------------------------- |
| Create a tar archive | `tar -cvf archive.tar <files>`     |
| Extract tar archive  | `tar -xvf archive.tar`             |
| Create gzip archive  | `tar -czvf archive.tar.gz <files>` |
| Extract gzip archive | `tar -xzvf archive.tar.gz`         |
| Create zip archive   | `zip archive.zip <files>`          |
| Extract zip archive  | `unzip archive.zip`                |

---

### 7. Search & Filtering

**Description:** Commands to search text, files, and filter outputs.

| Description             | Commands                           |
| ----------------------- | ---------------------------------- |
| Search for text in file | `grep "pattern" <file>`            |
| Search recursively      | `grep -r "pattern" <directory>`    |
| Search files by name    | `find <directory> -name <pattern>` |
| Count occurrences       | `grep -c "pattern" <file>`         |
| Print specific columns  | `awk '{print $1, $3}' <file>`      |
| Replace text in file    | `sed 's/old/new/g' <file>`         |

---

### 8. Package Management

**Description:** Commands to install, update, and remove software packages.

| Description                 | Commands                     |
| --------------------------- | ---------------------------- |
| Update apt repositories     | `sudo apt update`            |
| Upgrade installed packages  | `sudo apt upgrade`           |
| Install a package           | `sudo apt install <package>` |
| Remove a package            | `sudo apt remove <package>`  |
| Search for a package        | `apt search <package>`       |
| Yum install (RedHat/CentOS) | `sudo yum install <package>` |
| DNF install (Fedora)        | `sudo dnf install <package>` |

---

### 9. System & Information

**Description:** Commands to get system information and hardware details.

| Description                | Commands             |
| -------------------------- | -------------------- |
| Display disk usage         | `df -h`              |
| Display folder size        | `du -sh <directory>` |
| Display memory usage       | `free -h`            |
| Display kernel and OS info | `uname -a`           |
| Show CPU info              | `lscpu`              |
| Show block devices         | `lsblk`              |
| Show running services      | `systemctl status`   |

---

### 10. Advanced Utilities
Descripción:** Comandos para navegar y explorar el sistema de archivos Linux.

| Descripción                                  | Comandos          |
| -------------------------------------------- | ----------------- |
| Mostrar directorio actual                    | `pwd`             |
| Listar archivos y carpetas                   | `ls`              |
| Listar todos los archivos incluyendo ocultos | `ls -a`           |
| Listar archivos con detalles                 | `ls -l`           |
| Cambiar de directorio                        | `cd <directorio>` |
| Subir un nivel de directorio                 | `cd ..`           |
| Ir al directorio home                        | `cd ~`            |

---

### 2. Gestión de Archivos y Directorios

**Descripción:** Comandos para crear, copiar, mover y eliminar archivos y directorios.

| Descripción                          | Comandos                   |
| ------------------------------------ | -------------------------- |
| Crear un directorio                  | `mkdir <directorio>`       |
| Crear directorios padres             | `mkdir -p <ruta>`          |
| Eliminar un directorio vacío         | `rmdir <directorio>`       |
| Eliminar directorio recursivamente   | `rm -r <directorio>`       |
| Copiar archivo                       | `cp <origen> <destino>`    |
| Copiar directorio recursivamente     | `cp -r <origen> <destino>` |
| Mover o renombrar archivo/directorio | `mv <origen> <destino>`    |
| Eliminar archivo                     | `rm <archivo>`             |
| Mostrar contenido de un archivo      | `cat <archivo>`            |
| Ver contenido página por página      | `less <archivo>`           |
| Ver contenido con scroll             | `more <archivo>`           |

---

### 3. Permisos y Usuarios

**Descripción:** Comandos para gestionar permisos de archivos, propietarios y usuarios.

| Descripción                    | Comandos                        |
| ------------------------------ | ------------------------------- |
| Cambiar permisos de archivo    | `chmod 755 <archivo>`           |
| Cambiar propietario de archivo | `chown usuario:grupo <archivo>` |
| Mostrar permisos de archivos   | `ls -l`                         |
| Cambiar de usuario             | `su - <usuario>`                |
| Ver usuario actual             | `whoami`                        |
| Listar usuarios conectados     | `w` o `who`                     |

---

### 4. Procesos y Rendimiento

**Descripción:** Comandos para monitorizar y gestionar procesos en ejecución.

| Descripción                             | Comandos        |
| --------------------------------------- | --------------- |
| Mostrar procesos en ejecución           | `ps aux`        |
| Monitor de procesos en tiempo real      | `top`           |
| Monitor avanzado                        | `htop`          |
| Terminar proceso por PID                | `kill <PID>`    |
| Terminar proceso forzosamente           | `kill -9 <PID>` |
| Mostrar tiempo de actividad del sistema | `uptime`        |
| Ver árbol de procesos                   | `pstree`        |

---

### 5. Redes

**Descripción:** Comandos para comprobar configuración de red y conectividad.

| Descripción                 | Comandos        |
| --------------------------- | --------------- |
| Mostrar direcciones IP      | `ip addr`       |
| Mostrar tabla de rutas      | `ip route`      |
| Hacer ping a host           | `ping <host>`   |
| Mostrar puertos abiertos    | `netstat -tuln` |
| Comprobar conexión a URL    | `curl -I <url>` |
| Descargar archivo desde URL | `wget <url>`    |
| Test de velocidad de red    | `speedtest-cli` |
| Mostrar conexiones activas  | `ss -tuln`      |

---

### 6. Compresión y Archivos

**Descripción:** Comandos para comprimir y extraer archivos.

| Descripción         | Comandos                              |
| ------------------- | ------------------------------------- |
| Crear archivo tar   | `tar -cvf archivo.tar <archivos>`     |
| Extraer archivo tar | `tar -xvf archivo.tar`                |
| Crear archivo gzip  | `tar -czvf archivo.tar.gz <archivos>` |
| Extraer gzip        | `tar -xzvf archivo.tar.gz`            |
| Crear archivo zip   | `zip archivo.zip <archivos>`          |
| Extraer zip         | `unzip archivo.zip`                   |

---

### 7. Búsqueda y Filtrado

**Descripción:** Comandos para buscar texto, archivos y filtrar resultados.

| Descripción                  | Comandos                           |
| ---------------------------- | ---------------------------------- |
| Buscar texto en archivo      | `grep "patrón" <archivo>`          |
| Buscar recursivamente        | `grep -r "patrón" <directorio>`    |
| Buscar archivos por nombre   | `find <directorio> -name <patrón>` |
| Contar ocurrencias           | `grep -c "patrón" <archivo>`       |
| Mostrar columnas específicas | `awk '{print $1, $3}' <archivo>`   |
| Reemplazar texto en archivo  | `sed 's/viejo/nuevo/g' <archivo>`  |

---

### 8. Gestión de Paquetes

**Descripción:** Comandos para instalar, actualizar y eliminar paquetes.

| Descripción                    | Comandos                     |
| ------------------------------ | ---------------------------- |
| Actualizar repositorios apt    | `sudo apt update`            |
| Actualizar paquetes instalados | `sudo apt upgrade`           |
| Instalar paquete               | `sudo apt install <paquete>` |
| Eliminar paquete               | `sudo apt remove <paquete>`  |
| Buscar paquete                 | `apt search <paquete>`       |
| Instalar con yum               | `sudo yum install <paquete>` |
| Instalar con dnf               | `sudo dnf install <paquete>` |

---

### 9. Sistema e Información

**Descripción:** Comandos para obtener información del sistema y hardware.

| Descripción                    | Comandos              |
| ------------------------------ | --------------------- |
| Mostrar uso de disco           | `df -h`               |
| Mostrar tamaño de carpeta      | `du -sh <directorio>` |
| Mostrar memoria                | `free -h`             |
| Información de kernel y OS     | `uname -a`            |
