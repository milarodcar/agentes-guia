# Guía de uso de DraxBot

Manual web, en español, para los usuarios de **DraxBot**, el agente de documentación de Draxton. Explica cómo acceder, hacer preguntas, leer las respuestas y consultar los informes de inteligencia semanales y mensuales.

La guía es una página estática: no necesita servidor ni instalación.

## Contenido del proyecto

| Archivo | Para qué sirve |
| --- | --- |
| `index.html` | La guía completa (HTML, CSS y JavaScript en un solo archivo) |
| `img/` | Capturas de pantalla que aparecen en la guía |
| `.nojekyll` | Indica a GitHub Pages que publique los archivos tal cual |
| `README.md` | Este archivo |

## Ver la guía en local

Abre `index.html` con doble clic. Se abre en el navegador.

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
