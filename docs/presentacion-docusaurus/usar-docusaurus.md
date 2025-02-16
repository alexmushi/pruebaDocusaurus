---
title: Cómo Utilizar Docusaurus
sidebar_label: Cómo Utilizar Docusaurus
slug: /guia-docusaurus
---

# 📌 Cómo Utilizar Docusaurus

Docusaurus es una herramienta que podemos utilizar para la documentación, pues tiene control de versiones y una barra de búsqueda global. Usarlo es tan simple como hacer commits a un repo con carpetas y archivos de Markdown.

## Flujo de Trabajo Básico

1.  Lo normal de github, ya se la saben

    *   **Clonar el Repositorio:**
        ```bash
        git clone https://github.com/alexmushi/pruebaDocusaurus.git
        cd pruebaDocusaurus
        ```

    *   **Crear una branch:**  Probablemente será buena idea crear nuevas branches cada vez que se agregue algo nuevo (substancial), para que haya alguien que cree el documento y alguien que lo revise
        ```bash
        git checkout -b mi-nueva-caracteristica
        ```

    *   **Escribir/Editar Documentación:**
        *   Los archivos de documentación están en la carpeta `docs`.
        *   Usa Markdown (`.md`) o MDX (`.mdx` es para agregar componentes de React).
        *   Los archivos están organizados en carpetas, podemos definir una estructura desde el inicio
        *  Se pueden editar en cualquier IDE, o incluso pueden hacer primero el documento en word si no les gusta el MD y le piden a chat que lo traduzca

    *   **Ver los Cambios Localmente:**
        ```bash
        npm start  
        ```
        Esto inicia un servidor de desarrollo local (normalmente en `http://localhost:3000`).  Verás los cambios en tiempo real mientras editas.

    *   **Añadir, Confirmar y Subir Cambios:**
        ```bash
        git add -A
        git commit -m "Una descripción clara de mis cambios"
        git push origin mi-nueva-caracteristica
        ```

    *   **Crear un Pull Request (PR):**
        *   Crea un Pull Request desde tu rama (`mi-nueva-caracteristica`) hacia la rama principal (`main` o `master`).
        *   Describe los cambios en el PR.  *Sé detallado*.
        *   Solicita revisiones a otros miembros del equipo


    *   **Merge:**
        *   Una vez que el PR sea aprobado, un administrador (o tú, si tienes permisos) lo fusionará con la rama principal.

    *   **Deploy:**
        *   Esto queda pendiente... hasta ahorita hemos usado 
        ```bash
        GIT_USER=(tu_usuario) yarn deploy
        ```
        pero como queremos hacerlo lo más sencillo posible, vamos a automatizarlo para que cada que se apruebe un PR se actualice la página

