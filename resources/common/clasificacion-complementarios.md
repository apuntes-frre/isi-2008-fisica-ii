# Clasificación de fuentes complementarias

Revisión del 23/10/2026. Se conservan los originales y sus SHA-256 en el
inventario. La clasificación determina el alcance de la transcripción; no
significa que se haya transcrito el curso externo o ejecutado sus programas.

## CD de Física II de 2016

Original: `2015/CD -Física II FRReUTN- 2016.rar`. SHA-256:
`b537fe44a2a9866f53bf0781b26e5810921214fee85883d88b43a690e581486c`. Se extrajo
una copia con bsdtar y se leyeron los miembros del ZIP anidado sin cargar
applets. Los 11.319 archivos coinciden por SHA-256 con el inventario histórico;
no hay diferencias.

| Grupo | Archivos | Alcance |
| -- | -: | -- |
| Documentos docentes de la raíz | 11 | Duplicados exactos de fuentes canónicas ya inventariadas; heredan su cobertura y sus lecturas pendientes. |
| `fisica/`, dentro de `utilitarios/fisica.zip` | 11.252 | Curso externo de referencia y simulación; identidad comprobada, no transcrito íntegramente. |
| Paquetes y archivos de software restantes | 56 | Inventariados y cotejados por hash, sin ejecutar. |
| Total | 11.319 | Tres grupos disjuntos que cubren todo el inventario. |

El curso es **Física con ordenador. Curso Interactivo de Física en Internet**,
de **Ángel Franco García**, según `fisica/default.htm` y
`fisica/Introduccion/autor/AUTOR.HTM`. El índice abarca física general, desde
cinemática hasta mecánica cuántica, y describe simulaciones Java. Ya está citado
como recurso complementario en
[direcciones útiles](../../notes/2015/teoria/direcciones-utiles-internet-simulaciones.md).
Su identificación no convierte las páginas del sitio externo en nuevas guías de
la cátedra.

El detalle de los once duplicados y los criterios de clasificación están en
[clasificacion-contenedores.json](clasificacion-contenedores.json).
[contenedores.json](contenedores.json) conserva el inventario de extracción
histórico; sus estados antiguos de revisión se interpretan con esta
clasificación.

## Dos planillas de temas de cálculo

`2015/Extras/DOC-20161031-WA0003.xlsx` y `2015/Extras/DOC-20161109-WA0005.xlsx`
son duplicados exactos, con SHA-256
`33458cb3f2e1ab86f92df0cb13f05129c52871068c5882ee22497b9f7ab037f7`.

La lectura directa de su XML identifica una sola hoja, `Hoja1`, rango `B3:E34`,
32 filas, 124 celdas y 29 fórmulas. Tiene columnas **Sección**, **Tema**,
**Veces** y **Porcentaje**. Las secciones son **Límites**,
**Derivadas/Diferencial**, **Aplicaciones del Cálculo Diferencial** e
**Integrales**. Incluye, entre otros, Rolle, Lagrange, Cauchy, Barrow y
L'Hôpital. La planilla dice «Actualizado al 02/08/2016».

Se clasifica como estadística de temas de cálculo diferencial e integral, ajena
al contenido de Física II. No se atribuye a una asignatura exacta: no aparece un
título que la identifique. No se publica como apunte de esta materia.
