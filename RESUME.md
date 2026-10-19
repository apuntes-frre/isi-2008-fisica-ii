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

## Checkpoint 22: capacidad y dieléctrico 2015

- 28 notas/secciones, 442 expresiones esperadas, 97 páginas-sección cotejadas
  (94 únicas).
- Capacidad páginas13–15: once preguntas, catorce problemas, once figuras.
  Página15 cubierta solo sección capacidad; circuitos empieza después.
- Potencial a93892d:16/16math y ocho figuras cargadas verificadas.
  Gauss0fc1187:8/8math y seis figuras cargadas verificadas.
- Capacidad pendiente render:26math y once figuras. Revisar formatos originales
  P/B conservados y asociación de los tres circuitos del problema5.
- Próximo: circuitos desde página15 hasta final antes de «GUIAS7 12 Segundo
  parcial en construccion» en19. Renderizar16–19, delimitar solapamientos con
  fuente50 por cotejo y no asumir duplicado.

## Checkpoint 23: primera parte completa

- 29 notas/secciones,455 expresiones esperadas. 102 páginas-sección de notas más
  carátulas y cola compartida; total105 páginas de fuentes únicas cotejadas
  (normalizadas para DOCX).
- Fuente51 completa en24p: siete notas nuevas de vectorial, Coulomb, campo,
  Gauss, potencial, capacidad y circuitos; cola19–23 compartida con fuente50 y
  carátula/páginas sin ejercicios registradas.
- Circuitos:19 preguntas con salto18→20,16problemas,gráfica de cuestionario
  y13figuras. Página19 incluye figuras12/13 y aviso de construcción,
  conservados.
- Capacidad b544ebb:26/26math,oncefiguras cargadas verificadas. Circuitos
  pendiente publicar/render:13math y14imágenes.
- Próximo: fuente52 segunda parte13p; inventariar títulos y delimitar secciones.
  Antes, confirmar CI y render de circuitos y cerrar cargas pendientes de
  imágenes anteriores.
- Helper actualizado con fuentes_adicionales en cobertura y estado completo de
  fuente51; no duplicar matemática ni apuntes por cola compartida.

## Checkpoint 24: fuerzas magnéticas

- 30 notas/secciones,487expresiones esperadas;108páginas de fuentes únicas
  cotejadas, incluidas24de fuente51 y3de fuente52. La suma de páginas-sección en
  helper excluye carátulas/cola compartida y cuenta solapamientos.
- Fuente52 parcial páginas1–3:15preguntas,14problemas con numeración Serway
  discontinua,6figuras; vectores recuperados visualmente. Fuente51 completa
  en1800502.
- Circuitos13/13math verificados;14imágenes estaban cargándose parcialmente al
  primer chequeo, volver a consultar sin navegar antes.
- Fuerzas pendiente publicar/render:32math y6figuras.
- Próximo: fuente52 campo de inducción/propiedades desde página4. Página4render
  ya revisado; renderizar5y6 para delimitar final y conservar
  Fig1P/etiquetas/unidades originales.

## Checkpoint 25: Biot–Savart y propiedades

- 31 notas/secciones,507expresiones esperadas;111páginas únicas de fuentes
  cotejadas. Fuente52 parcial en1–6; página6 cubierta solo sección propiedades.
- Propiedades:13preguntas,14problemas(1,2,5,8,9,12,15,16,19,20,21,28,31,32),10figuras.
  No confundir números al inicio de continuaciones con números de problema; las
  extracciones requieren cotejo visual.
- Circuitos1800502:13/13math y14imágenes cargadas verificadas.
  Fuerzas2848689:32/32math; cincofiguras cargadas y selector de velocidades aún
  cargándose al primer chequeo.
- Propiedades pendiente publicar/render:20math y10figuras.
- Próximo: inducción electromagnética desde mitad de página6; renderizar7–8 para
  localizar final y revisar todas las figuras y preguntas con respuestas en
  blanco.

## Checkpoint 26: inducción electromagnética

- 32 notas/secciones,515expresiones esperadas;113páginas únicas de fuentes
  cotejadas.
- Fuente52 parcial páginas1–8, página8 solo hasta fin inducción. Once preguntas,
  once problemas y cuatro figuras. Pregunta8 conserva cuatro espacios;
  problema27 refiere figuras31.29a–d ausentes de páginas6–8, señalado sin
  inventar.
- Fuerzas:32/32math,seisfiguras cargadas verificadas.
  Biot02f4bd2:20/20math,nuevefiguras cargadas y figura30.37 aún cargándose al
  primer chequeo.
- Inducción pendiente publicar/render:8math,cuatrofiguras.
- Próximo: magnetismo en medios materiales desde fin de página8; renderizar9–10
  y delimitar hasta título corrientealterna. Conservar tablas de
  magnetización/datos y fórmulas.

## Checkpoint 27: magnetismo en medios materiales

- 33 notas/secciones,529expresiones esperadas;115páginas únicas cotejadas.
  Fuente52 hasta página10 solo sección medios materiales.
- Medios:11preguntas,7problemas,1figura,tabla4registros de susceptibilidad
  y14paresH/B. ψ/χ y unidadA/m² originales conservados; H800.000 no se corrige.
- Inducción9a089b5 publicada; verificar8math/cuatrofiguras. Medios pendiente
  publicar/render14math/unafigura/dostablas.
- Próximo: corriente alterna empieza en página10; renderizar11–13 para delimitar
  final y Maxwell, recuperar fórmulas de valor eficaz que pdftotext pierde.

## Checkpoint 28: corriente alterna

- 34notas/secciones,557expresiones esperadas;116páginas únicas cotejadas.
  Fuente52 hasta página11; Maxwell12–13pendiente.
- Alterna:10preguntas,8problemas,7figuras(primeracon3circuitos),datos completos
  de R/L/C/f/ω de problema8. Cocientes de valor eficaz recuperados visualmente;
  pregunta3 conserva su omisión de verbo/signoigual.
- Medios a1315bb:14/14math,2tablas,figura cargada.
  Inducción9a089b5:8/8math,4figuras cargadas. Biot02f4bd2:20/20math,10figuras
  cargadas.
- Alterna pendiente publicar/render:28math,7figuras.
- Próximo: Maxwell/ondas en12–13; ambas páginas ya renderizadas y revisadas.
  Recuperar fórmulas de problema3/6 y conservar símboloK,operadorsen y unidades
  impresas.

## Checkpoint 29: segunda parte completa

- 35notas/secciones,575expresiones esperadas y118páginas de fuentes únicas
  cotejadas. Fuente51completa24p yfuente52completa13p; no significa materia
  completa.
- Maxwell páginas12–13:9preguntas,8problemas,1figura,18math; ecuaciones
  completas recuperadas visualmente.
- Fuente52 distribuida en seis notas: fuerzas, propiedades/Biot, inducción,
  medios materiales, alterna y Maxwell. Página6/8/10 compartida entre secciones;
  conservar rangos.
- Alternacb375d0 pendiente render28math/7figuras; Maxwell pendiente
  publicar/render18math/1figura.
- Próximo: cerrar render/CI y coberturas pendientes, luego
  fuente77guía2011(31p), planificación y teoría2015/2019, informes y
  exámenes2020. Fuente47cuadernillo98p debe compararse por secciones con
  laboratorios ya hechos; no declarar cubierto por simple parecido.
- Helpers, PNG y extracciones permanecen en /tmp/fisica-ii-conversion;
  manifiesto de143originales y copias recuperables en
  /tmp/fisica-ii-20261017-fuentes.

## Checkpoint 30: cierre de render de las35notas

-35notas,118páginas únicas cotejadas y575/575expresiones verificadas en GitHub,
sin merror. Cobertura registra todos los conteos; tres hojas sin matemática
verificadas también por sus tablas.

- Todas las cargas de figuras que estaban pendientes cerradas: circuitos14,
  fuerzas6,Biot10,inducción4,medios1,alterna7,Maxwell1,Kirchhoff1,FaradayPDF/DOCX1cadauno,polarización2;
  revisiones previas restantes constan en checkpoints anteriores.
- Fuente51 completa24p y52completa13p. PR1 borrador,sinmerge. Queda mucho
  material pendiente; no declarar materia completa.
- Fuente77guía2011:31p,renders guia-2011-01.png…31.png generados. Texto
  evidencia problemas de Coulomb distintos; no deduplicar por título. Siguiente
  revisar1–4 y transcribir sección Coulomb desde3–4; año2011soloen nombre,
  carpeta canónica2015.
- Estado deCI consultar después de último push. Inventarios completos y helpers
  de recuperación siguen en rutas descritas.

## Checkpoint 31: Coulomb de la guía 2011

- 36 notas o secciones, 609 expresiones esperadas y 122 páginas únicas
  cotejadas, incluidas la carátula y página vacía de fuente 77.
- Fuente 77 parcial: Coulomb en páginas 3–4, nueve preguntas y nueve problemas;
  tres figuras con siete paneles, conservadas en cinco archivos. Difiere de las
  otras guías en los ejercicios de átomo de hidrógeno, configuraciones
  tridimensionales y plano bisector.
- El año 2011 solo consta en el nombre; se conserva la carpeta canónica 2015.
  Las 575 expresiones anteriores están verificadas; Coulomb nueva tiene 34
  expresiones y cinco imágenes pendientes de publicación/render.
- Campo de la misma guía, páginas 5–6: revisión visual y borrador local hechos.
  Contiene exponentes positivos 9 y 8, y «2 un». Falta añadir la cobertura y
  validar antes del commit.
- Siguiente sección: Gauss, páginas 7–9. Sus imágenes están listas pero todavía
  no revisadas; no declararlas cubiertas.

## Checkpoint 32: campo eléctrico de la guía 2011

- 37 notas o secciones, 644 expresiones esperadas y 124 páginas únicas
  cotejadas.
- Campo en páginas 5–6: nueve preguntas, doce problemas y ocho figuras en cinco
  archivos. Se recuperaron λ, σ, α y φ visibles en el original, sin añadir
  símbolos ausentes en 11 y 12.
- Se verificaron ampliaciones: exponentes positivos 9 y 8, distancia «2 un»,
  «ángulo α a» y ausencia de σ en el enunciado 11. No se corrigen datos por
  plausibilidad física.
- Coulomb publicada en 7adb6fa: pendiente render de 34 expresiones y cinco
  imágenes. Campo pendiente publicar/render: 35 expresiones y cinco imágenes.
- Gauss páginas 7–9 ya cotejadas visualmente: once preguntas, once problemas,
  fórmulas y figuras adicionales. Falta crear nota y cobertura. Recuperar
  vectores, frecuencia del oscilador y rangos originales sin asumirlos desde
  otras versiones.

## Checkpoint 33: Gauss de la guía 2011

- 38 notas o secciones, 676 expresiones esperadas y 127 páginas únicas
  cotejadas.
- Gauss en páginas 7–9: once preguntas, once problemas y siete archivos de
  figuras, con diagramas compuestos. Se recuperaron símbolos bitmap, campo
  vectorial, frecuencia del oscilador e intervalos de los problemas 6, 10 y 11.
- Coulomb 2011: 34/34 expresiones verificadas. Campo 2011: 35/35 verificadas.
  Sus imágenes dieron ancho cero durante la carga inicial; volver a consultar y
  no afirmar carga completada todavía.
- Gauss nueva: pendiente publicación/render de 32 expresiones y siete imágenes.
  Fuente 77 sigue parcial hasta página 9.
- Siguiente: potencial de la misma guía, páginas 10–11. Los renders están listos
  pero todavía no se revisaron; no deduplicar por título.

## Checkpoint 34: potencial de la guía 2011

- 39 notas o secciones, 699 expresiones esperadas y 129 páginas únicas
  cotejadas.
- Potencial en páginas 10–11: diez preguntas, once problemas y siete figuras. La
  fórmula del dipolo tiene r, sin cuadrado; se conservan anillo/disco, E(r) y
  condiciones repetidas de interruptores.
- Coulomb y campo de 2011: 34 y 35 expresiones verificadas, cinco imágenes
  cargadas en cada nota. Gauss: 32/32 expresiones verificadas; algunas figuras
  aún cargándose al último chequeo.
- Potencial nueva: 23 expresiones y siete figuras pendientes de
  publicación/render.
- Capacidad en páginas 12–13 ya revisada y borrador local creado: siete
  preguntas, nueve problemas y tres archivos gráficos. Falta cobertura y
  validación. Preservar 5800Km y «diferencia de potencia»; μF del problema 9 se
  recuperó visualmente.
- Siguiente sección: dieléctricos en páginas 14–15; renders listos, aún sin
  revisar.

## Checkpoint 35: capacidad de la guía 2011

- 40 notas o secciones, 703 expresiones esperadas y 131 páginas únicas
  cotejadas.
- Capacidad en páginas 12–13: siete preguntas, nueve problemas y tres archivos
  gráficos. Se conserva el radio de 5800Km y «diferencia de potencia»; μF
  recuperado visualmente.
- Potencial 2011 publicado en 4eba6ec: pendiente render de 23 expresiones y
  siete imágenes. Capacidad nueva: cuatro expresiones y tres imágenes pendientes
  de publicación/render.
- Dieléctricos páginas 14–15 ya revisadas y borrador local creado: doce
  preguntas, once problemas, dos figuras. Se recuperaron la ecuación vectorial,
  permitividades, σP, μC y δ. Falta agregar cobertura y validar.
- Antes del siguiente lote: conservar extracción adicional de PyMuPDF4LLM para
  fuente77, además de pdftotext y renders ya usados, para contraste entre
  motores. Sin OCR ni descargas de modelos.
- Siguiente: circuitos de la guía 2011, páginas 16–19; todavía no revisadas
  visualmente.

## Checkpoint 36: dieléctricos de la guía 2011

- 41 notas o secciones, 732 expresiones esperadas y 133 páginas únicas
  cotejadas.
- Dieléctricos en páginas 14–15: doce preguntas, once problemas y dos figuras.
  Ecuación vectorial, permitividades, σP, μC y δ recuperados desde páginas, con
  ampliación del símbolo ε del problema 11.
- Fuente77: extracción adicional PyMuPDF4LLM terminada sin OCR en
  /tmp/fisica-ii-conversion/guia-2011-pymupdf, con medios referenciados. Se
  revisó el comienzo para contrastar notación y figuras; no sustituye el cotejo
  visual ni declara revisadas las páginas restantes.
- Dieléctricos nueva: 29 expresiones y dos figuras pendientes de
  publicación/render. Capacidad df1e4de pendiente render de cuatro expresiones y
  tres imágenes.
- Circuitos páginas 16–19 ya revisadas visualmente: veinte preguntas, dieciséis
  problemas, gráfica del cuestionario y trece figuras de problemas. Falta crear
  nota, cobertura y validar. Recuperar símbolos bitmap y conservar los errores
  de texto de esta versión.
- Próximo después de circuitos: fuerzas magnéticas en páginas 20–21; todavía no
  cotejadas.

## Checkpoint 37: circuitos de la guía 2011

- 42 notas o secciones, 752 expresiones esperadas y 137 páginas únicas
  cotejadas.
- Circuitos en páginas 16–19: veinte preguntas y dieciséis problemas, gráfica
  del cuestionario y trece figuras de problemas. Símbolos de fem, resistividad,
  conductividad, unidades y corriente recuperados; llave sin cerrar e i9 se
  conservan.
- Gauss, potencial, capacidad y dieléctricos de 2011 ya verificadas en GitHub:
  32, 23, 4 y 29 expresiones, respectivamente, con todas sus figuras cargadas.
  Son 732 expresiones verificadas en las primeras 41 notas.
- Circuitos nueva: veinte expresiones y catorce imágenes pendientes de
  publicación/render.
- Fuerzas magnéticas de la guía 2011, páginas 20–21, ya cotejadas. Quince
  preguntas y catorce problemas diferentes de la otra guía, tres figuras. Falta
  crear nota; recuperar fórmula del problema 5 y μV del 9.
- A partir del siguiente checkpoint, validar localmente con base HEAD los
  archivos nuevos/cambiados; el conjunto anterior ya pasó y CI seguirá
  comprobando toda la rama. No repetir sin necesidad el mismo conjunto completo
  en cada checkpoint.

## Checkpoint 38: fuerzas magnéticas de la guía 2011

- 43 notas o secciones, 773 expresiones esperadas y 139 páginas únicas
  cotejadas.
- Fuerzas en páginas 20–21: quince preguntas, catorce problemas consecutivos y
  tres figuras. Fórmula mp·vo=Bo·Qp·ρ recuperada y dato 35μV conservado. El
  problema 14 no da dimensiones; no añadirlas.
- Fuente77 parcial hasta página 21. Nueva nota: 21 expresiones y tres figuras
  pendientes de publicación/render. Circuitos 2011 pendiente render de veinte
  expresiones y catorce imágenes.
- Las 732 expresiones de las primeras 41 notas ya verificadas, con figuras
  cargadas. Contadores actualizados en helper/cobertura.
- Biot–Savart/propiedades en páginas 22–23 ya cotejadas: trece preguntas, diez
  problemas y siete archivos gráficos. Falta crear nota y cobertura. Recuperar
  ecuación de hilo finito del problema 5 y mantener diez problemas, sin usar la
  selección distinta de otra guía.
- Próximo después: inducción de páginas 24–25, aún sin cotejar.

## Checkpoint 39: Biot–Savart de la guía 2011

- 44 notas o secciones, 783 expresiones esperadas y 141 páginas únicas
  cotejadas.
- Propiedades en páginas 22–23: trece preguntas, diez problemas y siete archivos
  gráficos. Ecuación del hilo finito recuperada; diez problemas consecutivos
  propios de esta versión.
- GitHub dejó r9 del apunte de circuitos como código por estar pegado a
  «resistencia». Se añadió un espacio antes de la matemática; verificar tras
  push que suba de 19 a 20 expresiones. No había error merror, por eso es
  necesario comparar conteos.
- Fuerzas de 2011: 21/21 expresiones y tres figuras cargadas verificadas. Biot
  nueva: diez expresiones y siete imágenes pendientes de publicación/render.
- Inducción páginas 24–26 ya cotejadas hasta el problema 12; comparte página 26
  con medios materiales. Falta crear nota y cobertura: once preguntas, doce
  problemas y diez imágenes. Recuperar μT, φ(t), π de la corriente y conservar
  mwb/m² y rn/seg del original.
- Medios materiales desde página 26 empieza con once preguntas; la página 27
  todavía no está cotejada. No declarar cubierta la sección.

## Checkpoint 40: inducción de la guía 2011

- 45 notas o secciones, 798 expresiones esperadas y 144 páginas únicas
  cotejadas.
- Inducción en páginas 24–26: once preguntas, doce problemas y diez archivos
  gráficos. El problema 12 continúa en 26 antes de medios materiales; μT, φ(t) y
  π recuperados.
- Circuitos corregida: 20/20 expresiones, ningún código matemático residual y
  catorce imágenes cargadas verificadas. Fuerzas: 21/21 y tres imágenes. Biot:
  10/10 y siete imágenes. Las primeras 44 notas suman 783 expresiones
  verificadas.
- Inducción nueva: quince expresiones y diez imágenes pendientes de
  publicación/render.
- Medios materiales de páginas 26–27 ya cotejada visualmente: contenido, siete
  problemas, once preguntas y tablas coinciden con la nota ya transcrita de
  fuente52, con distinta paginación. El diff de palabras muestra pérdidas de
  símbolos y orden de tabla de los extractores, sin diferencias de datos. Falta
  registrar fuente adicional y confirmar imagen original compartida; no duplicar
  matemática por el solapamiento.
- Siguiente: corriente alterna de páginas 28–29 y Maxwell 30–31. Todavía no
  revisadas visualmente.

## Checkpoint 41: procedencia compartida de medios materiales

- Se mantienen 45 notas y 798 expresiones; 145 páginas únicas de fuentes
  cotejadas.
- Fuente77 páginas26–27 registrada como procedencia adicional de la nota de
  medios materiales de fuente52. Once preguntas, siete problemas, cuatro
  registros de susceptibilidad y catorce pares H/B coinciden tras cotejo visual.
- Figura de la varilla: mismo bitmap de 250×238 píxeles, digest
  decodificado23a1de2c05cbfef1b6872e94913ee016 en ambosPDF. Se comparte nota y
  no se duplica matemática.
- Fuente77 parcial hasta página27; alterna28–29 ya cotejada visualmente y
  comparada en texto: mismos diez interrogantes, ocho problemas y datos de
  circuito. Falta registrar procedencia adicional y confirmar siete bitmaps.
  Registrar repetición de «Figura2P» en cambio de página.
- Maxwell30–31 todavía no revisadas. Inducción2011 pendiente render de quince
  expresiones y diez imágenes.

## Checkpoint 42: procedencia compartida de corriente alterna

- Se mantienen 45 notas y 798 expresiones; 147 páginas únicas cotejadas.
- Fuente77 páginas28–29 registrada como procedencia adicional de corriente
  alterna. Diez preguntas, ocho problemas, datos R/L/C/f/ω y siete figuras
  coinciden; comparación de digests de píxeles confirma los siete bitmaps
  idénticos. Se registra rótulo Figura2P repetido en cambio de página.
- Maxwell30–31 ya cotejada: mismos nueve interrogantes y ocho problemas.
  Ecuación6 presenta delimitadores superpuestos sobre x; el recorte ampliado y
  capa textual confirman x. Guardar recorte como evidencia al compartir nota,
  sin cambiar signos o valores. Falta confirmar bitmap de la onda y registrar la
  procedencia adicional.
- Inducción2011 todavía pendiente render de quince expresiones y diez imágenes.
  Fuente77 no declarar completa hasta incorporar Maxwell y evidencia de la
  superposición gráfica.

## Checkpoint 43: cierre documental de la guía identificada como 2011

- 45 notas, 798 expresiones esperadas y 149 páginas únicas de fuentes
  cotejadas visualmente. La materia completa sigue pendiente.
- Fuente77: 31 páginas revisadas; carátula y página vacía registradas, diez
  secciones propias y tres compartidas con fuente52. Maxwell30–31 queda
  registrado con su SHA-256 y recorte de la superposición gráfica en ecuación6.
- Validación local del cambio: checker de transcripción y lint sin incidencias.
- Pendiente: verificar en GitHub las quince expresiones y diez imágenes de
  inducción2011 y las adiciones de procedencia compartida, incluida la imagen
  de Maxwell. Después inventariar por páginas el compilado fuente47 de98p,
  comparándolo con laboratorios ya cotejados antes de transcribir variantes.

## Checkpoint 44: primeras secciones del compilado de laboratorios

- 48 notas y 810 expresiones esperadas. 154 páginas únicas de fuentes revisadas
  visualmente, incluidas carátulas y anexo; no es cobertura completa de la materia.
- Inducción2011 confirmada en GitHub: 15/15 expresiones y diez imágenes cargadas.
  Maxwell confirmado: 18/18 y ambas imágenes cargadas, incluido recorte2011.
- Fuente47: mapa textual de laboratorios1–17 y anexo en inventario. Ninguna página
  idéntica en render72dpi gris con fuentes40,41,42,45,73; no se asume duplicación.
- Hojas35 y39 transcritas: FEM con ocho expresiones y Kirchoff con cuatro; seis
  filas vacías para integrantes, tres lecturas por tabla y celdas combinadas.
- Página57 cotejada: solo presentación de Faraday; aviso de guía adicional
  incorporado en nota existente. Carátula1 cotejada. Anexo98: bitmap JPEG
  original conservado y29etiquetas transcritas; extracción textual las omite.
- Checker local pasó para las cinco notas/inventario modificados. Pendiente
  render de nuevas hojas y anexo, y resto del compilado47. Próximo: laboratorio9
  páginas52–56, distinto de la presentación9bis y guía adicional ya cubiertas.

## Checkpoint 45: Faraday y coeficiente de inducción del toroide

- 49 notas, 844 expresiones esperadas y159 páginas únicas cotejadas visualmente.
- Fuente47 páginas52–56 completas: laboratorio9, aviso9bis, cuatro figuras en
  tres archivos, ecuaciones1–10 con10 repetida, dos tablas de lecturas y hoja de
  datos. Se preservan signos menos de8/9, referencia de figura1/2 y reostato2/4A.
- Dos hojas del checkpoint44 confirmadas en GitHub: FEM8/8 y Kirchoff4/4,
  tablas8+4filas y8+4+4filas respectivamente. GLX:0math,29etiquetas y JPEG cargado.
- CI content del checkpoint44 pasó. Laboratorio9 suma34 expresiones y tres
  imágenes, todavía pendiente render GitHub. Próximo: laboratorio10 páginas58–64
  del compilado, seguido de11–17 y variantes de1–8. Mantener inventario parcial.
- Extracción PyMuPDF4LLM del compilado98p terminada sin OCR en8segundos en
  /tmp/fisica-ii-conversion/compilado47-pymupdf; texto de referencia adicional en
  /tmp/fisica-ii-conversion/textos. No tomar salida automática como cotejo total.

## Checkpoint 46: circuitos serie de corriente alterna

- 50 notas,919 expresiones esperadas y166 páginas únicas cotejadas visualmente.
- Fuente47 páginas58–64 completas: siete figuras más recorte de ecuaciones,
  pasos RL10/RC11/RLC8, hoja vacía de dos páginas y75 expresiones. Preservados
  RCL, salto5→7, VL en16.3, R=VC/I, ánguloRC positivo y rótulos repetidos4/5.
- Ecuaciones15/17/18 tienen delimitadores defectuosos sobre símbolos en PDF;
  recorte conservado y componentes contrastados con capa textual y diagrama.
- Checker local y git diff --check pasaron. Pendiente render GitHub de75
  expresiones y ocho imágenes de esta nota. Faraday9 ya confirmado34/34,
  tres imágenes cargadas y tablas7/5/2/11filas.
- Próximo: laboratorio11 fotometría páginas65–69; después12–17, y cotejo de
  variantes1–8. No declarar completo el compilado ni la materia.

## Checkpoint 47: fotometría

- 51 notas,934 expresiones esperadas y171 páginas únicas cotejadas visualmente.
- Fuente47 páginas65–69 completas: fotometría, cuatro imágenes, dos pasos de
  preparación, dos procedimientos y tablas10/11lecturas; quince expresiones.
  Conservadas Irradiancia(I), Figura4b, metros/cm y erratas textuales.
- Corriente alterna confirmada en GitHub75/75, ocho imágenes cargadas y listas
 10/11/8. Fotometría pendiente render15math, cuatro imágenes y tres tablas.
- Próximo: interferencia70–73 y difracción74–77; luego espectrómetro78–80,
  polarización81–89, termometría90–93, calorimetría94–97 y variantes1–8.

## Checkpoint 48: interferencia

- 52 notas,955 expresiones esperadas y175 páginas únicas cotejadas visualmente.
- Fuente47 páginas70–73 completas: tres figuras, recorte de ecuaciones con
  delimitadores superpuestos, cuatro ecuaciones numeradas,21 expresiones y hoja
  con cuatro lecturas vacías. Se conservan objetivos distintos y HeNe/NeNe.
- Fotometría confirmada en GitHub15/15, cuatro imágenes y tablas5/11/12filas.
  Interferencia pendiente render21math, cuatro imágenes y tabla5filas.
- Checker local pasó; comparación adicional con pdftotext-layout del compilado
  confirma texto, erratas y limitaciones de extracción de fórmulas. Próximo:
  difracción74–77, luego espectrómetro78–80 y laboratorios15–17.

## Checkpoint 49: difracción

- 53 notas,977 expresiones esperadas y179 páginas únicas cotejadas visualmente.
- Fuente47 páginas74–77 completas: seis figuras,22 expresiones, seis pasos de
  técnica y hoja con12filas vacías; conteo de tabla confirmado13filas con cabecera.
  Conservadas variantes a/p/l frente aα/π/λ, r/ρ, HeNe/NeHe/NeNe y numeración
 6,7,3,4,5,6,7. No se completan datos.
- Interferencia confirmada en GitHub21/21, cuatro imágenes cargadas y ambas
  tablas5filas. Difracción pendiente render22math y seis imágenes.
- Próximo: espectrómetro78–80, polarización81–89, termometría90–93,
  calorimetría94–97 y variantes1–8. Compilado y materia siguen parciales.

### Reparación del control de numeración del checkpoint49

- MD029 rechazó la lista que empieza en6. Se agregó una excepción local solo
  para esa lista original6/7; se conserva su inicio y el resto de reglas.
- Checker de transcripción y lint volvieron a pasar tras el ajuste.

## Checkpoint 50: espectrómetro de red de difracción

- 54 notas,988 expresiones esperadas y182 páginas únicas cotejadas visualmente.
- Fuente47 páginas78–80 completas: dos figuras,11 expresiones, cinco pasos y
  hoja8–14 sin resolver. Conservados N en ambos lugares del segundo factor de
  intensidad, falta de fórmula tras definición de dispersión y5276líneas/cm
  frente a1/600mm con aviso de verificar.
- Difracción confirmada en GitHub22/22, seis imágenes cargadas, tablas5/13filas
  y lista original con inicio6. Checker de la nueva nota y git diff --check pasaron.
- Espectrómetro pendiente render11math y dos imágenes. Fuente47 revisada solo
  en1,35,39,52–80,98; restantes páginas no cubiertas por semejanza de títulos.
- Próximo documento: polarización81–89, seguido de termometría90–93,
  calorimetría94–97 y cotejo de variantes1–8. Materia completa sigue pendiente.

## Checkpoint 51: cierre de render y siguiente lote

- Espectrómetro confirmado11/11, dos imágenes cargadas y listas5/7elementos,
  esta última con inicio8. Todas las54notas tienen conteos GitHub confirmados,
  total988expresiones;182páginas únicas de fuentes cotejadas visualmente.
- Próximo trabajo autorizado: polarización del compilado47 páginas81–89.
  Conservar todos los casos de polarización, diagramas, experiencias y hojas;
  no confundir con problemas de polarización fuente48 ya transcritos.

## Checkpoint 52: polarización de la luz

- 55 notas,1035 expresiones esperadas y191 páginas únicas cotejadas visualmente.
- Fuente47 páginas81–89 completas:13figuras,47expresiones, desarrollo de
  polarización lineal/circular/elíptica, dicroísmo, Brewster, Malus, materiales
  fotoelásticos, cuatro trabajos y hoja con36ángulos. Se preservan signos,
  convención de giro, αP/θP, ausencia de paréntesis sen90°−θP y n1/n2.
- Texto contrastado también con pdftotext-layout. Checker local y diff --check
  pasaron. Pendiente render47math,13imágenes y tabla13filas×6columnas.
- Próximo: termometría90–93 y calorimetría94–97; después cotejar variantes1–8
  del compilado. No declarar completa materia ni compilado.

## Checkpoint 53: termometría

- 56 notas,1044 expresiones esperadas y195 páginas únicas cotejadas visualmente.
- Fuente47 páginas90–93 completas: modelo exponencial y parámetros A/B,
  un montaje,12pasos, tablas3y12filas de datos vacías. Nueve expresiones.
- Polarización confirmada47/47,13imágenes cargadas y tablas5/13filas.
- Checker local de termometría pasó; pendiente render9math, imagen y tablas.
- Próximo: calorimetría94–97. Luego cotejar páginas2–51 del compilado,
  sin asumir que las variantes individuales ya transcritas cubren este PDF.

## Checkpoint 54: calorimetría

- 57 notas,1073 expresiones esperadas y199 páginas únicas cotejadas visualmente.
- Fuente47 páginas94–97 completas: dos experiencias con siete pasos cada una,
  materiales, actividades, balances y fórmulas;29expresiones. Imagen original
  de ocho accesos del GLX y tabla textual de los iconos. Se conserva Qabs=-Qced
  y signos posteriores,80C, barra de división y agrupación de la fórmula de c.
- Termometría confirmada9/9, imagen cargada y tablas4/5/13filas. Calorimetría
  pendiente render29math, una imagen y tabla de ocho operaciones. Checker local
  y diff --check pasaron. Texto contrastado con pdftotext-layout.
- Fuente47: revisadas1,35,39,52–98. Pendiente cotejo visual y documental2–51
  excepto hojas35/39. Próximo: comparar laboratorios1–8 con versiones ya
  transcritas; no duplicar notas si contenido coincide tras cotejo completo.

## Checkpoint 55: variante de Kirchoff del compilado

- 58 notas,1079 expresiones esperadas y202 páginas únicas cotejadas visualmente.
- Fuente47 páginas36–38 transcritas como variante separada: R2=1,5kΩ y
  R3=3,3kΩ, frente a cifras intercambiadas en DOCX60. Encabezados Vcf/Vgb
  también distintos. Se conserva todo el texto, circuito, dos leyes y dos tablas.
- Seis expresiones y una imagen pendientes de render. Checker local pasó.
- Calorimetría confirmada29/29, imagen cargada, tabla9filas y listas7/7. CI
  content del checkpoint54 pasó. Compilado sigue parcial: revisadas1,35–39,52–98.
- Comparación textual preliminar de laboratorios1–8 contra versiones individuales
  detecta variantes; evidencia temporal en comparacion-labs47.json. No acredita
  cotejo de páginas restantes. Próximo: FEM/potenciómetro31–34 y después
  laboratorios1–4,7–8 con sus hojas.

## Checkpoint 56: FEM y potenciómetro del compilado

- 59 notas,1094 expresiones esperadas y206 páginas únicas cotejadas visualmente.
- Fuente47 páginas31–34 completas como variante separada del DOCX69: cuatro
  figuras originales PDF,15expresiones, calibración, medición y sensibilidad.
  Se conserva Vc−Va en el párrafo del cursor, d.d.p. y finales con punto/guion.
- Kirchoff del compilado confirmado6/6, imagen cargada y tablas4/4filas.
- Checker local del potenciómetro y diff --check pasaron. Pendiente render
 15math y cuatro imágenes. Fuente47 cotejada1,31–39,52–98; resto pendiente.
- Próximo: laboratorio7 páginas40–45 y8 páginas46–51, incluidas hojas; luego
  laboratorios1–4 páginas2–30. Comparar las versiones individuales sin asumir
  identidad por título o porcentaje de coincidencia textual.

## Checkpoint 57: cierre verificado del potenciómetro

- Potenciómetro confirmado en GitHub15/15, cuatro imágenes cargadas y sin
  errores matemáticos ni fórmulas expuestas como código.
- Las59notas tienen conteos de render confirmados:1094expresiones. Fuentes
  cotejadas visualmente:206páginas únicas. Materia y compilado siguen parciales.
- Siguiente punto exacto: fuente47 páginas40–45 (laboratorio7 y hoja) y46–51
  (laboratorio8 y hoja), después2–30 (laboratorios1–4). No repetir lo ya cubierto
  en31–39,52–98 o confundir versiones individuales.

## Checkpoint 58: brújula de tangentes del compilado

- Instrucción vigente del usuario: continuar hasta estar listo para merge; no
  aprobar ni unir todavía. Solo se consultó PR1; sigue en borrador. La búsqueda
  de PR abiertos de apuntes-frre devolvió únicamente este PR, sin otras materias.
- 60 notas,1129 expresiones esperadas y212 páginas únicas cotejadas visualmente.
- Fuente47 páginas40–45 completas como variante: cinco imágenes,35expresiones,
  ecuaciones1–8, seis materiales, once pasos, tres preguntas, una lectura vacía
  en técnica y catorce en hoja. La identidad conserva seis integrantes y grupo.
- Se preservan(6)sin2, Ksin1/2, μo con s² y tg/Tang; paso4 ya no se repite
  en este original. Checker local y diff --check pasaron. Pendiente render35math
  y cinco imágenes. Próximo: fuerza magnética páginas46–51, después2–30.

## Checkpoint 59: fuerza magnética del compilado

- Instrucción del usuario reafirmada: trabajar hasta estar listo para merge,
  sin unir ni aprobar todavía. Mantener el PR en borrador mientras falte contenido.
- 61 notas,1150 expresiones esperadas y218 páginas únicas cotejadas visualmente.
- Fuente47 páginas46–51 completas:21expresiones, cinco figuras y forma de
  espira reutilizada, procedimientos1.1–1.3 y2.1–2.6, tablas5y8lecturas vacías.
  Se conserva L como densidad y horizontal/vertical. Dos θ recuperados de capa
  textual se marcan por cuadro del render; no se infieren de la teoría.
- Brújula compilada confirmada35/35, cinco imágenes, tablas2/8/15filas.
  Fuerza pendiente render21math y ocho apariciones de seis imágenes únicas.
- Checker local y diff --check pasaron; texto también contrastado con Poppler.
- Fuente47 cubierta1,31–98. Restan2–30: laboratorios1–4 y hojas. Próximo:
  Ohm24–30, despuésRC15–23, Laplace9–14 y potencial2–8. Después continuar
  con el resto de originales pendientes del inventario; no declarar materia completa.

## Checkpoint 60: Ohm y asociaciones del compilado

- 62 notas,1193 expresiones esperadas y225 páginas únicas cotejadas visualmente.
- Fuente47 páginas24–30 completas: ocho figuras,43expresiones, teoría de
  serie/paralelo y tres tablas del cuerpo más tres en la hoja, cinco lecturas
  cada una; columnas4/10/13. Se conservan R1=2,7KΩ y R2=3,3KΩ, Vbd en tabla
  y Vac/Vbd en preguntaD. Hoja repite encabezado de serie sobre tabla de paralelo.
- Fuerza magnética confirmada21/21, ocho apariciones de imágenes cargadas y
  tablas6/8/9filas. Ohm pendiente render43math, ocho imágenes y siete tablas.
- Checker local y diff --check pasaron; cotejo Poppler adicional. Fuente47
  cubierta1,24–98. PróximoRC15–23, Laplace9–14, potencial2–8. Continuar luego
  con originales pendientes: el PR no está listo para aprobar ni fusionar.

## Checkpoint 61: circuito RC del compilado

- 63 notas,1236 expresiones esperadas y234 páginas únicas cotejadas visualmente.
- Fuente47 páginas15–23 completas: nueve figuras y recorte de ecuaciones
  defectuosas,43expresiones, siete pasos de carga, cinco de descarga y
  procesamiento3.1–3.7 con3.3repetido. Datos R39000Ω,C11000µF,C2470µF,ΔR5%.
  Hoja con21instantes0–200s y seis pares de lecturas,13columnas.
- Se preservan salto9→11,19repetida,+0en17 y referencias del original. No se
  importan hojas del PDF individual distintas de esta matriz. Checker local
  y diff --check pasaron; pendiente render43math y diez imágenes.
- Ohm confirmado43/43, ocho imágenes y tablas6filas×4/10/13columnas en cuerpo
  y hoja, identificación8filas. Fuente47 cubierta1,15–98. Próximo9–14Laplace,
  luego2–8potencial. El PR sigue en borrador y la materia incompleta.

## Checkpoint 62: Laplace del compilado y corrección de índice

- 64 notas,1245 expresiones esperadas y240 páginas únicas cotejadas visualmente.
- Fuente47 páginas9–14 completas: nueve expresiones, montaje, tablas9×9 de
  experimental12V y teórica10.0V, hoja11×11 vacía conØ y X/Ymayúsculas.
- Se corrigió E_i a E_I en ambas versiones de Laplace: bitmap220×75 idéntico
  en DOCX39 y compilado, SHA-256 de píxeles e5e621076712eae487e411a955699c73a6e76ee4238ef8c9fd3391740291f7c6.
  Imagen original conservada y explicación agregada a ambas notas. Revisar render
  de ambas9math y de dos imágenes por nota. Checker local y diff --check pasaron.
- RC confirmado43/43, diez imágenes y tablas8/8/3/8/23filas; matriz13columnas.
- Fuente47 cubierta1,9–98. Restan2–8potencial y su hoja. Después de cerrar
  compilado continuar originales pendientes del inventario; materia sigue incompleta.

## Checkpoint 63: compilado de98páginas completo

- 65 notas,1271 expresiones esperadas y247 páginas únicas de fuentes cotejadas
  visualmente. Fuente47 completa1–98: todos los laboratorios1–17, presentación
 9bis, hojas, carátula y anexoGLX. No implica que toda FísicaII esté completa.
- Potencial2–8:26expresiones, cinco figuras, ocho pasos y nota original de
  pendientes. Hoja de siete grupos V1–V7 y nueve lecturas,15columnas, distinta
  del DOCX. Se conservan V9=7Vo/8, salto3→5, relación13 y erratas del texto.
- Checker local y diff --check pasaron; pendiente render26math, cinco imágenes
  y cinco tablas. Laplace nuevo e individual confirmados9/9 cada uno, ambas
  imágenes cargadas e índiceI confirmado en MathML.
- Próximo: revisar inventario de originales pendientes y continuar teoría,
  guías/modelos y otros años. Mantener PR en borrador hasta completar alcance
  y verificación, conforme a instrucción del usuario.

## Checkpoint 64: copias de idéntico render y próximo examen

- Las65notas están verificadas en GitHub:1271expresiones y247páginas únicas
  cotejadas visualmente. Compilado completo, pero materia aún incompleta.
- Fuente43 con SHA idéntico a42 tenía estado atrasado; corregida propagación
  de estado y páginas cuando la referencia tiene varias notas.
- Fuentes44/42:13/13páginas idénticas en dimensiones y muestras de render
 72dpi gris.46/45:6/6idénticas. Comparten notas sin sumar páginas a la cuenta
  de revisión visual manual. Evidencia por página en duplicados-render.json.
- Fuentes5/1:27/27idénticas en render, pero ambas siguen pendientes. Fuente66
  es SHA idéntico a1. Esta igualdad no se declaró transcripción completa.
- Checker local de tres notas con procedencia adicional y diff --check pasaron.
- Próximo: fuente1 modelos de parciales/finales27páginas, versión1.1fechada
 04/08/2010; fuentes5/66comparten contenido. Numerosas páginas3–8,14–21
  tienen imagen sin texto: preparar OCR español sobre copia y cotejar todo.
- Material que figura IEM/IQ debe conservar esa identificación y no atribuir
  automáticamente a ISI; la fuente está en carpeta canónica FísicaII.

## Checkpoint 65: modelos de exámenes, OCR y primeras ocho versiones

- Fuente1 modelos27p: OCR --skip-text omitía todas porque hay una capa de
  espacios. OCR español --force-ocr sobre copia temporal produjo texto; se
  conservó extracción PyMuPDF4LLM y Poppler en modelos-examenes-ocr. Original intacto.
- Nuevas8notas: página3 dos exámenes, página4 temas1 yF2, página5 inferior
  parcial2007temaA, páginas10–12 recuperatoriosIEM2010 temas1/2 y parcial16/09/08.
  No declarar completa página5: su recuperatorio superior sigue pendiente.
- Las cinco primeras notas publicadas se verificaron en GitHub:16+17+7+0+4
  expresiones; cinco figuras de los recuperatorios/2008 y dos de página3 cargadas.
  Acumulado confirmado70notas/1315math. Otras3notas pasan controles locales:
  8+5+5 expresiones; pendiente renderGitHub tras publicar.
- Conservados exponente15 en atm/Pa, repeticiónc), carga16sinpunto, masa3,11,
  tiempo2seg, V2textual/V1figura, identificaciónIQ/IEM y formularios sin completar.
- Figuras de problemas3/4 del tema2IEM continúan arriba de página12; las del
  tema1 están en página10 con rótulos desplazados a11. No confundir exámenes.
- Páginas1–12 renderizadas y vistas como orientación; para revisión terminada
  del texto/diagramas contar1,2,3,4,10,11,12; página5 solo examen inferior.
  Restantes4–9 requieren cubrir cada examen faltante, además de14–27.
- Próximo: verificar render de tres notas recién preparadas y continuar
  recuperatorioIQtemaA superiorp5; luego p6–9 y segunda mitad del compilado.
  Fuente5 tiene27/27rendersidénticos y66esSHAidéntico: siguenparcialescon1.

## Checkpoint 66: 82 notas publicadas y verificadas

- Las82notas y1353expresiones están verificadas en GitHub; todas las figuras
  de las9notas adicionales cargaron completas. Controles locales check74pasaron.
- Además: recuperatorio2008tema2 página6superior, tema2varilla página7superior,
  recuperatorioextraordinarioIEM2010 página22superior, segundosparciales2010
  temas1/2 páginas22–23, finalesmarzo2010 y17/12/09 página25, IQ2009temas1/2
  páginas26–27. No atribuir IQ/IEM automáticamente a ISI.
- Separadores13/24vistos: «Modelos de segundo parcial»/«Problemas de final».
  No contienen ejercicios. Páginas22–23 y25–27 completamente cotejadas;
  fuente1aúnparcial. Paginas3,4,10–12 completas;5,6,7soloexámenesindicados.
- Queda sin usar/referenciar iq-recuperatorio-tema-a-figuras.png (propio),
  destinado a siguiente nota página5superior. Revisar exponente de Q1 en
  recorte tema-a-iq-texto.png antes de transcribirlo: OCR no lo reconoce;
  no inferirlo desde otros exámenes similares. Q2 imprime10-9 en línea.
- Restan primerparcialp5superior,p6inferior,p7inferior,p8ambos,p9ambos;
  luego escaneados14–21. Todas1–12 y22–27 tienen renders temporales.
- TextoOCR/Poppler de27p y conversiónPyMuPDF4LLM completos en
  /tmp/fisica-ii-conversion/modelos-examenes-ocr; no prueban fidelidad por sí solos.
- PR sigueborrador; cuerpoactualizado explicita materia incompleta. No aprobar
  ni fusionar. Continuar luego teoría/documentos de otros años del inventario.

## Checkpoint 67: ocho exámenes escaneados adicionales preparados

- Hay90notas/1361math esperadas:82/1353ya verificadas en GitHub; ocho nuevas
  locales de páginas14temaB,16ambos,17ambos,18completa y19ambos.
- Figuras originales de cada nueva nota cotejadas; corregidos márgenes para
  no cortar datos. Último control check77pasó; check78incluye fuentes.md
  actualizado tras corregir estado de cobertura.
- Hallado y corregido helper temporal: agregación de varias notas ponía
  «dos secciones» y sobrescribía estado parcial de fuente1. Ahora1/66siguen
  parciales y cuentan25exámenes; separa páginas completas, parciales y
  carátulas/separadores. Fuente5tambiénparcial, igualdad de render no es cierre.
- No inferir valores de exámenes similares. Conservadas J=C.r frente aJ=C/r,
  «1ºPARCIAL» de fuente17aunque sean magnetismo/CA y circuitos diferentes.
- Próximo: publicar/verificar ocho nuevas y actualizar math_renderizada; seguir
  p15dosrecuperatorios y20dostemas,21dosversiones,14temaA, y pendientes5–9.
- Fuente1: completas3,4,10,11,12,16,17,18,19,22,23,25,26,27; parciales5,6,7,14.
  Carátula1 y separadores2,13,24cotejados. Resto de la materia aún pendiente.

## Checkpoint 68: texto impreso del compilado de27p completo

-105notas/1400math esperadas.97/1370verificadas en GitHub; ocho notas finales
  locales pasan check85. Próximo publicar y verificar esas ocho antes de seguir.
- Fuente1:39exámenes/versiones y nota de carátula/índice. Todas27páginas
  cotejadas, con las variantes y sus figuras separadas. Índice conserva portada
  y separadores2/13/24. Total acumulado274páginas únicas de fuentes cotejadas
  visualmente (247previas +27del compilado); no usar suma285de helper porque
  cuenta páginas repetidas entre notas.
- Amplificación correcta resolvió Q1p5:exponente−8, no−9; conservado recorte
  original en recursos y notaIQtemaA. Q2imprime10-9enlínea: no convertirlo
  silenciosamente a superíndice. Ejercicios5–8delrecuperatoriop6 conservan
  ncoul para λ sin añadir/m y numeración5–8.
- Permanece una unidad manuscrita de R en p14sinlectura inequívoca; recorte
  original conservado y pendiente explícito en nota/coverage/inventario.
- Próximo: verificar ocho nuevas en GitHub; revisar resultado readonly de
  buscar-duplicados-pdf.py (sesión6884) que calcula hashes de render de todos
  PDFs sin modificar originales, para identificar versiones realmenteiguales.
- PR sigueborrador. La materia aún tiene teoría y material2019/2020pendientes;
  este cierre cubre solo el texto impreso del compilado, no toda FísicaII.

## Checkpoint 69: unidad1teórica completa en local

-116notas/1478math esperadas.105/1400confirmadas en GitHub. Once notas teóricas
  nuevas de fuente74 cubren sus41páginas; fuente75SHAidéntica compartecontenido.
-315páginas únicas de fuentes cotejadas visualmente (274previas +41unidad1).
  La suma326del helper repite páginas por notas; no usarla como revisión única.
- Unidad1: fuerza/superposición1–6; definicióncampo7–10; puntuales11–13;
  hilo/plano14–15; líneas16–22; movimiento23; ángulosólido24–25; flujo26–29;
  Gauss30–31; aplicaciones32–38+41; diferencial39–40. La41solo tiene diagrama,
  no era blanca. Figuras y etiquetas revisadas; dos diagramas de38 y el39 se
  extraen del objeto raster original para evitar restos de texto ajeno.
- Página27 superpone animaciones22/45/90 ycasogeneral: fórmulas completas
  recuperadas desdecapatextual yrecorteconservado; x/asteriscos/superíndice0
  originales mantenidos. Índiceserróneos ysumatorias documentados sincorregir.
- Docling --enrich-formula muestra2–4 terminó370s y produjo expresiónespuria,
  omisiones y textoenfórmulas; no se aceptó esa salida. PyMuPDF4LLM conserva
  imágenes peroomiteLaTeX. Todoslosbloques fueron cotejadosvisualmente.
- Comparaciónreadonly102PDF/2217p terminó sinerrores; no hay copias porpágina
  adicionales hacia fuentescompletas fuera de gruposyaidentificados.
- Nuevaprueba de renders:52↔4(13p),112↔113(13p),127↔132(32p). Solo4comparte
  material ya transcrito;112/113y127/132siguenpendientesjuntoas referencia.
  No sumaridentidadpixelcomorevisiónmanual. Prueba ampliada en duplicados-render.
- check91pasó las11notas yfuentes2015/2019; diff --checkpendientealcommit.
  Próximo publicar y verificar1478esperadas, especialmenteoiint enGitHub;
  luego seguirinventariopendiente, sin aprobar ni fusionarPR.

## Checkpoint 70: verificación de la unidad teórica publicada

- 116 notas y 1478 expresiones verificadas en GitHub; 315 páginas únicas
  cotejadas visualmente. Las 24 imágenes de la unidad 1 cargaron correctamente.
- GitHub mostraba literalmente la macro oiint aunque KaTeX la aceptaba.
  Se sustituyó por el símbolo Unicode de integral de superficie cerrada dentro
  de mathop, conservando el significado original; ambas notas verificadas.
- CI del commit 6bc9831 pasó. PR sigue en borrador y materia incompleta.
- Búsqueda de PR abiertos: Física II #1 y control .github #13 de correlativas
  ISI Plan 2023; no aparecieron PR de otras materias.
- Próxima fuente: 89, Energía electrostática y potencial eléctrico, 16 páginas.
