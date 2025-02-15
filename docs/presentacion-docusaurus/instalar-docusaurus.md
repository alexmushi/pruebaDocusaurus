---
title: Instalación de Docusaurus
sidebar_label: Instalación
slug: /instalacion-docusaurus
---

# 📌 Instalación de la documentación con Docusaurus

Docusaurus es un framework de documentación basado en React. Sigue estos pasos para instalarlo y configurarlo en tu proyecto.

## 🔹 Requisitos previos
Antes de usar Docusaurus, asegúrate de tener:
- [Node.js](https://nodejs.org/) v16 o superior
- [Yarn](https://yarnpkg.com/)

## 🚀 Instalación de yarn
Para instalar Docusaurus, ejecuta el siguiente comando en tu terminal de git:


### Usando `npm`
```bash
npm install --global yarn
```
### Debes de ver el mensaje de:
```bash
up to date, audited 766 packages in 3s

94 packages are looking for funding
  run `npm fund` for details

5 vulnerabilities (2 moderate, 2 high, 1 critical)

To address all issues, run:
  npm audit fix

Run `npm audit` for details.
```

### Corrobora que se haya instalado con:
```bash
yarn --version
```

## 🔧 Construcción y despliegue
Para construir por primera vez el proyecto:
```bash
GIT_USER=tu_usuario yarn deploy
```

## 🎯 Ejecutar el servidor local
Después de la instalación, en tu terminal escribe:
```bash
npm start
```

Docusaurus estará disponible en [`http://localhost:3000`](http://localhost:3000) 🚀.
 
## 🔧Actualizar la documentación.
Dentro de la carpeta docs puedes. Aquí van archivos .md o .mdx los cuales deberían de ser apartados de la documentación y en la carpeta. Las actualizaciones se hacen con commits.

### Añadir todos los archivos:
```bash
git add -A
```

### Comprometer la transacción:
```bash
git commit -m "Esto es un mensaje ejemplo"
```

### Enviar la transacción :
```bash
git push
```

### Hacer el deploy de tus cambios :
```bash
GIT_USER=tu_usuario yarn deploy
```

## ✅ Conclusión
¡Ahora tienes Docusaurus instalado y corriendo! 🎉 Puedes empezar a personalizar tu documentación modificando los archivos en `docs/`.
