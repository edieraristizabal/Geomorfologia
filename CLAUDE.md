# CLAUDE.md

Guía para Claude Code (y para cualquier persona) que actualice este repositorio.

## Qué es

Curso **Geomorfología** (Universidad Nacional de Colombia, sede Medellín, Prof. Edier Aristizábal). Un solo repositorio contiene tres productos:

| Producto | Fuente en `master` | URL publicada |
|---|---|---|
| Página del curso (Jekyll, tema minimal) | `index.md`, `_config.yml`, programa en PDF | https://edieraristizabal.github.io/Geomorfologia/ |
| Diapositivas (Reveal.js) | `html/Geomorfologia.html` y sus recursos en `html/` | https://edieraristizabal.github.io/Geomorfologia/html/Geomorfologia.html |
| Libro (Jupyter Book 1.x) | `libro/` | https://edieraristizabal.github.io/Geomorfologia/libro/ |

Remoto: https://github.com/edieraristizabal/Geomorfologia

## Ramas: dónde hacer pull y push

**Siempre se trabaja en `master`.** Ese es el único lugar donde se edita, se hace `git pull` y `git push`, tanto para cambios de la página como de las diapositivas o del libro.

**Nunca editar ni hacer push a `gh-pages` a mano.** Esa rama la genera el workflow `.github/workflows/deploy.yml` en cada push a `master`: construye Jekyll en `_site/`, construye el libro y lo copia en `_site/libro/`, y publica todo en `gh-pages` con `force_orphan` (cualquier cambio manual en `gh-pages` se pierde en el siguiente despliegue).

GitHub Pages sirve un solo sitio por repositorio; por eso la página y el libro se combinan en el Action. En **Settings → Pages** la fuente debe ser *Deploy from a branch*, rama `gh-pages`, carpeta `/ (root)`.

Flujo normal:

```bash
git pull origin master
# ... editar ...
git add -A
git commit -m "Descripción del cambio"
git push origin master      # el Action publica en 2 a 5 minutos (pestaña Actions)
```

## Estructura

```
.github/
    workflows/
.gitignore
Documentos/
Programa_GEOMORFOLOGIA.aux
Programa_GEOMORFOLOGIA.log
Programa_GEOMORFOLOGIA.pdf
Programa_GEOMORFOLOGIA.synctex.gz.properties
Programa_GEOMORFOLOGIA.tex
README.md
TrabajosIndividuales/
_config.yml
html/
    .github/
    css/
    examples/
    js/
    test/
index.md
libro/
trabajoGrupo/
    Taller_morfometria/
```

Capítulos del libro (`libro/`, orden en `libro/_toc.yml`): MenM.md, aluvial.md, conceptos.md, cuencas.md, delta.md, eolica.md, evolucion.md, glacial.md, intro.md, meteorizacion.md, morfotectonica.md, pluvial.md, referencias.md, torrencial.md, volcanico.md.

El libro proviene del antiguo repositorio Libro_Geomorfologia (unificado aquí en octubre de 2026); sus capítulos son MyST Markdown sin código ejecutable.

Material fuente que **no** se sube (libros guía, presentaciones originales, documentos con derechos): está en `C:\Users\edier\Documents\CATEDRA\GEOMORFOLOGIA`, fuera de este repositorio.

## Cómo actualizar

**Página del curso.** Editar `index.md`. Los enlaces internos deben ser relativos (`Programa.pdf`, `html/...`), nunca empezar por `/`, porque el sitio vive en `/Geomorfologia/`. El libro se enlaza como `https://edieraristizabal.github.io/Geomorfologia/libro/<capítulo>.html`.

**Diapositivas.** Editar `html/Geomorfologia.html` directamente (Reveal.js; ecuaciones con MathJax). Previsualizar con `python -m http.server` desde la raíz y abrir `http://localhost:8000/html/Geomorfologia.html`.

**Libro.** Capítulos en MyST Markdown (`.md`) o notebooks (`.ipynb`) dentro de `libro/`; un capítulo nuevo debe agregarse a `libro/_toc.yml`; las citas `{cite:t}` / `{cite:p}` deben existir en el archivo `.bib` del libro.

- **El Action no ejecuta los notebooks** (`execute_notebooks: "off"`): publica las salidas guardadas en cada `.ipynb`. Si se cambia código, ejecutar el notebook localmente y guardarlo con sus salidas antes del commit.
- `libro/requirements.txt` contiene solo lo necesario para construir el libro; `libro/requirements-notebooks.txt` (si existe) lista las librerías para ejecutar los notebooks.
- Compilar localmente: `C:\Users\edier\.jbenv\Scripts\jupyter-book.exe build libro` y abrir `libro/_build/html/index.html`.



## Preferencias del autor

- Proponer los cambios de contenido del curso y esperar aprobación antes de editarlos.
- Prosa en párrafos, español, sin rayas (em dash): usar comas o paréntesis.
- Las figuras nuevas se buscan primero en los tableros de Pinterest del autor.
