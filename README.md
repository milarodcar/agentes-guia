# Guías de uso para Draxton

Manuales web, en español, para los usuarios de Draxton. Son páginas estáticas: no necesitan servidor ni instalación.

| Guía | Contenido | Dirección |
| --- | --- | --- |
| Portada | Página de inicio con las dos guías | https://milarodcar.github.io/agentes-guia/ |
| DraxBot | Cómo usar DraxBot, el agente de documentación: acceso, preguntas, respuestas e informes de inteligencia | https://milarodcar.github.io/agentes-guia/draxbot/ |
| BI Comercial con Claude | Cómo configurar Claude Desktop para consultar el informe de Power BI «BI Comercial» | https://milarodcar.github.io/agentes-guia/bi-comercial/ |

Las dos guías tienen arriba un selector **Guías** para pasar de una a otra; la palabra «Guías» lleva a la portada.

## Contenido del proyecto

| Archivo | Para qué sirve |
| --- | --- |
| `index.html` | Portada con las dos guías |
| `draxbot/index.html` | Guía de DraxBot (HTML, CSS y JavaScript en un solo archivo) |
| `img/` | Capturas de pantalla de la guía de DraxBot |
| `bi-comercial/index.html` | Guía de BI Comercial con Claude (copia de la guía de Inkoova, con las imágenes incluidas en el archivo) |
| `.nojekyll` | Indica a GitHub Pages que publique los archivos tal cual |
| `README.md` | Este archivo |

## Ver las guías en local

Abre `index.html` con doble clic: se abre la portada en el navegador y desde ahí se llega a cada guía.

## Publicar en GitHub Pages

1. En GitHub, crea un repositorio nuevo, por ejemplo `agentes-guia`.
   Con una cuenta gratuita, GitHub Pages solo publica repositorios **públicos**.
2. Sube el contenido de esta carpeta (`index.html`, las carpetas `draxbot`, `img` y `bi-comercial`, `.nojekyll` y `README.md`):
   - **Desde la web:** en el repositorio, pulsa **Add file → Upload files**, arrastra los archivos y pulsa **Commit changes**.
   - **Con Git**, desde esta carpeta:

     ```bash
     git init
     git add .
     git commit -m "Guías de uso para Draxton"
     git branch -M main
     git remote add origin https://github.com/<tu-usuario>/agentes-guia.git
     git push -u origin main
     ```

3. En el repositorio, ve a **Settings → Pages**.
4. En **Build and deployment**, elige **Source: Deploy from a branch**, rama **main** y carpeta **/ (root)**. Pulsa **Save**.
5. En uno o dos minutos la guía estará disponible en:
   `https://<tu-usuario>.github.io/agentes-guia/`

## Actualizar la guía

Edita el `index.html` de la guía (`draxbot/` o `bi-comercial/`), o sustituye una imagen en `img/` manteniendo el mismo nombre, y sube los cambios al repositorio. GitHub Pages publica la nueva versión automáticamente.
