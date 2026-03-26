
# Git Command Reference / Referencia de Comandos de Git

### 1. Initial Configuration

**Description:** Commands to configure Git for the first time and set global preferences.

| Description                     | Commands                                                  |
| ------------------------------- | --------------------------------------------------------- |
| Set user name                   | `git config --global user.name "Your Name"`               |
| Set user email                  | `git config --global user.email "your.email@example.com"` |
| Check current configuration     | `git config --list`                                       |
| Set default text editor         | `git config --global core.editor "vim"`                   |
| Initialize a new Git repository | `git init`                                                |
| Clone a remote repository       | `git clone <repository_url>`                              |

---

### 2. Workflow

**Description:** Commands for basic workflow operations in Git.

| Description              | Commands                         |
| ------------------------ | -------------------------------- |
| Show repository status   | `git status`                     |
| Add file to staging area | `git add <file>`                 |
| Add all changes          | `git add .`                      |
| Commit staged changes    | `git commit -m "Commit message"` |
| Amend the last commit    | `git commit --amend`             |

---

### 3. Branching & Merging

**Description:** Commands to create, switch, merge, and manage branches.

| Description                        | Commands                                 |
| ---------------------------------- | ---------------------------------------- |
| List branches                      | `git branch`                             |
| Create a new branch                | `git branch <branch_name>`               |
| Switch to a branch                 | `git checkout <branch_name>`             |
| Switch to a branch (modern)        | `git switch <branch_name>`               |
| Create and switch                  | `git checkout -b <branch_name>`          |
| Merge branch into current          | `git merge <branch_name>`                |
| Rebase current branch onto another | `git rebase <branch_name>`               |
| Delete a branch locally            | `git branch -d <branch_name>`            |
| Delete a branch remotely           | `git push origin --delete <branch_name>` |

---

### 4. Remote Synchronization

**Description:** Commands to interact with remote repositories.

| Description               | Commands                        |
| ------------------------- | ------------------------------- |
| Show remote repositories  | `git remote -v`                 |
| Add a remote repository   | `git remote add <name> <url>`   |
| Fetch changes from remote | `git fetch <remote>`            |
| Pull changes and merge    | `git pull <remote> <branch>`    |
| Push changes to remote    | `git push <remote> <branch>`    |
| Set upstream branch       | `git push -u <remote> <branch>` |

---

### 5. History & Inspection

**Description:** Commands to inspect commit history, changes, and differences.

| Description                       | Commands            |
| --------------------------------- | ------------------- |
| Show commit history               | `git log`           |
| Show one-line history             | `git log --oneline` |
| Show history of a file            | `git log <file>`    |
| Show changes in working directory | `git diff`          |
| Show changes staged for commit    | `git diff --staged` |
| Show specific commit details      | `git show <commit>` |

---

### 6. Staging & Commits

**Description:** Commands to manage staging and commit process efficiently.

| Description                           | Commands                       |
| ------------------------------------- | ------------------------------ |
| Unstage a file                        | `git reset <file>`             |
| Unstage all files                     | `git reset`                    |
| Stage specific lines interactively    | `git add -p`                   |
| Amend commit without changing message | `git commit --amend --no-edit` |
| Revert a commit                       | `git revert <commit>`          |

---

### 7. History Rewriting

**Description:** Commands to modify or rewrite commit history.

| Description                        | Commands                                     |
| ---------------------------------- | -------------------------------------------- |
| Reset branch to previous commit    | `git reset --hard <commit>`                  |
| Soft reset (keep changes)          | `git reset --soft <commit>`                  |
| Interactive rebase to edit history | `git rebase -i <commit>`                     |
| Squash commits                     | `git rebase -i <commit>` and combine commits |

---

### 8. Stash

**Description:** Commands to temporarily save changes without committing.

| Description                 | Commands                   |
| --------------------------- | -------------------------- |
| Save changes to stash       | `git stash`                |
| List stashes                | `git stash list`           |
| Apply latest stash          | `git stash apply`          |
| Apply and drop latest stash | `git stash pop`            |
| Drop a specific stash       | `git stash drop stash@{0}` |
| Clear all stashes           | `git stash clear`          |

---

### 9. Tags

**Description:** Commands to manage tags for marking versions or releases.

| Description              | Commands                              |
| ------------------------ | ------------------------------------- |
| List tags                | `git tag`                             |
| Create a lightweight tag | `git tag <tag_name>`                  |
| Create an annotated tag  | `git tag -a <tag_name> -m "Message"`  |
| Push tags to remote      | `git push origin <tag_name>`          |
| Push all tags            | `git push origin --tags`              |
| Delete a tag locally     | `git tag -d <tag_name>`               |
| Delete a tag remotely    | `git push origin --delete <tag_name>` |

---

### 10. Submodules

**Description:** Commands to manage submodules in a repository.

| Description                        | Commands                                |
| ---------------------------------- | --------------------------------------- |
| Add a submodule                    | `git submodule add <repository> <path>` |
| Initialize submodules              | `git submodule init`                    |
| Update submodules                  | `git submodule update`                  |
| Clone a repo with submodules       | `git clone --recurse-submodules <repo>` |
| Update submodules to latest commit | `git submodule update --remote`         |

---

### 11. Utilities

**Description:** Miscellaneous commands to facilitate Git workflows.

| Description                       | Commands                        |
| --------------------------------- | ------------------------------- |
| Show current branch               | `git branch --show-current`     |
| Show repository status succinctly | `git status -s`                 |
| Show last commit                  | `git log -1`                    |
| Clean untracked files             | `git clean -f`                  |
| Show ignored files                | `git status --ignored`          |
| Compare branches                  | `git diff <branch1>..<branch2>` |

---

## Versión en Español

### 1. Configuración Inicial

**Descripción:** Comandos para configurar Git por primera vez y establecer preferencias globales.

| Descripción                      | Comandos                                                |
| -------------------------------- | ------------------------------------------------------- |
| Configurar nombre de usuario     | `git config --global user.name "Tu Nombre"`             |
| Configurar correo electrónico    | `git config --global user.email "tu.email@ejemplo.com"` |
| Ver configuración actual         | `git config --list`                                     |
| Configurar editor de texto       | `git config --global core.editor "vim"`                 |
| Inicializar un repositorio nuevo | `git init`                                              |
| Clonar un repositorio remoto     | `git clone <url_del_repositorio>`                       |

---

### 2. Flujo de Trabajo (Workflow)

**Descripción:** Comandos para operaciones básicas de flujo de trabajo.

| Descripción                    | Comandos                             |
| ------------------------------ | ------------------------------------ |
| Mostrar estado del repositorio | `git status`                         |
| Agregar archivo al staging     | `git add <archivo>`                  |
| Agregar todos los cambios      | `git add .`                          |
| Hacer commit de cambios staged | `git commit -m "Mensaje del commit"` |
| Modificar último commit        | `git commit --amend`                 |

---

### 3. Gestión de Ramas

**Descripción:** Comandos para crear, cambiar, fusionar y gestionar ramas.

| Descripción                      | Comandos                                 |
| -------------------------------- | ---------------------------------------- |
| Listar ramas                     | `git branch`                             |
| Crear nueva rama                 | `git branch <nombre_rama>`               |
| Cambiar a una rama               | `git checkout <nombre_rama>`             |
| Cambiar a una rama (moderno)     | `git switch <nombre_rama>`               |
| Crear y cambiar de rama          | `git checkout -b <nombre_rama>`          |
| Fusionar rama en actual          | `git merge <nombre_rama>`                |
| Rebase de rama actual sobre otra | `git rebase <nombre_rama>`               |
| Eliminar rama local              | `git branch -d <nombre_rama>`            |
| Eliminar rama remota             | `git push origin --delete <nombre_rama>` |

---

### 4. Sincronización Remota

**Descripción:** Comandos para interactuar con repositorios remotos.

| Descripción                 | Comandos                        |
| --------------------------- | ------------------------------- |
| Listar repositorios remotos | `git remote -v`                 |
| Agregar repositorio remoto  | `git remote add <nombre> <url>` |
| Descargar cambios de remoto | `git fetch <remoto>`            |
| Traer y fusionar cambios    | `git pull <remoto> <rama>`      |
| Enviar cambios a remoto     | `git push <remoto> <rama>`      |
| Establecer upstream         | `git push -u <remoto> <rama>`   |

---

### 5. Historial e Inspección

**Descripción:** Comandos para inspeccionar historial de commits y cambios.

| Descripción                          | Comandos            |
| ------------------------------------ | ------------------- |
| Mostrar historial de commits         | `git log`           |
| Mostrar historial resumido           | `git log --oneline` |
| Historial de un archivo              | `git log <archivo>` |
| Mostrar cambios en working directory | `git diff`          |
| Mostrar cambios staged               | `git diff --staged` |
| Detalles de un commit específico     | `git show <commit>` |

---

### 6. Staging y Commits

**Descripción:** Comandos para manejar staging y commits de forma eficiente.

| Descripción                           | Comandos                       |
| ------------------------------------- | ------------------------------ |
| Quitar archivo del staging            | `git reset <archivo>`          |
| Quitar todos los archivos del staging | `git reset`                    |
| Staging interactivo por líneas        | `git add -p`                   |
| Modificar commit sin cambiar mensaje  | `git commit --amend --no-edit` |
| Revertir un commit                    | `git revert <commit>`          |

---

### 7. Reescritura de Historial

**Descripción:** Comandos para modificar o reescribir el historial de commits.

| Descripción                     | Comandos                                    |
| ------------------------------- | ------------------------------------------- |
| Reset de rama a commit anterior | `git reset --hard <commit>`                 |
| Soft reset (mantener cambios)   | `git reset --soft <commit>`                 |
| Rebase interactivo              | `git rebase -i <commit>`                    |
| Squash de commits               | `git rebase -i <commit>` y combinar commits |

---

### 8. Stash

**Descripción:** Comandos para guardar temporalmente cambios sin hacer commit.

| Descripción                     | Comandos                   |
| ------------------------------- | -------------------------- |
| Guardar cambios en stash        | `git stash`                |
| Listar stashes                  | `git stash list`           |
| Aplicar último stash            | `git stash apply`          |
| Aplicar y eliminar último stash | `git stash pop`            |
| Eliminar un stash específico    | `git stash drop stash@{0}` |
| Limpiar todos los stashes       | `git stash clear`          |

---

### 9. Tags

**Descripción:** Comandos para manejar tags y marcar versiones o releases.

| Descripción           | Comandos                              |
| --------------------- | ------------------------------------- |
| Listar tags           | `git tag`                             |
| Crear tag ligero      | `git tag <tag_name>`                  |
| Crear tag anotado     | `git tag -a <tag_name> -m "Mensaje"`  |
| Enviar tag a remoto   | `git push origin <tag_name>`          |
| Enviar todos los tags | `git push origin --tags`              |
| Eliminar tag local    | `git tag -d <tag_name>`               |
| Eliminar tag remoto   | `git push origin --delete <tag_name>` |

---

### 10. Submódulos

**Descripción:** Comandos para manejar submódulos en un repositorio.

| Descripción                            | Comandos                                 |
| -------------------------------------- | ---------------------------------------- |
| Agregar un submódulo                   | `git submodule add <repositorio> <ruta>` |
| Inicializar submódulos                 | `git submodule init`                     |
| Actualizar submódulos                  | `git submodule update`                   |
| Clonar repositorio con submódulos      | `git clone --recurse-submodules <repo>`  |
| Actualizar submódulos al último commit | `git submodule update --remote`          |

---

### 11. Utilidades

**Descripción:** Comandos varios para facilitar flujos de trabajo con Git.

| Descripción                    | Comandos                    |
| ------------------------------ | --------------------------- |
| Mostrar rama actual            | `git branch --show-current` |
| Estado resumido                | `git status -s`             |
| Último commit                  | `git log -1`                |
| Limpiar archivos no trackeados | `git clean -f`              |
| Mostrar archivos ignorados     | `git status --ignored`      |
| Comparar ramas                 | `git diff <rama1>..<rama2>` |

---

## How to set up a new local repository:

```git
cd ruta/del/repositorio
git init
git add .
git commit -m "Inicial commit: de algo"
git branch -M master
git remote add origin <link-repo>
git push origin main
```
## How to upload a repository:

```git
git add .
git commit -m "Commit message"
git push
```

## How to delete a commit

`Nota: Los archivos relacionados al commit serán eliminados del repositorio local y remoto.`

1. Ejecutar `git rebase -i <repositorio-anterior-al-que-se-desea-eliminar>`
2. Se abrirá una interfaz Vim, cambiar los `pick` por `drop` de los commits a eliminar.
3. Presionar `Esc` y teclear `:wq`, precionar `Enter` para guardar y salir.
4. Ejecutar `git push origin master --force`

