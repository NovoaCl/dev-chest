# Angular CLI Command Reference / Referencia de Comandos de Angular CLI

### 1. Initialization and Configuration

**Description:** Commands to create new Angular projects, configure workspace settings, and manage Angular versions.

| Description                                             | Commands                             |
| ------------------------------------------------------- | ------------------------------------ |
| Create a new Angular project                            | `ng new <project-name>`              |
| Add Angular routing to a project                        | `ng new <project-name> --routing`    |
| Specify stylesheet format (CSS, SCSS, SASS, LESS, etc.) | `ng new <project-name> --style=scss` |
| Add Angular CLI to an existing project                  | `ng add @angular/cli`                |
| Update Angular CLI and core packages                    | `ng update`                          |
| List installed Angular CLI packages                     | `ng version`                         |
| Configure Angular workspace settings                    | `ng config <key> <value>`            |

---

### 2. Code Generation

**Description:** Commands to scaffold Angular components, services, modules, directives, pipes, and more.

| Description              | Commands                                              |
| ------------------------ | ----------------------------------------------------- |
| Generate a new component | `ng generate component <name>` or `ng g c <name>`     |
| Generate a new module    | `ng generate module <name>` or `ng g m <name>`        |
| Generate a new service   | `ng generate service <name>` or `ng g s <name>`       |
| Generate a new directive | `ng generate directive <name>` or `ng g d <name>`     |
| Generate a new pipe      | `ng generate pipe <name>` or `ng g p <name>`          |
| Generate a class         | `ng generate class <name>` or `ng g cl <name>`        |
| Generate an interface    | `ng generate interface <name>` or `ng g i <name>`     |
| Generate an enum         | `ng generate enum <name>` or `ng g e <name>`          |
| Generate a guard         | `ng generate guard <name>` or `ng g g <name>`         |
| Generate a library       | `ng generate library <name>` or `ng g library <name>` |

---

### 3. Development

**Description:** Commands to serve the application locally and monitor changes during development.

| Description                           | Commands                            |
| ------------------------------------- | ----------------------------------- |
| Serve application locally             | `ng serve`                          |
| Serve on a specific port              | `ng serve --port <number>`          |
| Serve with a specific configuration   | `ng serve --configuration=<config>` |
| Watch files and rebuild automatically | `ng build --watch`                  |
| Run in production mode                | `ng serve --prod`                   |

---

### 4. Build

**Description:** Commands to compile and optimize Angular applications for deployment.

| Description                         | Commands                            |
| ----------------------------------- | ----------------------------------- |
| Build project for development       | `ng build`                          |
| Build project for production        | `ng build --prod`                   |
| Build with a specific configuration | `ng build --configuration=<config>` |
| Build and output stats for analysis | `ng build --stats-json`             |
| Build a library                     | `ng build <library-name>`           |

---

### 5. Testing

**Description:** Commands for unit testing, end-to-end testing, and code coverage analysis.

| Description                                        | Commands                           |
| -------------------------------------------------- | ---------------------------------- |
| Run unit tests (Karma/Jasmine)                     | `ng test`                          |
| Run tests with code coverage report                | `ng test --code-coverage`          |
| Run tests with a specific configuration            | `ng test --configuration=<config>` |
| Run end-to-end tests (Protractor)                  | `ng e2e`                           |
| Run end-to-end tests with a specific configuration | `ng e2e --configuration=<config>`  |

---

### 6. Deployment

**Description:** Commands to deploy Angular applications to different environments or services.

| Description                        | Commands                             |
| ---------------------------------- | ------------------------------------ |
| Build and deploy using Angular CLI | `ng deploy`                          |
| Deploy to GitHub Pages             | `ng deploy --base-href=/`            |
| Deploy with a specific builder     | `ng deploy --builder=<builder-name>` |

---

### 7. Maintenance and Utilities

**Description:** Commands to manage dependencies, linting, formatting, and miscellaneous tasks.

| Description                               | Commands                                      |
| ----------------------------------------- | --------------------------------------------- |
| Lint project files                        | `ng lint`                                     |
| Run format check                          | `ng lint --fix`                               |
| Analyze bundle sizes                      | `ng build --stats-json`                       |
| Serve bundle analyzer                     | `npx webpack-bundle-analyzer dist/stats.json` |
| Run Angular schematic                     | `ng generate <schematic>`                     |
| Display Angular CLI help                  | `ng help`                                     |
| Display help for a specific command       | `ng <command> --help`                         |
| Clean node_modules and reinstall packages | `rm -rf node_modules && npm install`          |

---

## Versión en Español

### 1. Inicialización y Configuración

**Descripción:** Comandos para crear nuevos proyectos Angular, configurar el workspace y gestionar versiones de Angular.

| Descripción                                                          | Comandos                                |
| -------------------------------------------------------------------- | --------------------------------------- |
| Crear un nuevo proyecto Angular                                      | `ng new <nombre-proyecto>`              |
| Agregar routing al proyecto                                          | `ng new <nombre-proyecto> --routing`    |
| Especificar formato de hojas de estilo (CSS, SCSS, SASS, LESS, etc.) | `ng new <nombre-proyecto> --style=scss` |
| Agregar Angular CLI a un proyecto existente                          | `ng add @angular/cli`                   |
| Actualizar Angular CLI y paquetes principales                        | `ng update`                             |
| Listar paquetes de Angular instalados                                | `ng version`                            |
| Configurar opciones del workspace de Angular                         | `ng config <clave> <valor>`             |

---

### 2. Generación de Código

**Descripción:** Comandos para generar componentes, servicios, módulos, directivas, pipes y más.

| Descripción                 | Comandos                                                 |
| --------------------------- | -------------------------------------------------------- |
| Generar un nuevo componente | `ng generate component <nombre>` o `ng g c <nombre>`     |
| Generar un nuevo módulo     | `ng generate module <nombre>` o `ng g m <nombre>`        |
| Generar un nuevo servicio   | `ng generate service <nombre>` o `ng g s <nombre>`       |
| Generar una nueva directiva | `ng generate directive <nombre>` o `ng g d <nombre>`     |
| Generar un nuevo pipe       | `ng generate pipe <nombre>` o `ng g p <nombre>`          |
| Generar una clase           | `ng generate class <nombre>` o `ng g cl <nombre>`        |
| Generar una interfaz        | `ng generate interface <nombre>` o `ng g i <nombre>`     |
| Generar un enum             | `ng generate enum <nombre>` o `ng g e <nombre>`          |
| Generar un guard            | `ng generate guard <nombre>` o `ng g g <nombre>`         |
| Generar una librería        | `ng generate library <nombre>` o `ng g library <nombre>` |

---

### 3. Desarrollo

**Descripción:** Comandos para servir la aplicación localmente y monitorear cambios durante el desarrollo.

| Descripción                                     | Comandos                            |
| ----------------------------------------------- | ----------------------------------- |
| Servir la aplicación localmente                 | `ng serve`                          |
| Servir en un puerto específico                  | `ng serve --port <número>`          |
| Servir con una configuración específica         | `ng serve --configuration=<config>` |
| Observar archivos y reconstruir automáticamente | `ng build --watch`                  |
| Ejecutar en modo producción                     | `ng serve --prod`                   |

---

### 4. Construcción (Build)

**Descripción:** Comandos para compilar y optimizar aplicaciones Angular para despliegue.

| Descripción                                    | Comandos                            |
| ---------------------------------------------- | ----------------------------------- |
| Construir proyecto en desarrollo               | `ng build`                          |
| Construir proyecto en producción               | `ng build --prod`                   |
| Construir con configuración específica         | `ng build --configuration=<config>` |
| Construir y generar estadísticas para análisis | `ng build --stats-json`             |
| Construir una librería                         | `ng build <nombre-librería>`        |

---

### 5. Testing

**Descripción:** Comandos para pruebas unitarias, end-to-end y análisis de cobertura de código.

| Descripción                                              | Comandos                           |
| -------------------------------------------------------- | ---------------------------------- |
| Ejecutar pruebas unitarias (Karma/Jasmine)               | `ng test`                          |
| Ejecutar pruebas con reporte de cobertura                | `ng test --code-coverage`          |
| Ejecutar pruebas con configuración específica            | `ng test --configuration=<config>` |
| Ejecutar pruebas end-to-end (Protractor)                 | `ng e2e`                           |
| Ejecutar pruebas end-to-end con configuración específica | `ng e2e --configuration=<config>`  |

---

### 6. Despliegue

**Descripción:** Comandos para desplegar aplicaciones Angular en diferentes entornos o servicios.

| Descripción                              | Comandos                             |
| ---------------------------------------- | ------------------------------------ |
| Construir y desplegar usando Angular CLI | `ng deploy`                          |
| Desplegar en GitHub Pages                | `ng deploy --base-href=/`            |
| Desplegar con un builder específico      | `ng deploy --builder=<builder-name>` |

---

### 7. Mantenimiento y Utilidades

**Descripción:** Comandos para gestión de dependencias, linting, formateo y tareas auxiliares.

| Descripción                                | Comandos                                      |
| ------------------------------------------ | --------------------------------------------- |
| Analizar código con lint                   | `ng lint`                                     |
| Ejecutar corrección automática de lint     | `ng lint --fix`                               |
| Analizar tamaños de bundles                | `ng build --stats-json`                       |
| Servir análisis de bundle                  | `npx webpack-bundle-analyzer dist/stats.json` |
| Ejecutar un schematic de Angular           | `ng generate <schematic>`                     |
| Mostrar ayuda de Angular CLI               | `ng help`                                     |
| Mostrar ayuda de un comando específico     | `ng <command> --help`                         |
| Limpiar node_modules y reinstalar paquetes | `rm -rf node_modules && npm install`          |

