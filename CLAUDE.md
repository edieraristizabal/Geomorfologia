# CLAUDE.md

Guía para Claude Code (y para cualquier persona) que actualice este repositorio. **Cada cambio que se haga en el repositorio debe registrarse al final, en "Registro de cambios".**

## Qué es

Curso **Geomorfología** (Universidad Nacional de Colombia, sede Medellín, Prof. Edier Aristizábal). Un solo repositorio contiene tres productos:

| Producto | Fuente en `master` | URL publicada |
|---|---|---|
| Página del curso (Jekyll, tema minimal) | `index.md`, `_config.yml`, programa en PDF | https://edieraristizabal.github.io/Geomorfologia/ |
| Diapositivas (Reveal.js) | `html/Geomorfologia.html` y sus recursos en `html/` | https://edieraristizabal.github.io/Geomorfologia/html/Geomorfologia.html |
| Libro (Jupyter Book 1.x) | `libro/` | https://edieraristizabal.github.io/Geomorfologia/libro/ |

Remoto: https://github.com/edieraristizabal/Geomorfologia

## Resumen del contenido

El curso de **Geomorfología** está orientado para estudiantes de semestres intermedios de Ingeniería Geológica e Ingeniería Ambiental que deseen adquirir conocimientos sobre los procesos endógenos y exógenos que modelan las geoformas de la superficie terrestre. Luego de una introducción a la geomorfología donde se estudia la historia, los modelos de evolución y las técnicas que existen dentro de la geomorfología, el curso se estructura en tres grandes bloques:

El libro (Geomorfología Aplicada) está escrito en MyST Markdown, sin código ejecutable; las figuras están en `libro/images/` y las referencias en `libro/references.bib`.

Contenido del libro (orden de `libro/_toc.yml`; el título es el primer encabezado de cada archivo):

- `intro`: GEOMORFOLOGÍA EN AMBIENTES TROPICALES

**Parte I: Fundamentos de Geomorfología**

- `conceptos`: Conceptos fundamentales en Geomorfología
- `evolucion`: Teorías Clásicas de la Evolución de Laderas

**Parte II: Procesos Endógenos**

- `morfotectonica`: Morfotectónica y geomorfología estructural
- `volcanico`: Geomorfología de Ambientes Volcánicos

**Parte III: Procesos Exógenos**

- `glacial`: Geomorfología Glacial y Periglacial
- `meteorizacion`: Meteorización: procesos, perfiles y geoformas
- `MenM`: Geomorfología de Movimientos en Masa
- `pluvial`: Erosión Pluvial
- `eolica`: Erosión Eólica
- `cuencas`: Geomorfología de Cuencas Hidrográficas
- `torrencial`: Ambientes Torrenciales
- `aluvial`: Geomorfología de Ambientes Fluviales
- `delta`: Geomorfología de Ambientes Deltaicos

**Referencias**

- `referencias`: Referencias

## Ramas: dónde hacer pull y push

**Siempre se trabaja en `master`.** Ese es el único lugar donde se edita, se hace `git pull` y `git push`, tanto para cambios de la página como de las diapositivas o del libro.

**Nunca editar ni hacer push a `gh-pages` a mano.** Esa rama la genera el workflow `.github/workflows/deploy.yml` en cada push a `master`: construye Jekyll en `_site/`, construye el libro y lo copia en `_site/libro/`, y publica todo en `gh-pages` con `force_orphan` (cualquier cambio manual en `gh-pages` se pierde en el siguiente despliegue).

GitHub Pages sirve un solo sitio por repositorio; por eso la página y el libro se combinan en el Action. En **Settings → Pages** la fuente debe ser *Deploy from a branch*, rama `gh-pages`, carpeta `/ (root)`.

Flujo normal:

```bash
git pull origin master
# ... editar ...
# ... agregar una línea al Registro de cambios de este archivo ...
git add -A
git commit -m "Descripción del cambio"
git push origin master      # el Action publica en 2 a 5 minutos (pestaña Actions)
```

## Estructura

```
.github/
    workflows/
.gitignore
CLAUDE.md
Documentos/
    aluvial_tmp.html
    glacial_tmp.html
    meteorizacion_tmp.html
    morfotectonica_tmp.html
    pluvial_tmp.html
Programa_GEOMORFOLOGIA.pdf
Programa_GEOMORFOLOGIA.tex
README.md
TrabajosIndividuales/
_config.yml
_layouts/
    default.html
html/
    .github/
    Geomorfologia.backup-2026-10-05.html
    Geomorfologia.backup-2026-10-05b.html
    Geomorfologia.html
index.md
libro/
trabajoGrupo/
    Taller_morfometria/
```

Material fuente que **no** se sube (libros guía, presentaciones originales, documentos con derechos): está en `C:\Users\edier\Documents\CATEDRA\GEOMORFOLOGIA`, fuera de este repositorio.

## Cómo actualizar

**Página del curso.** Editar `index.md`. Los enlaces internos deben ser relativos (`Programa.pdf`, `html/...`), nunca empezar por `/`, porque el sitio vive en `/Geomorfologia/`. El libro se enlaza como `https://edieraristizabal.github.io/Geomorfologia/libro/<capítulo>.html`. Si cambia la evaluación, actualizarla también en el programa (`.tex` + PDF) y en las diapositivas.

**Diapositivas.** Editar `html/Geomorfologia.html` directamente (Reveal.js; ecuaciones con MathJax). Previsualizar con `python -m http.server` desde la raíz y abrir `http://localhost:8000/html/Geomorfologia.html`.

**Libro.** Capítulos en MyST Markdown (`.md`) o notebooks (`.ipynb`) dentro de `libro/`; un capítulo nuevo debe agregarse a `libro/_toc.yml`; las citas `{cite:t}` / `{cite:p}` deben existir en el archivo `.bib` del libro.

- **El Action no ejecuta los notebooks** (`execute_notebooks: "off"`): publica las salidas guardadas en cada `.ipynb`. Si se cambia código, ejecutar el notebook localmente y guardarlo con sus salidas antes del commit.
- `libro/requirements.txt` contiene solo lo necesario para construir el libro; `libro/requirements-notebooks.txt` (si existe) lista las librerías para ejecutar los notebooks.
- Si git falla con `bad object refs/desktop.ini` o `failed to perform geometric repack`, es porque Windows/Google Drive creó archivos `desktop.ini` dentro de `.git/`: borrarlos con `find .git -name desktop.ini -delete` y repetir el comando.
- Compilar localmente: `C:\Users\edier\.jbenv\Scripts\jupyter-book.exe build libro` y abrir `libro/_build/html/index.html`.



## Preferencias del autor

- Proponer los cambios de contenido del curso y esperar aprobación antes de editarlos.
- Prosa en párrafos, español, sin rayas (em dash): usar comas o paréntesis.
- Las figuras nuevas se buscan primero en los tableros de Pinterest del autor.

## Pendientes conocidos

- Cambiar en Settings → Pages la fuente a la rama `gh-pages` (hasta entonces sigue publicando la rama `master` sin el libro nuevo).
- Borrar el repositorio viejo `Libro_Geomorfologia` en GitHub una vez verificado que https://edieraristizabal.github.io/Geomorfologia/libro/ funciona.
- `html/` contiene dos respaldos de la presentación (`Geomorfologia.backup-2026-10-05*.html`) que podrían eliminarse.

## Registro de cambios

Cada cambio al repositorio se anota aquí, el más reciente primero, con el formato `- **AAAA-MM-DD**: qué se cambió y por qué (archivos principales).` Esta sección es la memoria del curso entre sesiones: leerla antes de empezar a trabajar.

- **2026-10-25**: Tres figuras de ResearchGate de `html/Geomorfologia.html` movidas a Pinterest (tablero geomorfologia): dos recuperadas del Internet Archive (pseudokarst en El Hierro, evolución de cerros residuales) y una reemplazada por una figura nueva de factores condicionantes y detonantes (`html/img/figuras/geomorf_factores_condicionantes.png`), porque ResearchGate dejó de servirla. Quedan 16 figuras de ResearchGate que hoy cargan pero pueden fallar; no tienen copia en el Internet Archive.
- **2026-10-25**: Revisión de figuras de la presentación en el navegador; se reemplazaron 12 imágenes rotas de html/Geomorfologia.html: 9 recuperadas del Internet Archive y fijadas en el tablero geomorfologia de Pinterest, la cárcava con un pin existente del mismo tablero, y dos figuras nuevas generadas con matplotlib (respuesta hidrológica de la cuenca y carst hipogénico, este último con el atributo src mal escrito, sin comilla inicial). Las figuras generadas quedan también en `html/img/figuras/`; la presentación las enlaza desde `i.pinimg.com`.
- **2026-10-25**: `README.md` con la sección "Enlaces del curso" (página, presentación y libro publicados) y el enlace a la página personal https://edieraristizabal.github.io/.
- **2026-10-24**: Interfaz en español: `_layouts/default.html` traducido ("Ver el proyecto en GitHub", "Este proyecto es mantenido por", `lang` = es), reemplaza el texto en inglés del tema minimal de Jekyll; `language: es` en `libro/_config.yml` para que la interfaz del libro (búsqueda, navegación) quede en español.
- **2026-10-24**: Revisión de idioma: se tradujeron al español 7 bloques en inglés de `html/Geomorfologia.html` (penillanura y pediplanicie, georreferenciación, meseta, ciclos de Milankovitch, coluvión). Se mantienen en inglés los títulos de lecturas, los enlaces externos y los tweets incrustados (los reemplaza la publicación original al cargar).
- **2026-10-24**: CLAUDE.md ampliado con resumen del contenido, pendientes y este registro de cambios.
- **2026-10-24**: Unificación en un solo repositorio: el libro (antes repositorio `Libro_Geomorfologia`) se copió a `libro/` con `execute_notebooks: off`, `baseurl` y enlaces al repositorio nuevo; se agregó `.github/workflows/deploy.yml` (Jekyll + Jupyter Book → `gh-pages`); `_config.yml` con `url`/`baseurl: /Geomorfologia` y exclusiones; en `index.md` los enlaces absolutos (`/...`) pasaron a relativos y el enlace al libro apunta a `/Geomorfologia/libro/`.
- **2026-10-24**: Commit de respaldo de los cambios locales pendientes antes de unificar (38 archivos modificados) y limpieza de archivos `desktop.ini` dentro de `.git/` que impedían el mantenimiento de git.
