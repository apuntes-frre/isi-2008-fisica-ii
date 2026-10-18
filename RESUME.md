# Reanudación de Física II

## Estado

- Rama: `codex/transcribir-fisica-ii`, creada desde `origin/main` actualizado.
- Clon: `/Users/carlosferreyra/Development/apuntes-frre/isi-2008-fisica-ii`.
- Checkpoint 1 validado localmente: laboratorio 9 bis, versión PDF, 2 páginas.
- No fusionar a main. Publicación autorizada como PR borrador.
- README raíz autogenerado: no modificar.

## Fuentes y salidas recuperables

- Canónica:
  `/Users/carlosferreyra/Library/CloudStorage/OneDrive-FacultadRegionalResistencia/Facultad/Materias Homogeneas/Fisica II`.
- Inventario preliminar:
  `/Users/carlosferreyra/Development/apuntes-frre/.transcription/dispatch-fisica-ii-2026-10-17/source-inventory.json`.
- Preflight de los 143 archivos COMPLETADO, copias numeradas y SHA-256:
  `/tmp/fisica-ii-20261017-fuentes`; inventario completo en `sources.json`.
- Extracciones y vistas: `/tmp/fisica-ii-conversion`.
- Archivo RAR de CD 2016 extraído con bsdtar en `/tmp/fisica-ii-conversion/cd`;
  software NO ejecutado.
- Textos Poppler por documento: `/tmp/fisica-ii-conversion/textos`.
- Pandoc DOCX: `/tmp/fisica-ii-conversion/docx` (solo primeros documentos).
- Faraday: `faraday-docling` (JSON, MD, medios), `faraday-pandoc`,
  `faraday-1.png`, `faraday-2.png`, `faraday.txt`.
- Potencial TP1: `potencial.md`, `potencial-medios`, `potencial-*.png`, PDF
  generado por LibreOffice del DOCX (no es PDF canónico).

## Cobertura verificada

- `notes/2015/practica/ley-de-faraday-laboratorio-9-bis.md`: PDF completo,
  páginas 1–2 comparadas visualmente con pdftoppm, cinco ecuaciones numeradas,
  tabla de cinco filas, esquema extraído con Docling, seis consignas.
- Procedencia y SHA-256 en `resources/2015/fuentes.md`.
- DOCX Faraday NO es duplicado: integrales definidas, procedimiento y tabla
  distintos. Pendiente transcripción separada.
- Prueba PyMuPDF4LLM: guía de campo magnético (13 páginas), salida en
  `problemas-parte-dos`. Solo página 1 revisada. Fórmulas y listas dañadas: NO
  publicar salida cruda ni declarar cobertura.
- AL ESTUDIANTE.docx identificado como extracto de Sears/Mark Hollabaugh:
  clasificar bibliografía, no incluir como apunte docente original.
- Extras contiene otras materias: Arquitectura, Sintaxis y Semántica,
  Probabilidad y Estadística, Ingeniería y Sociedad; excluir con evidencia.

## Validaciones

- documents:check: todas las herramientas disponibles; español spa verificado.
- Docling, mdformat y markdownlint help comprobados (lint --help devuelve 2).
- Conversión real Pandoc, PyMuPDF4LLM y Docling ejecutada.
- Docling Faraday omite cinco fórmulas, reparadas por comparación visual.
- mdformat aplicado a nota Faraday con GFM y MyST.
- Formato, lint y checker self-test/base aprobados para nota e inventario.
- Pendientes: diff check, commit, push, PR borrador y conteo MathJax real en
  GitHub.

## Próximo paso concreto

1. Completar controles y commit del laboratorio Faraday; abrir PR borrador.
1. Revisar en navegador GitHub la nota y contar math esperado/renderizado.
1. Completar inventario SHA-256 de preflight, deduplicados y pertenencia.
1. Continuar TP1 potencial: revisar todas las páginas del PDF normalizado,
   transcribir fórmulas WMF a LaTeX con evidencia; tablas y hoja de datos.
1. Avanzar por documentos, commit/push y actualizar este archivo en cada lote.

```sh
cd /Users/carlosferreyra/Development/apuntes-frre/isi-2008-fisica-ii
/Users/carlosferreyra/.local/bin/mise -C .github/transcription exec -- uv run check.py --self-test
/Users/carlosferreyra/.local/bin/mise -C .github/transcription exec -- uv run check.py --base origin/main
git diff --check
```

## Checkpoint 2 en cierre

- Checkpoint 1 remoto: `5d6a5b9`, PR borrador
  <https://github.com/apuntes-frre/isi-2008-fisica-ii/pull/1>.
- Faraday: GitHub verificado, 17/17 expresiones; cero merror/código residual.
- TP1 potencial: siete páginas normalizadas revisadas, todas las ecuaciones WMF
  reparadas y cinco figuras extraídas; fuente y SHA-256 registrados.
- Nota y medios guardados; cerrando lint y commit. Render GitHub pendiente.
- Preflight 143/143 finalizado con hashes y páginas. Textos Poppler extraídos.

## Checkpoint 3: inventario materializado

- Preflight: 143 archivos legibles, 124 hashes únicos, 2217 páginas PDF brutas
  (incluyen otras materias y duplicados).
- Inventario durable: `resources/common/inventario.json`; 2015/2019/2020 fuentes
  con hashes de todos los originales.
- Contenedores: `resources/common/contenedores.json`, 11319 miembros extraídos y
  hasheados; no se ejecutó software. Copias: `cd`, `emboe`, `fisica-zip` bajo el
  directorio temporal de conversión.
- TP1 GitHub: 26/26 expresiones, sin errores; inspección detectó numeración
  alterada por Pandoc, corregida con marcadores explícitos en este checkpoint.
  Imágenes lazy-load requieren desplazamiento para confirmar carga.
- Último checkpoint previo: `ad38928`. PR #1 sigue en borrador.
- Próxima acción: revisar render TP1 corregido y comenzar laboratorio 2 Laplace
  (DOCX ya extraído, falta PDF normalizado y comparación).

## Checkpoint 4: laboratorio 2 Laplace

- Tres notas completas: Faraday PDF (2 p.), TP1 DOCX (7 p. normalizadas), TP2
  DOCX (5 p. normalizadas).
- TP1 corregido: GitHub `29bb56f`, 26/26 math, cinco figuras cargadas, ocho
  pasos con numeración correcta.
- TP2: todas las cinco páginas revisadas, siete fórmulas reparadas, un montaje y
  cuatro tablas conservadas. Lint/checker en cierre; render GitHub pendiente.
- Salidas reutilizables: `laplace-1.png` a `laplace-5.png`, `laplace.txt`, DOCX
  y PDF normalizado bajo `/tmp/fisica-ii-conversion`.
- Siguiente documento pequeño: guía Polarización (2015, 1 página) y hojas de
  datos TP7/8.

## Checkpoint 5: polarización y formularios

- Laplace: render real GitHub 9/9 math y montaje cargado; corrección de
  puntuación de títulos ya publicada (consultar git log).
- Nuevas notas: polarización (1 p., ocho problemas y párrafo sin número, dos
  diagramas), hojas de datos TP7 (1 p., 14 filas vacías) y TP8 (1 p., ocho filas
  vacías y símbolo ausente en original señalado).
- Tres páginas completas comparadas visualmente; tablas corroboradas con PyMuPDF
  find_tables.
- Local checker/formato/lint aprobados; pendientes push y render GitHub de estas
  tres notas.
- Siguiente lote: guía de Coulomb 2018 (3 p.) o completar DOCX Faraday variante.
