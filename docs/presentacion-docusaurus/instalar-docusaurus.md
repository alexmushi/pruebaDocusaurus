---
title: Instalación de Docusaurus
sidebar_label: Instalación
slug: /instalacion-docusaurus
---

# 📌 Instalación de la documentación con Docusaurus

Docusaurus es un framework de documentación basado en React. Sigue estos pasos para instalarlo y configurarlo en tu ambiente de desarrollo.

## 💡 Requisitos previos
Antes de usar Docusaurus, asegúrate de tener:
- [Node.js](https://nodejs.org/) v16 o superior
- [Yarn](https://yarnpkg.com/)

## 🚀 Instalación de yarn
Para instalar Docusaurus, ejecuta los siguientes comando en **GitBash**:


### Usando `npm`
```bash
npm install --global yarn
```

Debes de ver el siguiente mensaje:

```bash
up to date, audited 766 packages in 3s

94 packages are looking for funding
  run `npm fund` for details

5 vulnerabilities (2 moderate, 2 high, 1 critical)

To address all issues, run:
  npm audit fix

Run `npm audit` for details.
```

Corrobora que se haya instalado con:

```bash
yarn --version
```

## 🔧 Construcción y despliegue
Para construir por primera vez el proyecto en tu ambiente, ejecuta el siguiente comando en **GitBash**:
```bash
GIT_USER=tu_usuario yarn deploy
```

## 🎯 Ejecución del servidor local
Después de la instalación, en tu **terminal** escribe:
```bash
npm start
```

Se van a desplegar varios mensajes. Al final, deberías ver:

```bash
> prueba-docusaurus@0.0.0 start
> docusaurus start

[INFO] Starting the development server...
[SUCCESS] Docusaurus website is running at: http://localhost:3000/pruebaDocusaurus/

√ Client
  Compiled successfully in 996.50ms

client (webpack 5.98.0) compiled successfully
```

Automáticamente se desplegará la página en tu navegador. 

### Páginas prueba
Docusaurus estará disponible en [`http://localhost:3000/pruebaDocusaurus`](http://localhost:3000/pruebaDocusaurus) 🚀.

Ahorita para acceder a las páginas prueba, debes seleccionar **Tutorial** en la barra de navegación.
 
## 🔧 Actualización de la documentación
Dentro de la carpeta docs puedes encontrar los archivos de las páginas **.md** o **.mdx**, los cuales deberían de ser apartados de la documentación y en la carpeta. Las actualizaciones se hacen con commits siguiendo los siguientes pasos.

### Añadir todos los archivos
```bash
git add -A
```

### Comprometer la transacción
```bash
git commit -m "Esto es un mensaje ejemplo"
```

### Enviar la transacción
```bash
git push
```

### Hacer el deploy de tus cambios
```bash
GIT_USER=tu_usuario yarn deploy
```

## ✅ Conclusión
¡Ahora tienes Docusaurus instalado y corriendo! 🎉 Puedes interactuar con la documentación modificando los archivos en `docs`.
