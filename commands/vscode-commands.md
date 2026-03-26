# Visual Studio Code CLI Cheat Sheet / Hoja de Comandos de VS Code CLI

### 1. Opening Files and Folders

*Commands to open files, folders, or workspaces from the terminal.*

| Description                                    | Command                                |
| ---------------------------------------------- | -------------------------------------- |
| Open a file or folder                          | `code <file-or-folder>`                |
| Open in a new window                           | `code -n <file-or-folder>`             |
| Open in the last active window                 | `code -r <file-or-folder>`             |
| Open a specific workspace                      | `code <workspace-file>.code-workspace` |
| Wait until the file is closed before returning | `code -w <file>`                       |

---

### 2. Navigation and Windows

*Commands to control VS Code windows and focus from CLI.*

| Description                              | Command                      |
| ---------------------------------------- | ---------------------------- |
| Open VS Code with a new window           | `code -n`                    |
| Open VS Code with the last window        | `code -r`                    |
| Open with a specific user data directory | `code --user-data-dir <dir>` |
| Open with disabled extensions            | `code --disable-extensions`  |
| Open in verbose mode for debugging       | `code --verbose`             |

---

### 3. Extensions

*Managing extensions from the CLI.*

| Description                           | Command                                     |
| ------------------------------------- | ------------------------------------------- |
| List installed extensions             | `code --list-extensions`                    |
| Install an extension                  | `code --install-extension <extension-id>`   |
| Uninstall an extension                | `code --uninstall-extension <extension-id>` |
| Show detailed info about an extension | `code --show-versions`                      |

---

### 4. Configuration and Settings

*Commands for modifying or using settings via CLI.*

| Description                           | Command                                                                                                        |
| ------------------------------------- | -------------------------------------------------------------------------------------------------------------- |
| Open settings.json directly           | `code ~/.config/Code/User/settings.json` (Linux/macOS) <br> `code %APPDATA%\Code\User\settings.json` (Windows) |
| Launch VS Code with a specific locale | `code --locale <locale>`                                                                                       |
| Launch with a specific log level      | `code --log <level>`                                                                                           |
| Open keybindings.json                 | `code keybindings.json`                                                                                        |

---

### 5. Git Integration

*CLI commands useful for interacting with Git repositories in VS Code.*

| Description                            | Command                       |
| -------------------------------------- | ----------------------------- |
| Open a Git repository folder           | `code <repo-folder>`          |
| Open Git changes view for a repository | `code --diff <file1> <file2>` |
| Compare branches or commits via files  | `code --diff <file1> <file2>` |

---

### 6. Debugging

*Run or configure debugging sessions from CLI.*

| Description                         | Command                  |
| ----------------------------------- | ------------------------ |
| Open VS Code in debug verbose mode  | `code --verbose`         |
| Launch a debug session (task-based) | `code --task <taskName>` |

---

### 7. Advanced Utilities

*Tasks, snippets, workspace management, and other CLI options.*

| Description                                   | Command                           |
| --------------------------------------------- | --------------------------------- |
| Open a file and wait for it to be closed      | `code -w <file>`                  |
| Open VS Code with a new workspace             | `code -n <folder>`                |
| Open a workspace file                         | `code <workspace>.code-workspace` |
| List all CLI flags                            | `code --help`                     |
| Run a specific task from CLI                  | `code --task <taskName>`          |
| Open VS Code and specify extensions directory | `code --extensions-dir <dir>`     |
| Open VS Code and specify user data directory  | `code --user-data-dir <dir>`      |

---

## **Versión en Español**

### 1. Apertura de Archivos y Carpetas

*Comandos para abrir archivos, carpetas o workspaces desde la terminal.*

| Descripción                                              | Comando                                   |
| -------------------------------------------------------- | ----------------------------------------- |
| Abrir un archivo o carpeta                               | `code <archivo-o-carpeta>`                |
| Abrir en una ventana nueva                               | `code -n <archivo-o-carpeta>`             |
| Abrir en la última ventana activa                        | `code -r <archivo-o-carpeta>`             |
| Abrir un workspace específico                            | `code <archivo-workspace>.code-workspace` |
| Esperar hasta que se cierre el archivo antes de retornar | `code -w <archivo>`                       |

---

### 2. Navegación y Ventanas

*Comandos para controlar ventanas y enfoque de VS Code desde la CLI.*

| Descripción                                            | Comando                             |
| ------------------------------------------------------ | ----------------------------------- |
| Abrir VS Code en una ventana nueva                     | `code -n`                           |
| Abrir VS Code en la última ventana                     | `code -r`                           |
| Abrir con un directorio de datos de usuario específico | `code --user-data-dir <directorio>` |
| Abrir con extensiones deshabilitadas                   | `code --disable-extensions`         |
| Abrir en modo verbose para depuración                  | `code --verbose`                    |

---

### 3. Extensiones

*Administrar extensiones desde la CLI.*

| Descripción                                  | Comando                                     |
| -------------------------------------------- | ------------------------------------------- |
| Listar extensiones instaladas                | `code --list-extensions`                    |
| Instalar una extensión                       | `code --install-extension <id-extension>`   |
| Desinstalar una extensión                    | `code --uninstall-extension <id-extension>` |
| Mostrar información detallada de extensiones | `code --show-versions`                      |

---

### 4. Configuración y Ajustes

*Comandos para modificar o usar configuraciones desde la CLI.*

| Descripción                            | Comando                                                                                                        |
| -------------------------------------- | -------------------------------------------------------------------------------------------------------------- |
| Abrir settings.json directamente       | `code ~/.config/Code/User/settings.json` (Linux/macOS) <br> `code %APPDATA%\Code\User\settings.json` (Windows) |
| Abrir VS Code con un idioma específico | `code --locale <locale>`                                                                                       |
| Abrir con nivel de log específico      | `code --log <nivel>`                                                                                           |
| Abrir keybindings.json                 | `code keybindings.json`                                                                                        |

---

### 5. Integración con Git

*Comandos CLI útiles para interactuar con repositorios Git en VS Code.*

| Descripción                                | Comando                             |
| ------------------------------------------ | ----------------------------------- |
| Abrir carpeta de repositorio Git           | `code <carpeta-repo>`               |
| Abrir vista de cambios para un archivo     | `code --diff <archivo1> <archivo2>` |
| Comparar ramas o commits mediante archivos | `code --diff <archivo1> <archivo2>` |

---

### 6. Depuración

*Ejecutar o configurar sesiones de depuración desde la CLI.*

| Descripción                                     | Comando                      |
| ----------------------------------------------- | ---------------------------- |
| Abrir VS Code en modo verbose de depuración     | `code --verbose`             |
| Iniciar sesión de depuración (basada en tareas) | `code --task <nombre-tarea>` |

---

### 7. Utilidades Avanzadas

*Tareas, snippets, administración de workspaces y otras opciones de CLI.*

| Descripción                                                | Comando                              |
| ---------------------------------------------------------- | ------------------------------------ |
| Abrir un archivo y esperar a que se cierre                 | `code -w <archivo>`                  |
| Abrir VS Code con un workspace nuevo                       | `code -n <carpeta>`                  |
| Abrir un archivo de workspace                              | `code <workspace>.code-workspace`    |
| Listar todos los flags de la CLI                           | `code --help`                        |
| Ejecutar una tarea específica desde CLI                    | `code --task <nombre-tarea>`         |
| Abrir VS Code especificando directorio de extensiones      | `code --extensions-dir <directorio>` |
| Abrir VS Code especificando directorio de datos de usuario | `code --user-data-dir <directorio>`  |

---
