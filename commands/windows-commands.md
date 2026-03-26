# Windows Command Line Reference / Referencia de Línea de Comandos de Windows

### 1. File System Navigation

_Commands to move through folders and display contents._

| Description                 | Commands                                      |
| --------------------------- | --------------------------------------------- |
| List files and directories  | `dir` (CMD) <br> `Get-ChildItem` (PowerShell) |
| Change directory            | `cd <path>` (CMD/PowerShell)                  |
| Go to root of current drive | `cd\` (CMD/PowerShell)                        |
| Clear the screen            | `cls` (CMD/PowerShell)                        |
| Show current directory      | `cd` (CMD) <br> `Get-Location` (PowerShell)   |

---

### 2. File and Directory Management

_Commands to create, copy, move, rename, or delete files and directories._

| Description               | Commands                                                                                 |
| ------------------------- | ---------------------------------------------------------------------------------------- |
| Copy a file               | `copy <source> <destination>` (CMD) <br> `Copy-Item <source> <destination>` (PowerShell) |
| Move a file or folder     | `move <source> <destination>` (CMD) <br> `Move-Item <source> <destination>` (PowerShell) |
| Delete a file             | `del <file>` (CMD) <br> `Remove-Item <file>` (PowerShell)                                |
| Create a new directory    | `mkdir <folder>` (CMD/PowerShell)                                                        |
| Remove an empty directory | `rmdir <folder>` (CMD) <br> `Remove-Item <folder>` (PowerShell)                          |
| Rename a file or folder   | `ren <old> <new>` (CMD) <br> `Rename-Item <old> <new>` (PowerShell)                      |

---

### 3. Processes and Performance

_Monitor and manage running processes._

| Description             | Commands                                                                        |
| ----------------------- | ------------------------------------------------------------------------------- |
| List running processes  | `tasklist` (CMD) <br> `Get-Process` (PowerShell)                                |
| Kill a process by name  | `taskkill /IM <process>` (CMD) <br> `Stop-Process -Name <process>` (PowerShell) |
| Kill a process by PID   | `taskkill /PID <pid>` (CMD) <br> `Stop-Process -Id <pid>` (PowerShell)          |
| View system performance | `typeperf` (CMD) <br> `Get-Counter` (PowerShell)                                |

---

### 4. Networking

_Commands to check and manage network configurations._

| Description                  | Commands                                                   |
| ---------------------------- | ---------------------------------------------------------- |
| Show IP configuration        | `ipconfig /all` (CMD) <br> `Get-NetIPAddress` (PowerShell) |
| Test network connectivity    | `ping <host>` (CMD/PowerShell)                             |
| Show active connections      | `netstat -an` (CMD/PowerShell)                             |
| Display network interfaces   | `Get-NetAdapter` (PowerShell)                              |
| Release and renew DHCP lease | `ipconfig /release` <br> `ipconfig /renew` (CMD)           |

---

### 5. Users and Permissions

_Commands to manage user accounts and permissions._

| Description         | Commands                                                                                                                                                           |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| List user accounts  | `net user` (CMD) <br> `Get-LocalUser` (PowerShell)                                                                                                                 |
| Create a new user   | `net user <username> <password> /add` (CMD) <br> `New-LocalUser -Name <username> -Password (ConvertTo-SecureString "<password>" -AsPlainText -Force)` (PowerShell) |
| Delete a user       | `net user <username> /delete` (CMD) <br> `Remove-LocalUser -Name <username>` (PowerShell)                                                                          |
| Add user to a group | `net localgroup <group> <user> /add` (CMD) <br> `Add-LocalGroupMember -Group <group> -Member <user>` (PowerShell)                                                  |

---

### 6. System Information

_Commands to retrieve detailed system data._

| Description             | Commands                                                  |
| ----------------------- | --------------------------------------------------------- |
| Display system info     | `systeminfo` (CMD) <br> `Get-ComputerInfo` (PowerShell)   |
| Show OS version         | `ver` (CMD) <br> `(Get-ComputerInfo).OsName` (PowerShell) |
| List installed hotfixes | `wmic qfe list` (CMD) <br> `Get-HotFix` (PowerShell)      |

---

### 7. Disk Management

_Commands for disks, partitions, and file system checks._

| Description         | Commands                                                          |
| ------------------- | ----------------------------------------------------------------- |
| Check disk status   | `chkdsk <drive>` (CMD/PowerShell)                                 |
| Manage partitions   | `diskpart` (CMD)                                                  |
| List logical drives | `wmic logicaldisk get name` (CMD) <br> `Get-PSDrive` (PowerShell) |
| Format a drive      | `format <drive> /FS:<filesystem>` (CMD/PowerShell)                |

---

### 8. PowerShell Core Commands

_Key commands for daily administrative tasks in PowerShell._

| Description             | Commands                           |
| ----------------------- | ---------------------------------- |
| Get help on a cmdlet    | `Get-Help <cmdlet>`                |
| Update help content     | `Update-Help`                      |
| List installed modules  | `Get-Module -ListAvailable`        |
| Import a module         | `Import-Module <module>`           |
| Run scripts with policy | `Set-ExecutionPolicy RemoteSigned` |

---

### 9. System Administration

_Commands for managing services and scheduled tasks._

| Description             | Commands                                                                |
| ----------------------- | ----------------------------------------------------------------------- |
| List services           | `sc query` (CMD) <br> `Get-Service` (PowerShell)                        |
| Start a service         | `net start <service>` (CMD) <br> `Start-Service <service>` (PowerShell) |
| Stop a service          | `net stop <service>` (CMD) <br> `Stop-Service <service>` (PowerShell)   |
| View scheduled tasks    | `schtasks /query` (CMD) <br> `Get-ScheduledTask` (PowerShell)           |
| Create a scheduled task | `schtasks /create /tn <name> /tr <task> /sc <schedule>` (CMD)           |

---

### 10. Advanced Utilities

_Advanced commands and troubleshooting tools._

| Description                   | Commands                                                                        |                                        |
| ----------------------------- | ------------------------------------------------------------------------------- | -------------------------------------- |
| Display environment variables | `set` (CMD) <br> `Get-ChildItem Env:` (PowerShell)                              |                                        |
| Shutdown or restart           | `shutdown /s` / `shutdown /r` (CMD/PowerShell)                                  |                                        |
| Task automation scripts       | PowerShell scripts: `.\script.ps1`                                              |                                        |
| Export process list           | `tasklist > processes.txt` (CMD) <br> `Get-Process                              | Export-Csv processes.csv` (PowerShell) |
| Network diagnostics           | `tracert <host>` (CMD/PowerShell) <br> `Test-NetConnection <host>` (PowerShell) |                                        |

---

## **Versión en Español**

### 1. Navegación del Sistema de Archivos

_Comandos para moverse por carpetas y mostrar contenido._

| Descripción                      | Comandos                                      |
| -------------------------------- | --------------------------------------------- |
| Listar archivos y directorios    | `dir` (CMD) <br> `Get-ChildItem` (PowerShell) |
| Cambiar directorio               | `cd <ruta>` (CMD/PowerShell)                  |
| Ir a la raíz de la unidad actual | `cd\` (CMD/PowerShell)                        |
| Limpiar pantalla                 | `cls` (CMD/PowerShell)                        |
| Mostrar directorio actual        | `cd` (CMD) <br> `Get-Location` (PowerShell)   |

---

### 2. Gestión de Archivos y Directorios

_Comandos para crear, copiar, mover, renombrar o eliminar archivos y carpetas._

| Descripción                 | Comandos                                                                         |
| --------------------------- | -------------------------------------------------------------------------------- |
| Copiar un archivo           | `copy <origen> <destino>` (CMD) <br> `Copy-Item <origen> <destino>` (PowerShell) |
| Mover un archivo o carpeta  | `move <origen> <destino>` (CMD) <br> `Move-Item <origen> <destino>` (PowerShell) |
| Eliminar un archivo         | `del <archivo>` (CMD) <br> `Remove-Item <archivo>` (PowerShell)                  |
| Crear un directorio         | `mkdir <carpeta>` (CMD/PowerShell)                                               |
| Eliminar directorio vacío   | `rmdir <carpeta>` (CMD) <br> `Remove-Item <carpeta>` (PowerShell)                |
| Renombrar archivo o carpeta | `ren <antiguo> <nuevo>` (CMD) <br> `Rename-Item <antiguo> <nuevo>` (PowerShell)  |

---

### 3. Procesos y Rendimiento

_Monitorear y gestionar procesos en ejecución._

| Descripción                  | Comandos                                                                        |
| ---------------------------- | ------------------------------------------------------------------------------- |
| Listar procesos en ejecución | `tasklist` (CMD) <br> `Get-Process` (PowerShell)                                |
| Finalizar proceso por nombre | `taskkill /IM <proceso>` (CMD) <br> `Stop-Process -Name <proceso>` (PowerShell) |
| Finalizar proceso por PID    | `taskkill /PID <pid>` (CMD) <br> `Stop-Process -Id <pid>` (PowerShell)          |
| Ver rendimiento del sistema  | `typeperf` (CMD) <br> `Get-Counter` (PowerShell)                                |

---

### 4. Redes

_Comandos para revisar y administrar configuración de red._

| Descripción                | Comandos                                                   |
| -------------------------- | ---------------------------------------------------------- |
| Mostrar configuración IP   | `ipconfig /all` (CMD) <br> `Get-NetIPAddress` (PowerShell) |
| Probar conectividad        | `ping <host>` (CMD/PowerShell)                             |
| Mostrar conexiones activas | `netstat -an` (CMD/PowerShell)                             |
| Mostrar interfaces de red  | `Get-NetAdapter` (PowerShell)                              |
| Liberar y renovar IP DHCP  | `ipconfig /release` <br> `ipconfig /renew` (CMD)           |

---

### 5. Usuarios y Permisos

_Comandos para gestionar cuentas de usuario y permisos._

| Descripción               | Comandos                                                                                                                                                             |
| ------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Listar cuentas de usuario | `net user` (CMD) <br> `Get-LocalUser` (PowerShell)                                                                                                                   |
| Crear usuario nuevo       | `net user <usuario> <contraseña> /add` (CMD) <br> `New-LocalUser -Name <usuario> -Password (ConvertTo-SecureString "<contraseña>" -AsPlainText -Force)` (PowerShell) |
| Eliminar usuario          | `net user <usuario> /delete` (CMD) <br> `Remove-LocalUser -Name <usuario>` (PowerShell)                                                                              |
| Agregar usuario a grupo   | `net localgroup <grupo> <usuario> /add` (CMD) <br> `Add-LocalGroupMember -Group <grupo> -Member <usuario>` (PowerShell)                                              |

---

### 6. Información del Sistema

_Comandos para obtener información detallada del sistema._

| Descripción                       | Comandos                                                  |
| --------------------------------- | --------------------------------------------------------- |
| Mostrar información del sistema   | `systeminfo` (CMD) <br> `Get-ComputerInfo` (PowerShell)   |
| Mostrar versión de OS             | `ver` (CMD) <br> `(Get-ComputerInfo).OsName` (PowerShell) |
| Listar actualizaciones instaladas | `wmic qfe list` (CMD) <br> `Get-HotFix` (PowerShell)      |

---

### 7. Gestión de Discos

_Comandos para discos, particiones y revisión de sistema de archivos._

| Descripción               | Comandos                                                          |
| ------------------------- | ----------------------------------------------------------------- |
| Comprobar estado de disco | `chkdsk <unidad>` (CMD/PowerShell)                                |
| Administrar particiones   | `diskpart` (CMD)                                                  |
| Listar unidades lógicas   | `wmic logicaldisk get name` (CMD) <br> `Get-PSDrive` (PowerShell) |
| Formatear unidad          | `format <unidad> /FS:<sistema-de-archivos>` (CMD/PowerShell)      |

---

### 8. Comandos Clave de PowerShell

| Descripción                   | Comandos                           |
| ----------------------------- | ---------------------------------- |
| Obtener ayuda sobre un cmdlet | `Get-Help <cmdlet>`                |
| Actualizar ayuda              | `Update-Help`                      |
| Listar módulos instalados     | `Get-Module -ListAvailable`        |
| Importar módulo               | `Import-Module <modulo>`           |
| Ejecutar scripts con política | `Set-ExecutionPolicy RemoteSigned` |

---

### 9. Administración del Sistema

| Descripción            | Comandos                                                                  |
| ---------------------- | ------------------------------------------------------------------------- |
| Listar servicios       | `sc query` (CMD) <br> `Get-Service` (PowerShell)                          |
| Iniciar servicio       | `net start <servicio>` (CMD) <br> `Start-Service <servicio>` (PowerShell) |
| Detener servicio       | `net stop <servicio>` (CMD) <br> `Stop-Service <servicio>` (PowerShell)   |
| Ver tareas programadas | `schtasks /query` (CMD) <br> `Get-ScheduledTask` (PowerShell)             |
| Crear tarea programada | `schtasks /create /tn <nombre> /tr <tarea> /sc <programa>` (CMD)          |

---

### 10. Utilidades Avanzadas

| Descripción                        | Comandos                                                                        |                                       |
| ---------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------- |
| Mostrar variables de entorno       | `set` (CMD) <br> `Get-ChildItem Env:` (PowerShell)                              |                                       |
| Apagar o reiniciar                 | `shutdown /s` / `shutdown /r` (CMD/PowerShell)                                  |                                       |
| Ejecutar scripts de automatización | `.\script.ps1` (PowerShell)                                                     |                                       |
| Exportar lista de procesos         | `tasklist > procesos.txt` (CMD) <br> `Get-Process                               | Export-Csv procesos.csv` (PowerShell) |
| Diagnóstico de red                 | `tracert <host>` (CMD/PowerShell) <br> `Test-NetConnection <host>` (PowerShell) |                                       |

---

### 11. Others

| Descripción                         | Comandos                    |
| ----------------------------------- | --------------------------- |
| Genera un arbol dentro del archivo. | `tree /F /A > repo_tree.md` |
