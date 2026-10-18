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
- TP1 corregido: GitHub `e42bf07`, 26/26 math, cinco figuras cargadas, ocho
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

## Checkpoint 6: guía de Coulomb

- Guía 1.1 de 2019 (nombre 2018): páginas 1–3 revisadas, 9 preguntas, 10
  problemas, cinco diagramas y ecuación recuperada.
- Lint/checker aprobados antes de commit. Duplicado 92 cubierto por hash exacto.
- Checkpoint previo `22c08ff`: polarización y hojas TP7/8 renderizadas, 6/6, 6/6
  y 1/1 math.
- Próximo: render de Coulomb; guías 1.2 Campo eléctrico y 1.3 Gauss ya
  convertidas/renderizadas localmente en
  `/tmp/fisica-ii-conversion/campo-electrico*` y `gauss*`, aún NO
  revisadas/transcritas.

## Checkpoint 7: campo eléctrico y Gauss

- Campo eléctrico 1.2: 3 páginas, 9 preguntas, 13 problemas, 11 diagramas y tres
  ecuaciones gráficas recuperadas.
- Gauss 1.3: 3 páginas, 5 preguntas con apartados y 12 problemas, seis
  diagramas. Todas las páginas comparadas.
- math_expressions: campo 18 expresiones; Gauss 12. Pendiente verificación
  GitHub después del push.
- Coulomb GitHub verificado en `e267b67`: 28/28 expresiones y cinco figuras
  cargadas.
- Próximo: DOCX Faraday versión independiente; luego guías Kirchhoff/Puente de
  hilo.

## Checkpoint 8: Faraday DOCX y Kirchhoff

- Faraday DOCX completo, dos páginas normalizadas; versión distinta del PDF con
  tabla de dos filas y erratas propias preservadas.
- Kirchhoff DOCX completo, tres páginas normalizadas; circuito extraído y
  comparado, dos ecuaciones y dos tablas de tres registros vacíos.
- Se corrigieron encabezados vacíos artificiales de Pandoc en tablas GFM de
  notas ya publicadas; no son filas de datos del original.
- Gauss GitHub: 12/12 expresiones y seis diagramas cargados; Campo: 18/18,
  pendiente terminar confirmación de carga de sus imágenes.
- Salidas: `/tmp/fisica-ii-conversion/faraday-docx*`, `kirchhoff*`; herramientas
  y fuentes en manifiestos.
- Próxima acción: publicar checkpoint y verificar render. Luego Puente de hilo
  (Pandoc ya extraído; NO validado), conservando ecuaciones/imágenes con
  faltantes propios de la fuente.

## Checkpoint 9: potenciómetro de hilo

- DOCX laboratorio 5: cuatro páginas normalizadas comparadas, cuatro circuitos
  extraídos, fórmulas y leyendas incrustadas recuperadas como texto/LaTeX.
- Fuente usa capturas de Adobe con crop de Word; se respetó el recorte visible y
  se excluyó interfaz de Windows. Scripts reutilizables: `cortar-puente.py`,
  `reparar-puente.py` en el temporal.
- Nota guardada y checker aprobado; cerrar commit y render GitHub.
- Checkpoint previo remoto `9f6fdf8`: Faraday DOCX 16/16 math; Kirchhoff 2/2;
  montaje e imágenes pendientes de confirmación tras carga asíncrona.
- Próximo documento: laboratorio 3 Capacidad (11 p.) o laboratorio 4 Ley de Ohm
  (7 p.), aún sin conversión.

## Checkpoint 10: ley de Ohm y cobertura consolidada

- 13 documentos completos, 42 páginas cotejadas (PDF originales o normalizados
  identificados en cobertura), 188 expresiones matemáticas esperadas. No es la
  materia completa.
- Laboratorio 4: siete páginas originales, ocho figuras, tres tablas de 4/10/13
  columnas y cinco filas; ecuaciones reparadas con evidencia.
- Registro compacto de avance: `resources/common/cobertura.json`. Inventarios
  por año sincronizados con estados actuales.
- Script temporal para renovar manifiestos:
  `/tmp/fisica-ii-conversion/actualizar-cobertura.py`, ejecutar con el Python de
  mise mdformat, que importa el checker distribuido.
- Office restante extraído a `/tmp/fisica-ii-conversion/office`;
  inventario-office.json registra hojas/diapositivas y fallos. PPSX falla en
  MarkItDown incluso copia pptx, requiere normalizar con LibreOffice. No se
  publicó salida cruda.
- Capacidad: PDF de 11 páginas ya convertido y renderizado localmente en
  `capacidad*`, todavía sin revisar todas las páginas ni transcribir.
- Próximo: commit/render de Ohm y revisar Capacidad.

## Checkpoint 11: capacidad y régimen RC

- 14 documentos completos, 53 páginas comparadas, 231 math esperadas; fuente
  exacta/estado por documento en cobertura.json.
- Capacidad: 11 páginas completas, nueve figuras, ocho formularios lógicos; 43
  expresiones. Todas las fórmulas e imágenes revisadas.
- Figuras 6/7 faltaban en salida PyMuPDF4LLM; recuperadas directamente de xref
  73/76 del PDF original (sin sustitución de ecuaciones por capturas).
- Filas vacías contadas: tablas del cuerpo 3 registros, hoja carga 16, serie 14,
  paralelo 14, descarga 16; continuaciones de páginas 9 y 11 incluidas.
- Salidas: capacidad-tablas.json, capacidad-01.png a capacidad-11.png,
  reparar-capacidad.py. Primera tentativa de recorte de figuras 6/7 descartada,
  archivos finales contienen objetos originales correctos.
- Pendiente: render GitHub de Ohm (33 expresiones) y Capacidad (43),
  confirmación de imágenes de los últimos laboratorios; actualizar informe y CI.
- Próximo: laboratorios 7 y 8 completos (solo hojas de datos ya transcritas),
  PDF 42/45.

## Checkpoint 12: fuerza magnética

- 15 documentos, 59 páginas cotejadas, 250 math esperadas. Laboratorio 8
  completo: seis páginas y 19 math, tablas vacías de cinco/ocho filas.
- Recuadros de símbolos ausentes en el original señalados, sin inferirlos.
  Bibliografía y frase de procedimiento recuperadas visualmente.
- Capacidad en GitHub: 43/43 math y ocho formularios. Ohm: 33/33 y ocho imágenes
  cargadas.
- Se eliminan del inventario público tres extractos con datos de alumnos de otra
  materia; se conserva solo encabezado genérico. Se reescribirá exclusivamente
  el historial propio de esta rama para retirar también esas citas de versiones
  previas, conservando todos los checkpoints.
- Laboratorio 7: conversiones e imágenes listas en brujula-tangentes\*,
  pendientes de revisión de las 13 páginas.
- Legacy Office: normalización con LibreOffice en
  /tmp/fisica-ii-conversion/legacy; extraer con MarkItDown/Pandoc antes de
  revisar. No software ejecutado.

## Historial saneado

- HEAD del checkpoint 12: `5187a60`. Rama remota actualizada con
  force-with-lease, exclusivamente commits creados para esta transcripción.
- Se preservaron los 13 commits/checkpoints y el árbol final idéntico; solo se
  retiraron tres extractos de calificaciones ajenas de 10 inventarios
  históricos. main intacto.
- Mapa privado de SHA anteriores/nuevos:
  `/tmp/fisica-ii-conversion/mapa-commits-redactados.json`; no volver a publicar
  las versiones anteriores. Los SHA del registro se actualizan al historial
  saneado.
- No se afirma borrado de cachés/objetos del servidor; el historial activo de la
  rama ya no incluye los extractos.

## Checkpoint 13: brújula de tangentes

- 16 notas/secciones, 66 páginas revisadas, 285 math esperadas. Laboratorio 7
  corresponde a páginas 1–7 de PDF compuesto de 13; páginas 8–13 aún pendientes.
- Ocho ecuaciones, cinco figuras (tres diagramas y dos fotos), técnica y
  cuestionario íntegros, hoja con catorce registros; fuente/duplicado por hash y
  cobertura parcial bien marcados.
- Próxima acción: revisar visualmente páginas 8–13, comparar con fuente45 del
  laboratorio8 y transcribir variante/anexo sin presumir duplicado.
- Render GitHub de esta nota pendiente: 35 math. Último checkpoint de fuerza
  magnética19 math también pendiente.

## Checkpoint 14: cuadernillo completo de laboratorios 7 y 8

- 17 notas/secciones, 72 páginas comparadas, 305 math esperadas. Son 16 fuentes
  únicas de notas porque el PDF compuesto se divide en dos secciones. No se
  declara completa la materia.
- Fuente 42/43 (duplicados exactos) cubierta en páginas 1–13 por dos notas,
  incluida página 7 vacía y anexo gráfico de página 13.
- Nota de laboratorio8 versión2 incluye texto/ecuaciones/diagramas comunes
  cotejados y pendiente gráfica adicional, sin rellenar resultados.
- Helper actualizar-cobertura.py contempla rangos1–7 y8–13 y agrega notas por
  fuente; cuidar que duplicados con notas múltiples reciban también la lista
  notas, no una única nota antigua.
- Estado próximo: publicar y verificar render de laboratorio7 (35), laboratorio8
  (19), versión2 (20); imágenes pendientes tras carga asíncrona en algunos
  apuntes.
- A continuación: hojas DOCX independientes 54/55/56/57, guías de problemas
  extensas 50/51/52/77, planificación y teoría 2015/2019, informes y exámenes
  2020; bibliografía y otras materias separadas en inventario.

## Checkpoint 15: hojas DOCX independientes

- 21 notas/secciones, 76 páginas cotejadas, 315 math esperadas. Cuatro hojas
  adicionales de una página normalizada cada una: TP1/2/3/4.
- No son copias asumidas: TP1 siete potenciales y nueve lecturas; TP2
  malla11×11; TP3 tabla temporal0–200 con seis pares de columnas; TP4 tres
  tablas con título serie repetido, fórmulas recuperadas. Formularios/firmas
  vacíos conservados.
- Next: cerrar commit y verificar render; las cuatro hojas suman diez math (solo
  Ohm), las otras tres tienen cero.
- Páginas normalizadas: hoja-potencial-1.png, hoja-laplace-1.png,
  hoja-ohm-1.png, hoja-rc-1.png.
- Próximo lote: guía de problemas tercera parte (5p.) y guía polarización ya
  transcrita por separado; antes contrastar ejercicios/figuras.

## Checkpoint 16: guía tercera parte

- 22 notas/secciones, 81 páginas cotejadas, 348 expresiones matemáticas
  esperadas.
- Fuente50: cinco páginas completas; 6 problemas de interferencia, 8 de
  difracción, 9 de calorimetría y 8 de termodinámica. Seis figuras y tabla de
  signos con siete filas conservadas.
- Ecuaciones omitidas por el extractor recuperadas visualmente; datos
  discordantes y erratas del original señalados sin resolver ejercicios.
- Render GitHub nuevo pendiente: 33 expresiones y seis imágenes. Confirmar
  también cuatro hojas independientes y cargas de imágenes pendientes
  anteriores.
- Próximo documento: fuente51 (guía primera parte, 24 páginas), revisión por
  secciones; conservar avance antes de operaciones largas.

## Checkpoint 17: repaso vectorial

- 23 notas/secciones, 83 páginas cotejadas y 373 expresiones matemáticas
  esperadas.
- Fuente51 cubierta parcialmente: páginas3–4, nueve enunciados con numeración
  original repetida, 25 expresiones y figura de cuatro superficies.
- No declarar completa fuente51: faltan carátula, página institucional y
  secciones Coulomb/campo/Gauss/potencial/capacidad/circuitos y cola de
  óptica/termodinámica. Revisar solapamientos por contenido, no por nombre.
- Fuente50 commit f32c9cc: 33/33 math y seis imágenes cargadas verificadas en
  GitHub. Hoja Ohm:10/10 math. Laboratorio8versión2:20math y ocho referencias de
  imágenes cargadas.
- Próximo paso: verificar render vectorial y seguir fuente51 desde página5
  (Coulomb), sin confundir con guía2019 distinta de diez problemas.

## Checkpoint 18: Coulomb 2015

- 24 notas/secciones, 85 páginas cotejadas, 384 expresiones esperadas.
- Fuente51 parcialmente cubierta en páginas3–6: vectorial y Coulomb. Esta
  versión tiene nueve preguntas, once problemas y cinco figuras, incluido el
  ejercicio de esferas suspendidas que falta en guía2019.
- Vectorial publicado ada56ef y verificado:25/25 math, figura cargada.
  Coulomb2015 pendiente render:11 expresiones y cinco figuras.
- CI del checkpoint16 pasó. PR1 continúa borrador; descripción actualizada para
  reflejar el alcance parcial real.
- Próximo paso: fuente51 páginas7–9 campo eléctrico, comprobar límites exactos
  de sección antes de transcribir. Los extractores pierden ecuaciones e
  imágenes, no tomar texto plano como contenido completo.

## Checkpoint 19: campo eléctrico 2015

- 25 notas/secciones, 88 páginas-sección cotejadas y 392 expresiones esperadas.
- Campo2015: nueve preguntas, trece problemas, tres ecuaciones recuperadas y
  once figuras; páginas7–9. Página9 cubierta solo hasta fin del problema13;
  Gauss empieza en esa misma página y permanece pendiente.
- Coulomb2015 publicado ab2e462:11/11 math verificadas; imágenes aún en carga al
  primer chequeo, volver a comprobarlas.
- Vectorial:25/25 math y figura cargada verificadas; fuente51 continúa parcial.
- Próximo paso: fuente51 Gauss desde mitad de página9 hasta antes de potencial;
  renderizar página10 y determinar si continúa en11 antes de delimitar.
- No confundir suma de páginas por sección con páginas únicas cuando dos
  secciones comparten página.

## Checkpoint 20: Gauss 2015

- 26 notas/secciones y 400 expresiones esperadas. 91 páginas-sección cotejadas;
  90 páginas únicas porque campo y Gauss comparten página9.
- Gauss2015:cinco preguntas, doce problemas y seis figuras; páginas9–11 entre
  título de Gauss y título de potencial. Página11 solo Gauss está cubierta por
  esta nota.
- Coulomb2015:11/11math y cinco figuras cargadas verificadas. Campo2015
  commit60e042a:8/8math y once figuras cargadas verificadas.
- Próximo paso: verificar Gauss publicado (8math/seisfiguras), transcribir
  potencial desde mitad de página11; ver página12 y comienzo13 para delimitar
  final.
- Fuente51 todavía parcial; no se han validado las páginas restantes por existir
  extracciones.

## Checkpoint 21: potencial eléctrico 2015

- 27 notas/secciones, 416 expresiones esperadas y 94 páginas-sección cotejadas
  (92 páginas únicas).
- Potencial en páginas11–13: diez preguntas, once problemas con salto7→9 y ocho
  figuras. LetrasB/P impresas junto a subíndices/potencias se conservan y
  documentan.
- Fuente51 parcial hasta potencial en página13; capacidad empieza en esa misma
  página y no queda cubierta por esta nota.
- Siguiente: verificar render potencial16math/ochofiguras y
  Gauss8math/seisfiguras. Luego capacidad desde página13, renderizar14–15 para
  encontrar fin.
