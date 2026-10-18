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
- Preflight de los 143 archivos EN CURSO, copias numeradas y SHA-256:
  `/tmp/fisica-ii-20261017-fuentes`; al terminar genera `sources.json`.
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
- Pendientes: diff check,
  commit, push, PR borrador y conteo MathJax real en GitHub.

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
