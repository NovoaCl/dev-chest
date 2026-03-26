# Vim & Neovim Cheat Sheet / Hoja de Comandos

### 1. Editing Modes

*Vim and Neovim operate in different modes. Knowing them is fundamental.*

| Description                        | Commands |
| ---------------------------------- | -------- |
| Enter Insert mode                  | `i`      |
| Enter Insert mode after cursor     | `a`      |
| Open a new line below current line | `o`      |
| Open a new line above current line | `O`      |
| Exit to Normal mode                | `Esc`    |
| Enter Visual mode (character-wise) | `v`      |
| Enter Visual Line mode             | `V`      |
| Enter Visual Block mode            | `Ctrl+v` |
| Enter Command-line mode            | `:`      |

---

### 2. Navigation

*Efficient movement through text.*

| Description                 | Commands   |
| --------------------------- | ---------- |
| Move left                   | `h`        |
| Move down                   | `j`        |
| Move up                     | `k`        |
| Move right                  | `l`        |
| Go to beginning of line     | `0`        |
| Go to end of line           | `$`        |
| Go to top of file           | `gg`       |
| Go to end of file           | `G`        |
| Jump to matching brace      | `%`        |
| Search forward              | `/pattern` |
| Search backward             | `?pattern` |
| Repeat last search forward  | `n`        |
| Repeat last search backward | `N`        |

---

### 3. Editing Text

| Description              | Commands    |
| ------------------------ | ----------- |
| Delete current line      | `dd`        |
| Delete current character | `x`         |
| Change text in motion    | `c{motion}` |
| Undo last change         | `u`         |
| Redo undone change       | `Ctrl+r`    |
| Replace character        | `r<char>`   |
| Join lines               | `J`         |

---

### 4. Copy, Cut, Paste

| Description           | Commands    |
| --------------------- | ----------- |
| Yank (copy) line      | `yy`        |
| Yank text in motion   | `y{motion}` |
| Paste after cursor    | `p`         |
| Paste before cursor   | `P`         |
| Delete (cut) line     | `dd`        |
| Delete text in motion | `d{motion}` |

---

### 5. Search and Replace

| Description                 | Commands         |
| --------------------------- | ---------------- |
| Search forward              | `/pattern`       |
| Search backward             | `?pattern`       |
| Substitute in current line  | `:s/old/new/`    |
| Substitute globally in file | `:%s/old/new/g`  |
| Confirm each substitution   | `:%s/old/new/gc` |

---

### 6. File Management

| Description         | Commands      |
| ------------------- | ------------- |
| Save file           | `:w`          |
| Quit                | `:q`          |
| Save and quit       | `:wq`         |
| Quit without saving | `:q!`         |
| Edit another file   | `:e filename` |
| Reload file         | `:e!`         |

---

### 7. Windows and Splits

| Description           | Commands         |
| --------------------- | ---------------- |
| Horizontal split      | `:split`         |
| Vertical split        | `:vsplit`        |
| Move to another split | `Ctrl+w h/j/k/l` |
| Close current split   | `:close`         |

---

### 8. Buffers

| Description               | Commands          |
| ------------------------- | ----------------- |
| List buffers              | `:ls`             |
| Switch to next buffer     | `:bnext` or `:bn` |
| Switch to previous buffer | `:bprev` or `:bp` |
| Delete buffer             | `:bd`             |

---

### 9. Tabs

| Description          | Commands              |
| -------------------- | --------------------- |
| Open new tab         | `:tabnew`             |
| Move to next tab     | `:tabnext` or `:tabn` |
| Move to previous tab | `:tabprev` or `:tabp` |
| Close current tab    | `:tabclose`           |

---

### 10. Basic Configuration

| Description                      | Commands                                   |
| -------------------------------- | ------------------------------------------ |
| Open configuration file (Vim)    | `:e ~/.vimrc`                              |
| Open configuration file (Neovim) | `:e ~/.config/nvim/init.vim` or `init.lua` |
| Set option                       | `:set option`                              |
| Enable line numbers              | `:set number`                              |
| Disable line numbers             | `:set nonumber`                            |

---

### 11. Macros and Automation

| Description                    | Commands   |
| ------------------------------ | ---------- |
| Record macro into register `a` | `qa` … `q` |
| Play macro from register `a`   | `@a`       |
| Repeat last macro              | `@@`       |

---

### 12. Plugins (Neovim)

| Description                      | Commands         |
| -------------------------------- | ---------------- |
| Install plugin (example: packer) | `:PackerInstall` |
| Update plugins                   | `:PackerUpdate`  |
| Clean unused plugins             | `:PackerClean`   |
| Sync plugins                     | `:PackerSync`    |

---

### 13. Advanced Utilities

| Description                   | Commands                 |
| ----------------------------- | ------------------------ |
| Record search pattern         | `/pattern`               |
| Visual block insert           | `Ctrl+v` then `I` or `A` |
| Execute external command      | `:!command`              |
| Split window and run terminal | `:term` (Neovim)         |
| Toggle relative line numbers  | `:set relativenumber`    |

---

## **Versión en Español**

### 1. Modos de Edición

*Vim y Neovim funcionan en diferentes modos. Conocerlos es fundamental.*

| Descripción                                 | Comandos |
| ------------------------------------------- | -------- |
| Entrar en modo Inserción                    | `i`      |
| Entrar en modo Inserción después del cursor | `a`      |
| Abrir línea nueva debajo de la actual       | `o`      |
| Abrir línea nueva encima de la actual       | `O`      |
| Salir al modo Normal                        | `Esc`    |
| Entrar en modo Visual (carácter)            | `v`      |
| Entrar en modo Visual línea                 | `V`      |
| Entrar en modo Visual bloque                | `Ctrl+v` |
| Entrar en modo de línea de comandos         | `:`      |

---

### 2. Navegación

*Movimiento eficiente a través del texto.*

| Descripción                             | Comandos   |
| --------------------------------------- | ---------- |
| Mover a la izquierda                    | `h`        |
| Mover abajo                             | `j`        |
| Mover arriba                            | `k`        |
| Mover a la derecha                      | `l`        |
| Ir al inicio de la línea                | `0`        |
| Ir al final de la línea                 | `$`        |
| Ir al inicio del archivo                | `gg`       |
| Ir al final del archivo                 | `G`        |
| Saltar a paréntesis o llave coincidente | `%`        |
| Buscar hacia adelante                   | `/pattern` |
| Buscar hacia atrás                      | `?pattern` |
| Repetir última búsqueda hacia adelante  | `n`        |
| Repetir última búsqueda hacia atrás     | `N`        |

---

### 3. Edición de Texto

| Descripción                 | Comandos    |
| --------------------------- | ----------- |
| Borrar línea actual         | `dd`        |
| Borrar carácter actual      | `x`         |
| Cambiar texto en movimiento | `c{motion}` |
| Deshacer último cambio      | `u`         |
| Rehacer cambio deshecho     | `Ctrl+r`    |
| Reemplazar carácter         | `r<char>`   |
| Unir líneas                 | `J`         |

---

### 4. Copiar, Cortar y Pegar

| Descripción                | Comandos    |
| -------------------------- | ----------- |
| Copiar línea               | `yy`        |
| Copiar texto en movimiento | `y{motion}` |
| Pegar después del cursor   | `p`         |
| Pegar antes del cursor     | `P`         |
| Cortar línea               | `dd`        |
| Cortar texto en movimiento | `d{motion}` |

---

### 5. Buscar y Reemplazar

| Descripción                  | Comandos         |
| ---------------------------- | ---------------- |
| Buscar hacia adelante        | `/pattern`       |
| Buscar hacia atrás           | `?pattern`       |
| Sustituir en la línea actual | `:s/old/new/`    |
| Sustituir en todo el archivo | `:%s/old/new/g`  |
| Confirmar cada sustitución   | `:%s/old/new/gc` |

---

### 6. Manejo de Archivos

| Descripción        | Comandos      |
| ------------------ | ------------- |
| Guardar archivo    | `:w`          |
| Salir              | `:q`          |
| Guardar y salir    | `:wq`         |
| Salir sin guardar  | `:q!`         |
| Abrir otro archivo | `:e filename` |
| Recargar archivo   | `:e!`         |

---

### 7. Ventanas y Splits

| Descripción            | Comandos         |
| ---------------------- | ---------------- |
| División horizontal    | `:split`         |
| División vertical      | `:vsplit`        |
| Moverse a otra ventana | `Ctrl+w h/j/k/l` |
| Cerrar ventana actual  | `:close`         |

---

### 8. Buffers

| Descripción      | Comandos         |
| ---------------- | ---------------- |
| Listar buffers   | `:ls`            |
| Siguiente buffer | `:bnext` o `:bn` |
| Buffer anterior  | `:bprev` o `:bp` |
| Borrar buffer    | `:bd`            |

---

### 9. Pestañas

| Descripción           | Comandos             |
| --------------------- | -------------------- |
| Abrir nueva pestaña   | `:tabnew`            |
| Siguiente pestaña     | `:tabnext` o `:tabn` |
| Pestaña anterior      | `:tabprev` o `:tabp` |
| Cerrar pestaña actual | `:tabclose`          |

---

### 10. Configuración Básica

| Descripción                             | Comandos                                  |
| --------------------------------------- | ----------------------------------------- |
| Abrir archivo de configuración (Vim)    | `:e ~/.vimrc`                             |
| Abrir archivo de configuración (Neovim) | `:e ~/.config/nvim/init.vim` o `init.lua` |
| Configurar opción                       | `:set option`                             |
| Habilitar números de línea              | `:set number`                             |
| Deshabilitar números de línea           | `:set nonumber`                           |

---

### 11. Macros y Automatización

| Descripción                       | Comandos   |
| --------------------------------- | ---------- |
| Grabar macro en registro `a`      | `qa` … `q` |
| Ejecutar macro desde registro `a` | `@a`       |
| Repetir última macro              | `@@`       |

---

### 12. Plugins (Neovim)

| Descripción                       | Comandos         |
| --------------------------------- | ---------------- |
| Instalar plugin (ejemplo: packer) | `:PackerInstall` |
| Actualizar plugins                | `:PackerUpdate`  |
| Limpiar plugins no usados         | `:PackerClean`   |
| Sincronizar plugins               | `:PackerSync`    |

---

### 13. Utilidades Avanzadas

| Descripción                | Comandos                 |
| -------------------------- | ------------------------ |
| Grabar patrón de búsqueda  | `/pattern`               |
| Inserción en bloque visual | `Ctrl+v` luego `I` o `A` |
| Ejecutar comando externo   | `:!command`              |
| Abrir terminal en split    | `:term` (Neovim)         |
| Alternar números relativos | `:set relativenumber`    |

---
