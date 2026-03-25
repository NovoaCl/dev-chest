## Vim 25-03-2026

`https://www.youtube.com/watch?v=9XpvT2IEIB0`

1. Intro
2. Vim y NeoVim
3. Primeros pasos en Vim
4. Navegación
5. Edición
6. Modos de selección
7. Búsquedas y remplazo
8. Registers
9. Macros
10. Buffers y ventanas
11. Tips y trucos
12. Neo Vim
13. Configuraciones de la comunidad.

## Vim

Editor de texto, perfecto para programar, funciona desde la terminal, ligero y consume muy pocos recursos, configurable, funciona para cualquier lenguaje de programación, multitarea.

Modos:
- Insertar
- Normal
- Visual
- Comando

## NeoVim

Es un fork de Vim, version más moderna y extensible. Puede utilizar LUA para configuración, crear temas y plugins, tiene soporte nativo para LSP(Language SErver Protocol) lo que nos dara funcionalidades como autocompletado, saltar a definiciones, disgnostico de errores.
Vim + Lua + LSP

## Tips

- Todo es diferente
- Touch typing, mecanografía
- Aprender los atajos
- Hojas de ayuda

## Instalar WSL2

*Herramienta para generar una imagen de linux Ubuntu

- `wsl --install`:Comando para instalarlo:
- `Ctrl + Shift + 4`: Abre la terminal de ubuntu.
- `pwd`
- Entrar al usuario de ubuntu y generar un directorio para el curso.
- Generar el acceso directo al directorio

## Instalar Homebrew

Emulador de terminal, da más caracteristicas, personalizacion 

#### Instrucciones:
1. Instalar Homebrew desde la terminal de ubuntu
2. Ejecutar este comando para agregar la direccion de instalación a PATH:

```bash
echo 'eval "$(/home/linuxbrew/.linuxbrew/bin/brew shellenv)"' >> ~/.bashrc
eval "$(/home/linuxbrew/.linuxbrew/bin/brew shellenv)"
```
3. Consultar la version de homebrew con `brew -v`

### Instalar NeoVim


