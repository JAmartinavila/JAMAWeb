# JAMAWeb — Personal academic website

Web personal de **Jorge A. Martín-Ávila**, desarrollada en **Quarto** y publicada mediante GitHub Pages.

- Web pública: https://jamartinavila.github.io/JAMAWeb/
- Repositorio: https://github.com/JAmartinavila/JAMAWeb

## Renovación (noviembre de 2026)

Esta carpeta es una **copia completa y limpia del código fuente** que has facilitado. No incluye `.git/` (historial de Git), `_site/` (HTML generado), `.quarto/` (caché) ni `.Rproj.user/` (archivos locales temporales). La rama `main` de tu repositorio existente conserva el historial, mientras que el código de este ZIP se puede incorporar a una nueva rama.

Cambios realizados:

1. Nueva portada (`index.qmd`) con fotografía original, líneas de investigación y artículos destacados.
2. Nuevo estilo responsive (`styles.css`) con identidad visual verde bosque y tipografía editorial.
3. Nueva página `About.qmd` con trayectoria, formación, competencias y contacto.
4. Publicaciones actualizadas (`Publications.qmd`), con enlaces DOI a trabajos verificados.
5. Nuevo proyecto `projects/honey-buzzard.qmd`, y mantenimiento de proyectos previos y blog.
6. Enlaces de SEO y navegación corregidos en `_quarto.yml`.
7. Conserva `.github/workflows/publish.yml` para la publicación automática en GitHub Pages.

**Contenido preservado:** fotografía `Jorge.jpeg`, proyectos originales, fotografías y artículo sobre el cárabo, herramientas R, extensión iconify y workflow de publicación. El `.Rproj` pasa a llamarse `JAMAWeb.Rproj`.

## Cómo verlo antes de publicar

1. Abre la carpeta `JAMAWeb` en RStudio / VS Code con Quarto instalado.
2. Abre una terminal en la raíz de `JAMAWeb` y ejecuta `quarto preview`.
3. Revisa la versión para escritorio y móvil. `quarto render` genera el sitio en `_site/`.
4. Alternativamente, abre el archivo separado `JAMAWeb_vista_previa.html` de esta entrega: es **solo una maqueta** de la portada, no el render oficial de Quarto.

## Cómo sustituir tu web en GitHub sin perder el historial

La manera más segura es crear una rama nueva desde el repo actual:

```bash
git clone https://github.com/JAmartinavila/JAMAWeb.git
cd JAMAWeb
git switch -c renovacion-web
```

Sustituye en esta carpeta clonada los archivos por el contenido de este ZIP (sin borrar `.git`), incluidos nuevos `About.qmd` y `projects/honey-buzzard.qmd`. Luego:

```bash
git add -A
git commit -m "Renovar web personal académica"
git push -u origin renovacion-web
```

Revisa la rama y abre un *pull request* hacia `main`; al integrarla, el workflow original de GitHub Actions publicará en `gh-pages` si las opciones de Pages ya están bien configuradas (Settings > Pages > Deploy from a branch: `gh-pages` / root).

## Edición habitual

- Presentación y portada: `index.qmd`
- Proyectos: añadir un archivo `.qmd` en `projects/`
- Publicaciones: `Publications.qmd`
- Perfil y trayectoria: `About.qmd`
- Blog: añadir un `.qmd` en `posts/`
- Menú, redes y ajustes generales: `_quarto.yml`
- Estilos visuales: `styles.css`

## Cosas por validar personalmente

- Dirección de email institucional (se ha conservado la que tenías en el repositorio).
- Texto de experiencia laboral actual y cualquier matiz del perfil que quieras ajustar.
- La referencia bibliográfica completa del trabajo de *Animal Behaviour* aceptado en 2026; por ahora figura como manuscrito en prensa y **no se ha inventado DOI**.
- Añadir el CV en PDF cuando lo tengas definitivo (se ha evitado crear un enlace a un archivo inexistente).
- Revisar y actualizar tus publicaciones futuras en cuanto salgan.

## Validación técnica

Se comprobó el contenido fuente, los enlaces internos y la sintaxis YAML. **No se ha ejecutado Quarto render en este entorno porque el ejecutable de Quarto no está instalado**; validar el resultado real mediante `quarto preview` o GitHub Actions antes de fusionar a `main`.
