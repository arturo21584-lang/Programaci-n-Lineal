# Libro interactivo de Programación Lineal — EM-4010

Proyecto base de **Quarto Book**, con identidad editorial geométrica, navegación HTML, área de exploraciones y biblioteca de recursos.

## Requisitos de publicación

- Repositorio **público** de GitHub.
- Rama principal llamada `main`.
- GitHub Pages configurado en `Settings → Pages → Build and deployment → Deploy from a branch` con la rama `gh-pages` y carpeta `/ (root)` (la rama aparecerá después de una publicación exitosa).
- GitHub Actions con permiso `Read and write permissions` para el GITHUB_TOKEN en `Settings → Actions → General → Workflow permissions` si el repositorio no permite escritura por defecto.

## Puesta en marcha sin instalar Quarto

1. Crear un repositorio público vacío en GitHub, preferiblemente llamado `libro-programacion-lineal`.
2. Extraer este ZIP en una carpeta; **no subir el ZIP sin extraer**.
3. Subir los archivos y carpetas al repositorio conservando rutas, incluidos `.github/workflows/publicar.yml` y `_quarto.yml`. Si GitHub Web no deja subir bien una estructura, se puede usar el editor `github.dev` para crear rutas y pegar contenidos.
4. Confirmar los archivos con un commit en `main`.
5. Revisar la pestaña `Actions` y comprobar que el flujo «Publicar libro Quarto» termine correctamente.
6. Activar GitHub Pages desde la rama `gh-pages` y carpeta raíz. El sitio será `https://USUARIO.github.io/NOMBRE-REPOSITORIO/`.
7. Editar contenido en `github.dev` y confirmar cambios; cada commit desencadena una nueva compilación automática.

**Advertencia:** esta versión aún no ha sido compilada en el servicio de GitHub, por lo que deben comprobarse los resultados del primer flujo de trabajo y ajustar cualquier configuración que resulte necesaria.

## Estructura

- `_quarto.yml`: configuración del libro.
- `index.qmd`: portada.
- `capitulos/*.qmd`: estructura académica preliminar.
- `exploraciones.qmd`: directorio de experiencias interactivas.
- `recursos/index.qmd`: biblioteca de recursos.
- `bibliografia/referencias.bib`: bibliografía **vacía por diseño**.
- `bibliografia/registro-fuentes.csv`: trazabilidad.
- `estilos/editorial.css`: identidad gráfica.
- `.github/workflows/publicar.yml`: publicación automática.

## Principio de integridad académica

No copiar texto ajeno ni inventar teoremas, referencias, páginas o datos bibliográficos. Cada capítulo se aprobará tras contrastar materiales reales, verificar la matemática, diseñar la interactividad y revisar derechos de autor.
