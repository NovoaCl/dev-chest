# Directorios

## Core Workflow Commands

| Description                                                                             |          Command          |
| --------------------------------------------------------------------------------------- | :-----------------------: |
| Inicializa un repositorio local nuevo.                                                  |        `git init`         |
| Crea una copia local de un repositorio remoto.                                          |     `git clone <url>`     |
| Muestra el status de los archivos en el directorio de trabajo y el area de preparación. |       `git status`        |
| Agrega un archivo especifico al area de preparación.                                    |     `git add <file>`      |
| Agrega todas las modificaciones del directorio.                                         |        `git add .`        |
| Registra los cambios como un commit nuevo con un mensaje descriptivo.                   | `git commit -m "message"` |
| Muestra las diferencias entre el directorio de trabajo y el área de preparación.        |        `git diff`         |

## Branching & Merging

| Description                                                    |         Command          |
| -------------------------------------------------------------- | :----------------------: |
| Crea una nueva rama.                                           |   `git branch <name>`    |
| Cambia a la rama especificada o al commit                      |  `git checkout <name>`   |
| Una alternativa moderna para cambiar de ramas.                 |   `git switch <name>`    |
| Borra una rama local(solo si ha sido mezclada).                | `git checkout -d <name>` |
| Combina los cambios de la rama especificada en la rama actual. |   `git merge <branch>`   |
| Elimina una rama local(solo si ha sido mezclada).              |  `git branch -d <name>`  |

## Remote Synchronization

| Description                                                                              |            Command            |
| ---------------------------------------------------------------------------------------- | :---------------------------: |
| Conecta un repositorio local a un servidor remoto.                                       | `git remote add <name> <url>` |
| Descarga cambios y ramas del repositorio remoto, pero no lo integra a las ramas locales. |          `git fetch`          |
| Busca cmabios y ramas del repositorio remoto y los mezcla en la rama local actual.       |          `git pull`           |
| Sube el commit local al repositorio remoto.                                              |          `git push`           |
| Se usa la primera vez establecer la upstream branch.                                     | `git push -u origin <branch>` |

## Utility & Inspection

| Description                                                                                 |      Command       |
| ------------------------------------------------------------------------------------------- | :----------------: |
| Muestra el historial de commits.                                                            |     `git log`      |
| Salva temporalmente los cambios que no estén listos para el commit limpiando el directorio. |    `git stash`     |
| Muestra que autor modificó cada linea de un archivo.                                        | `git blame <file>` |

## Others

| Description                       |                 Command                  |
| --------------------------------- | :--------------------------------------: |
| Establece o reescribe el usuario. |  `git config --global user.name "name"`  |
| Muestra el usuario.               |     `git config --global user.name`      |
| Establece o reescribe el email.   | `git config --global user.email "email"` |
| Muestra el email.                 |     `git config --global user.email`     |

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

==Nota: Los archivos relacionados al commit serán eliminados del repositorio local y remoto.==

1. Ejecutar `git rebase -i <repositorio-anterior-al-que-se-desea-eliminar>`
2. Se abrirá una interfaz Vim, cambiar los `pick` por `drop` de los commits a eliminar.
3. Presionar `Esc` y teclear `:wq`, precionar `Enter` para guardar y salir.
4. Ejecutar `git push origin master --force`

