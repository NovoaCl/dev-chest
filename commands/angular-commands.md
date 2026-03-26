# Angular CLI Command Reference

A structured and practical reference for the most commonly used Angular CLI commands, organized by workflow.

---

## 📦 1. Project Setup

**Description:** Commands used to install Angular CLI and create new projects.

| Description                                | Commands                      |
| ------------------------------------------ | ----------------------------- |
| Install Angular CLI globally               | `npm install -g @angular/cli` |
| Check Angular CLI version                  | `ng version`                  |
| Create a new Angular project               | `ng new my-app`               |
| Create project with routing                | `ng new my-app --routing`     |
| Create project with specific stylesheet    | `ng new my-app --style=scss`  |
| Add Angular features (PWA, Material, etc.) | `ng add <package>`            |

**Examples:**

```bash
ng new ecommerce-app --routing --style=scss
ng add @angular/material
```

---

## 🚀 2. Development Server

**Description:** Commands to run and manage the development environment.

| Description                   | Commands                              |
| ----------------------------- | ------------------------------------- |
| Start development server      | `ng serve`                            |
| Start server on specific port | `ng serve --port 4201`                |
| Open app in browser           | `ng serve --open`                     |
| Enable live reload            | `ng serve --live-reload`              |
| Use environment configuration | `ng serve --configuration=production` |

**Examples:**

```bash
ng serve --open
ng serve --port 4500
```

---

## 🏗️ 3. Code Generation

**Description:** Commands to generate Angular building blocks.

| Description        | Commands                       |
| ------------------ | ------------------------------ |
| Generate component | `ng generate component <name>` |
| Generate module    | `ng generate module <name>`    |
| Generate service   | `ng generate service <name>`   |
| Generate directive | `ng generate directive <name>` |
| Generate pipe      | `ng generate pipe <name>`      |
| Generate guard     | `ng generate guard <name>`     |
| Generate interface | `ng generate interface <name>` |
| Generate enum      | `ng generate enum <name>`      |

**Short alias:** `ng g`

**Examples:**

```bash
ng g component shared/navbar
ng g service core/auth
```

---

## ⚙️ 4. Build & Deployment

**Description:** Commands to compile and prepare the application for deployment.

| Description                            | Commands                              |
| -------------------------------------- | ------------------------------------- |
| Build application                      | `ng build`                            |
| Build for production                   | `ng build --configuration=production` |
| Output build files to custom directory | `ng build --output-path=dist/custom`  |
| Watch mode build                       | `ng build --watch`                    |

**Examples:**

```bash
ng build --configuration=production
```

---

## 🧪 5. Testing

**Description:** Commands for running unit and end-to-end tests.

| Description                | Commands                |
| -------------------------- | ----------------------- |
| Run unit tests             | `ng test`               |
| Run tests in headless mode | `ng test --watch=false` |
| Run end-to-end tests       | `ng e2e`                |

**Examples:**

```bash
ng test --watch=false
```

---

## 🔍 6. Linting & Code Quality

**Description:** Commands to analyze and maintain code quality.

| Description                   | Commands        |
| ----------------------------- | --------------- |
| Run linting                   | `ng lint`       |
| Fix lint issues automatically | `ng lint --fix` |

---

## 🛠️ 7. Utilities & Workspace Management

**Description:** Miscellaneous commands for maintaining and managing Angular workspace.

| Description                 | Commands                    |
| --------------------------- | --------------------------- |
| Show help                   | `ng help`                   |
| Update Angular dependencies | `ng update`                 |
| Add library/package         | `ng add <package>`          |
| Remove package              | `ng remove <package>`       |
| Run custom builder          | `ng run <project>:<target>` |
| Show project configuration  | `ng config`                 |

**Examples:**

```bash
ng update @angular/core @angular/cli
ng run my-app:build
```

---

# 📘 Referencia de Comandos Angular CLI

Referencia estructurada y práctica de los comandos más utilizados de Angular CLI, organizados por flujo de trabajo.

---

## 📦 1. Configuración del Proyecto

**Descripción:** Comandos para instalar Angular CLI y crear nuevos proyectos.

| Descripción                                   | Comandos                      |
| --------------------------------------------- | ----------------------------- |
| Instalar Angular CLI globalmente              | `npm install -g @angular/cli` |
| Verificar versión de Angular CLI              | `ng version`                  |
| Crear un nuevo proyecto Angular               | `ng new my-app`               |
| Crear proyecto con routing                    | `ng new my-app --routing`     |
| Crear proyecto con estilo específico          | `ng new my-app --style=scss`  |
| Agregar funcionalidades (PWA, Material, etc.) | `ng add <package>`            |

**Ejemplos:**

```bash
ng new ecommerce-app --routing --style=scss
ng add @angular/material
```

---

## 🚀 2. Servidor de Desarrollo

**Descripción:** Comandos para ejecutar y gestionar el entorno de desarrollo.

| Descripción                           | Comandos                              |
| ------------------------------------- | ------------------------------------- |
| Iniciar servidor de desarrollo        | `ng serve`                            |
| Iniciar servidor en puerto específico | `ng serve --port 4201`                |
| Abrir aplicación en navegador         | `ng serve --open`                     |
| Habilitar recarga en vivo             | `ng serve --live-reload`              |
| Usar configuración específica         | `ng serve --configuration=production` |

**Ejemplos:**

```bash
ng serve --open
ng serve --port 4500
```

---

## 🏗️ 3. Generación de Código

**Descripción:** Comandos para generar bloques de construcción de Angular.

| Descripción        | Comandos                       |
| ------------------ | ------------------------------ |
| Generar componente | `ng generate component <name>` |
| Generar módulo     | `ng generate module <name>`    |
| Generar servicio   | `ng generate service <name>`   |
| Generar directiva  | `ng generate directive <name>` |
| Generar pipe       | `ng generate pipe <name>`      |
| Generar guard      | `ng generate guard <name>`     |
| Generar interfaz   | `ng generate interface <name>` |
| Generar enum       | `ng generate enum <name>`      |

**Alias corto:** `ng g`

**Ejemplos:**

```bash
ng g component shared/navbar
ng g service core/auth
```

---

## ⚙️ 4. Build y Despliegue

**Descripción:** Comandos para compilar y preparar la aplicación para producción.

| Descripción                  | Comandos                              |
| ---------------------------- | ------------------------------------- |
| Compilar aplicación          | `ng build`                            |
| Compilar para producción     | `ng build --configuration=production` |
| Definir directorio de salida | `ng build --output-path=dist/custom`  |
| Build en modo watch          | `ng build --watch`                    |

**Ejemplos:**

```bash
ng build --configuration=production
```

---

## 🧪 5. Testing

**Descripción:** Comandos para ejecutar pruebas unitarias y end-to-end.

| Descripción                 | Comandos                |
| --------------------------- | ----------------------- |
| Ejecutar pruebas unitarias  | `ng test`               |
| Ejecutar tests sin watch    | `ng test --watch=false` |
| Ejecutar pruebas end-to-end | `ng e2e`                |

**Ejemplos:**

```bash
ng test --watch=false
```

---

## 🔍 6. Linting y Calidad de Código

**Descripción:** Comandos para analizar y mantener la calidad del código.

| Descripción                        | Comandos        |
| ---------------------------------- | --------------- |
| Ejecutar linting                   | `ng lint`       |
| Corregir problemas automáticamente | `ng lint --fix` |

---

## 🛠️ 7. Utilidades y Gestión del Workspace

**Descripción:** Comandos adicionales para gestionar el workspace de Angular.

| Descripción                    | Comandos                    |
| ------------------------------ | --------------------------- |
| Mostrar ayuda                  | `ng help`                   |
| Actualizar dependencias        | `ng update`                 |
| Agregar librería               | `ng add <package>`          |
| Eliminar librería              | `ng remove <package>`       |
| Ejecutar tarea personalizada   | `ng run <project>:<target>` |
| Ver configuración del proyecto | `ng config`                 |

**Ejemplos:**

```bash
ng update @angular/core @angular/cli
ng run my-app:build
```

---
