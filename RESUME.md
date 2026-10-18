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
