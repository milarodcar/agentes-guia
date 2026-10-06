# Guías de uso para Draxton

Manuales web, en español, para los usuarios de Draxton. Son páginas estáticas: no necesitan servidor ni instalación.

| Guía | Contenido | Dirección |
| --- | --- | --- |
| DraxBot | Cómo usar DraxBot, el agente de documentación: acceso, preguntas, respuestas e informes de inteligencia | https://milarodcar.github.io/draxbot-guia-web/ |
| Proyección Comercial con Claude | Cómo configurar Claude Desktop para consultar el informe de Power BI «Proyección Comercial» | https://milarodcar.github.io/draxbot-guia-web/proyeccion-comercial/ |

Las dos páginas tienen arriba un selector **Guías** para pasar de una a otra.

## Contenido del proyecto

| Archivo | Para qué sirve |
| --- | --- |
| `index.html` | Guía de DraxBot (HTML, CSS y JavaScript en un solo archivo) |
| `img/` | Capturas de pantalla de la guía de DraxBot |
| `proyeccion-comercial/index.html` | Guía de Proyección Comercial con Claude (copia de la guía de Inkoova, con las imágenes incluidas en el archivo) |
| `.nojekyll` | Indica a GitHub Pages que publique los archivos tal cual |
| `README.md` | Este archivo |

## Ver las guías en local

Abre `index.html` (o `proyeccion-comercial/index.html`) con doble clic. Se abre en el navegador.

## Publicar en GitHub Pages

1. En GitHub, crea un repositorio nuevo, por ejemplo `draxbot-guia-web`.
   Con una cuenta gratuita, GitHub Pages solo publica repositorios **públicos**.
2. Sube el contenido de esta carpeta (`index.html`, la carpeta `img`, `.nojekyll` y `README.md`):
   - **Desde la web:** en el repositorio, pulsa **Add file → Upload files**, arrastra los archivos y pulsa **Commit changes**.
   - **Con Git**, desde esta carpeta:

     ```bash
     git init
     git add .
     git commit -m "Guía de uso de DraxBot"
     git branch -M main
     git remote add origin https://github.com/<tu-usuario>/draxbot-guia-web.git
     git push -u origin main
     ```

3. En el repositorio, ve a **Settings → Pages**.
4. En **Build and deployment**, elige **Source: Deploy from a branch**, rama **main** y carpeta **/ (root)**. Pulsa **Save**.
5. En uno o dos minutos la guía estará disponible en:
   `https://<tu-usuario>.github.io/draxbot-guia-web/`

## Actualizar la guía

Edita `index.html` (o sustituye una imagen en `img/` manteniendo el mismo nombre) y sube los cambios al repositorio. GitHub Pages publica la nueva versión automáticamente.
