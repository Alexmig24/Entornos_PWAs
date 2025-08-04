# 🛠️ Boilerplate para PWAs con Entorno de Desarrollo Profesional

Este proyecto es una **plantilla inicial (boilerplate)** para construir aplicaciones web progresivas (PWA) de forma rápida, profesional y con herramientas de desarrollo automatizadas. Incluye todo lo necesario para comenzar de inmediato con una estructura clara, recarga en vivo, control de calidad de código y preparación para producción.

---

## Fase 1: Inicialización y Servidor de Desarrollo

### Tareas realizadas:

- Creación de estructura de archivos base (`src/`, `assets/`, `css/`, `js/`).
- Inicialización del proyecto con `npm init -y`.
- Instalación de `live-server` como dependencia de desarrollo:
  ```bash
  npm install --save-dev live-server
  ```
- Agregado del script para desarrollo en `package.json`:
  ```json
  "scripts": {
    "dev": "live-server"
  }
  ```

### Entregable:
Repositorio con estructura base y `package.json` funcional que permite iniciar el servidor de desarrollo con:
```bash
npm run dev
```

---

## Fase 2: Integración de Calidad de Código

### Tareas realizadas:

- Instalación de ESLint y Prettier:
  ```bash
  npm install --save-dev eslint prettier eslint-config-prettier
  ```

- Creación del archivo `.eslintrc.json` para configurar ESLint.
- Creación del archivo `.prettierrc` para configurar el estilo del código.
- Agregado de scripts para linting y formateo en `package.json`:
  ```json
  "scripts": {
    "lint": "eslint .",
    "format": "prettier --write ."
  }
  ```
---

## Fase 3: Documentación y Versión Final

### Tareas realizadas:

- Instalación de `http-server` para simular un entorno de producción:
  ```bash
  npm install --save-dev http-server
  ```

- Agregado del script de producción en `package.json`:
  ```json
  "scripts": {
    "serve": "http-server -c-1"
  }
  ```

  El flag `-c-1` es **esencial** para desactivar el caché del navegador y evitar conflictos con el Service Worker.

---

## Scripts disponibles

| Comando         | Descripción                                                       |
|-----------------|-------------------------------------------------------------------|
| `npm run dev`   | Inicia el servidor con recarga en vivo (live-server).            |
| `npm run lint`  | Revisa el código JavaScript con ESLint.                          |
| `npm run format`| Formatea todo el código (HTML/CSS/JS) con Prettier.              |
| `npm run serve` | Simula entorno de producción sin caché (http-server -c-1).       |

---

## Estructura del proyecto

```
📦 Entorno_PWAs/
 ┣ 📁 src/
 ┃ ┣ 📄 index.html
 ┃ ┣ 📁 assets/
 ┃ ┣ 📁 css/
 ┃ ┣ 📁 js/
 ┣ 📄 .eslintrc.json
 ┣ 📄 .prettierrc
 ┣ 📄 package.json
 ┣ 📄 manifest.json
 ┣ 📄 sw.js
 ┗ 📄 README.md
```

---
## Cómo comenzar

Sigue estos pasos para comenzar a trabajar con este proyecto:

### 1. Clona este repositorio

```bash
git clone https://github.com/Alexmig24/Entornos_PWAs.git
cd Entornos_PWAs
```

### 2. Instala las dependencias

```bash
npm install
```

### 3. Ejecuta el servidor de desarrollo

```bash
npm run dev
```

---

## Requisitos Previos

- Node.js y npm instalados. Puedes descargarlos desde: https://nodejs.org/

---

## Autor

Desarrollado por: Alexander Quizhpe

---