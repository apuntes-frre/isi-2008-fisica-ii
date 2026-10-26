# Registro de correcciones y anotaciones de Física II

Este archivo está en la raíz de la materia, junto a README.md. Permite localizar
las intervenciones editoriales y los límites de lectura acordados durante la
transcripción. Estado documentado: cierre del 25/10/2026; registro preparado el
26/10/2026. Las decisiones de contenido siguientes fueron cotejadas y aceptadas
por el usuario. Los recortes originales permanecen junto a cada apunte.

## Índice de fragmentos intervenidos

| Apunte | Fragmento | Intervención |
| -- | -- | -- |
| [Ciclotrón](notes/2019/teoria/ciclotron-variante-impresa-2019.md#ciclotron) | Diapositiva 26; fórmulas de radio, velocidad y energía | Corrección editorial de fórmula y notación; aclaración con asterisco. |
| [Trayectoria helicoidal](notes/2019/teoria/demostracion-helicoidal-variante-impresa-2019.md#diapositiva-40) | Diapositiva 40; fuerza, determinante y ecuaciones (1)–(4) | Notación vectorial, producto vectorial y delimitadores normalizados. |
| [Trayectoria helicoidal](notes/2019/teoria/demostracion-helicoidal-variante-impresa-2019.md#diapositiva-41) | Diapositiva 41; solución, condiciones iniciales y referencia a (5) | Notación normalizada y referencia expresada mediante su relación matemática. |
| [Trayectoria helicoidal](notes/2019/teoria/demostracion-helicoidal-variante-impresa-2019.md#diapositiva-42) | Diapositiva 42; ecuaciones (12)–(17), especialmente (13) | Coeficientes corregidos y delimitadores normalizados. |
| [Examen ISI, tema A](notes/2015/practica/isi-recuperatorio-segundo-parcial-tema-a.md#problema-4) | Problema 4; radio manuscrito de la espira | Lectura elegida de 5 m con aclaración de posible 5 cm. |
| [Kirchhoff: hoja de datos](notes/2015/practica/kirchhoff-informe-grupo-6-hoja-datos.md#verificaci%C3%B3n-de-las-leyes-de-malla) | Tabla de mallas; cuatro celdas | Se mantiene `[ilegible]` y se conserva imagen nativa. |
| [Brújula: hoja de datos](notes/2015/practica/brujula-informe-grupo-6-hoja-datos.md#1--recolecci%C3%B3n-de-datos) | Fila de 30° y radio medio del encabezado | Lecturas confirmadas: 0,0945 m y 0,0275 m. |
| [Fuerza sobre corriente: hoja de datos](notes/2015/practica/fuerza-corriente-informe-grupo-6-hoja-datos.md#1--recolecci%C3%B3n-de-datos) | Densidad y anotación inferior de masa | Versión principal elegida; rótulo ilegible y símbolo no identificado omitidos. |

## Detalle de las correcciones y sus anotaciones

### Ciclotrón: energía en función del campo magnético y el radio

Fuente: `2019/2do Parcial/UT 5 4 pag.pdf`, página PDF 7, casillero 2,
diapositiva 26. Segunda impresión: `UT 5 6 pag.pdf`, página 5, casillero 2.

- El original muestra `v²` en el numerador de la expresión final de energía y
  varios glifos mal renderizados. Se corrigió ese factor a `B²`.
- Se despeja `v = qBR/m` y se sustituye en `Ec = mv²/2`. El resultado final
  conserva el radio: `Ec = q²B²R²/(2m)`.
- La flecha entre el radio y la velocidad y los paréntesis de la sustitución son
  notación editorial legible, no glifos recuperados del PDF.
- El apunte contiene una aclaración marcada con `*`, que explica la errata y la
  interpretación. La sustitución inversa del radio se retiró porque devolvía la
  expresión inicial, en lugar de obtener la energía en función de B y R.

[Recorte original del ciclotrón](resources/2019/fuerzas-magneticas-variante-impresa/diapositiva-26-deteriorada.png).

### Trayectoria helicoidal: diapositiva 40

Fuente: `UT 5 4 pag.pdf`, página PDF 10, casillero 4; `UT 5 6 pag.pdf`, página
7, casillero 4.

- Las marcas `fi` sobre F, v, B y a se transcribieron como flechas vectoriales.
- El punto entre v y B se normalizó como producto vectorial: la ecuación inicial
  expresa la fuerza magnética igualada a la fuerza neta de Newton.
- Se normalizaron los versores, las barras del determinante de tres filas y los
  paréntesis que elevan al cuadrado el cociente `qBz/m` en (4).
- Se conservaron las etiquetas (1)–(4). Se añadieron enlaces explicativos entre
  las operaciones para que el desarrollo se entienda sin mirar la imagen.
- Por indicación del usuario, esta normalización no lleva aclaración al pie;
  queda registrada en la procedencia del apunte y en este archivo.

[Recorte original de la diapositiva 40](resources/2019/fuerzas-magneticas-variante-impresa/diapositiva-40-deteriorada.png).

### Trayectoria helicoidal: diapositiva 41

Fuente: `UT 5 4 pag.pdf`, página PDF 11, casillero 1; `UT 5 6 pag.pdf`, página
7, casillero 5.

- Se normalizaron la flecha de implicación, el vector de velocidad inicial, los
  versores y la presentación de los grupos de condiciones iniciales y solución.
- El texto original cita una ecuación (5), cuyo número no se distingue junto a
  la relación correspondiente en la diapositiva anterior. Se escribió «la
  relación para la componente de la velocidad» y se conserva la expresión
  `vy = m/(qBz) · dvx/dt`, sin inventar una nueva etiqueta (5).
- Las soluciones y las condiciones iniciales se conservaron; las ecuaciones
  (9)–(11) fueron cotejadas con el usuario mediante captura.

[Recorte original de la diapositiva 41](resources/2019/fuerzas-magneticas-variante-impresa/diapositiva-41-deteriorada.png).

### Trayectoria helicoidal: diapositiva 42

Fuente: `UT 5 4 pag.pdf`, página PDF 11, casillero 2; `UT 5 6 pag.pdf`, página
7, casillero 6.

- En (13), el original intercambia los coeficientes de los términos con coseno y
  seno. Se corrigió a `y(t) = (v₀ₓ/ω)[cos(ωt) − 1] + (v₀ᵧ/ω)sin(ωt)`.
- La corrección integra la velocidad de (10) y concuerda con la circunferencia
  de (15). El usuario la autorizó tras comparar la captura y las expresiones.
- Se normalizaron los paréntesis y exponentes de (15), y los paréntesis del
  centro en (16). Se conservó el radio de (17).
- La explicación de (15) indica reordenar las coordenadas, elevar al cuadrado y
  sumar miembro a miembro. La procedencia registra la corrección de (13).

[Recorte original de la diapositiva 42](resources/2019/fuerzas-magneticas-variante-impresa/diapositiva-42-deteriorada.png).

### Examen: radio manuscrito con unidad dudosa

Fuente: compilado de modelos de examen, página PDF 14, examen superior ISI,
recuperatorio del segundo parcial, tema A, problema 4.

- Se incorporó `R = 5 m`, lectura elegida por el usuario tras revisar el
  ejercicio completo de espira junto a conductor recto.
- El asterisco del dato remite a una aclaración al pie: la unidad manuscrita no
  es inequívoca y podría ser `cm`. La elección de metros no confirma la unidad
  original ni se deduce de una solución del ejercicio.

[Anotación original del radio](resources/2015/modelos-examenes/isi-recuperatorio-segundo-parcial-tema-a-anotacion.png).

### Kirchhoff: conservación de lecturas no recuperadas

Fuente: `2015/L6 Kirchoff G6 Aprobado.pdf`, página PDF 5 de 20.

- Posición 1: Vcd, Veb y Vgb permanecen como `[ilegible]`.
- Posición 3: Vcd permanece como `[ilegible]`.
- Tras comparar original y propuestas de ambos agentes, el usuario eligió
  conservar la fotografía y no adoptar aproximaciones. No se rellenaron celdas
  desde la tabla mecanografiada posterior ni se ajustaron mediciones para
  obtener un porcentaje de error determinado.
- Se añadió el PNG nativo de mallas de 497 × 85 píxeles: recorte sin reescalado
  de la foto incrustada de 533 × 350, con identidad de píxeles verificada. Las
  fotos JPEG exactas y sus hashes se conservan también en caché local; el PDF
  original está intacto en OneDrive. El apunte documenta esta decisión.

[Tabla original ampliada](resources/2015/kirchhoff-informe-grupo-6/hoja-datos-mallas.png)
y
[tabla con píxeles nativos](resources/2015/kirchhoff-informe-grupo-6/hoja-datos-mallas-nativa.png).

### Brújula: cifra sobreescrita y radio medio

Fuente: `2015/L7 Brujula G6 A corregir.docx`, página 6 del PDF normalizado. La
hoja fotografiada tiene su propia numeración 1.

- La celda X (m) para 30° pasó de `0,09[ilegible]` a `0,0945`, lectura
  confirmada por el usuario después de comparar original, principal y subagente.
- Se confirmó el radio medio como `0,0275 m`; no se adoptó la lectura
  alternativa `0,075 m` del subagente. El valor del radio ya figuraba así en el
  apunte.
- La tabla mecanografiada posterior conserva `0,094 m`: ambas versiones se
  mantienen diferenciadas. No se recalcularon sus resultados para igualarlas.
- La anotación de procedencia registra ambas confirmaciones. Las columnas
  originalmente vacías y los ceros finales de otras distancias se preservaron.

[Tabla manuscrita original de brújula](resources/2015/brujula-informe-grupo-6/hoja-datos-tablas.png).

### Fuerza sobre corriente: versión elegida y omisiones autorizadas

Fuente: `2015/L8 Fza sobre elemento de cte G6 Aprobado.pdf`, página PDF 7 de 9.

- El usuario eligió la versión del agente principal: `a = 0,065 m`,
  `b = 0,1 cm`, densidad `μ = 0,0326`, corriente de la lectura 3 `0,82` y
  anotaciones marginales `13° — 2,29` y `10° — 1,49`.
- Se quitó la marca `[símbolo no representado]` de la línea de densidad y el
  rótulo parcialmente ilegible de la masa. Quedan `Densidad μ = 0,0326` y
  `Masa: 7,5 g`, sin inventar el símbolo ni expandir el rótulo.
- Se conservan `L = a + b + a` y `μ = m/L =`, con su resultado sin completar.
- Se preservaron las diferencias del original: unidad `cm` junto a b frente a
  `m` en los resultados posteriores; encabezado «Ángulo (radianes)» frente a
  mediciones en grados. No se convirtieron ni homogeneizaron los datos.
- La procedencia registra la elección y las omisiones autorizadas. Los recortes
  originales conservan la escritura que se decidió no reconstruir.

[Tabla y datos originales](resources/2015/fuerza-corriente-informe-grupo-6/hoja-tabla-mediciones.png)
y
[anotaciones inferiores originales](resources/2015/fuerza-corriente-informe-grupo-6/hoja-anotaciones.png).

## Reparaciones de presentación matemática

Para evitar que GitHub apilara verticalmente las ecuaciones numeradas, se
retiraron los comandos de etiqueta `\tag` del bloque matemático y se colocaron
los números como texto adyacente. Las fórmulas y los números de referencia se
conservaron. Esta reparación cambia la presentación, no los valores físicos.

Dos reparaciones iniciales:

- [Resumen: fuerza electromotriz](notes/2015/teoria/resumen-fuerza-electromotriz.md):
  etiqueta (1), expresión de la fuerza electromotriz con resistencia interna.
- [Resumen: gradiente, Poisson y Laplace](notes/2015/teoria/resumen-gradiente-poisson-laplace.md):
  etiquetas (1)–(4), desarrollo de Taylor y diferencias finitas.

La reparación posterior abarcó 222 etiquetas en los 31 apuntes siguientes. La
lista de etiquetas identifica los fragmentos afectados dentro de cada archivo;
algunas numeraciones se repiten entre secciones del mismo apunte.

- [Trabajo práctico Nº 17: Calorimetria](notes/2015/practica/calorimetria-laboratorio-17.md):
  etiquetas `1`.

- [Trabajo de laboratorio Nº 7: Campo de inducción magnética (compilado)](notes/2015/practica/campo-induccion-laboratorio-7-compilado.md):
  etiquetas `1, 2, 3, 4, 5, 6, 7, 8`.

- [Trabajo de laboratorio Nº 7: Campo de inducción magnética](notes/2015/practica/campo-induccion-magnetica-laboratorio-7.md):
  etiquetas `1, 2, 3, 4, 5, 6, 7, 8`.

- [Trabajo de laboratorio Nº 3: Estudio del regimen transitorio del circuito RC](notes/2015/practica/circuito-rc-capacidad-laboratorio-3.md):
  etiquetas
  `1, 2, 3, 4, 5, 6, 7, 8, 9, 11, 12, 13, 14, 15.a, 15.b, 16, 17, 18, 19, 20, 21`.

- [Trabajo de laboratorio Nº 3: Estudio del regimen transitorio del circuito RC (compilado)](notes/2015/practica/circuito-rc-laboratorio-3-compilado.md):
  etiquetas
  `1, 2, 3, 4, 5, 6, 7, 8, 9, 11, 12, 13, 14, 15.a, 15.b, 16, 17, 18, 19, 20, 21`.

- [Trabajo de laboratorio Nº 10: Circuito de corriente alterna - serie](notes/2015/practica/corriente-alterna-serie-laboratorio-10.md):
  etiquetas
  `1, 2, 3, 4, 5, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16.1, 16.2, 16.3, 17, 18`.

- [Trabajo práctico Nº 13: Estudio del fenómeno de difracción](notes/2015/practica/difraccion-laboratorio-13.md):
  etiquetas `1, 2, 3, 4`.

- [Trabajo de laboratorio Nº 2: Potencial eléctrico. Ecuación de Laplace](notes/2015/practica/ecuacion-de-laplace-laboratorio-2.md):
  etiquetas `1, 2, 3, 4, 5`.

- [Trabajo práctico Nº 14: Espectrómetro de red de difracción](notes/2015/practica/espectrometro-laboratorio-14.md):
  etiquetas `1`.

- [Trabajo de laboratorio Nº 9: Ley de Faraday. Coeficiente de induccion](notes/2015/practica/faraday-induccion-toroide-laboratorio-9.md):
  etiquetas `1, 2, 3, 4, 5, 6, 7, 8, 9, 10`.

- [Trabajo de laboratorio Nº 8: Fuerza magnetica sobre elementos de corriente (compilado)](notes/2015/practica/fuerza-magnetica-laboratorio-8-compilado.md):
  etiquetas `1, 2, 3, 4, 5, 6, 7, 8, 9`.

- [Trabajo de laboratorio Nº 8: Fuerza magnetica, versión del cuadernillo](notes/2015/practica/fuerza-magnetica-laboratorio-8-version-2.md):
  etiquetas `1, 2, 3, 4, 5, 6, 7, 8, 9`.

- [Trabajo de laboratorio Nº 8: Fuerza magnetica sobre elementos de corriente](notes/2015/practica/fuerza-magnetica-laboratorio-8.md):
  etiquetas `1, 2, 3, 4, 5, 6, 7, 8, 9`.

- [Trabajo práctico Nº 12: Estudio del fenómeno de interferencia](notes/2015/practica/interferencia-laboratorio-12.md):
  etiquetas `1, 2, 3, 4`.

- [Trabajo de laboratorio Nº 2: Potencial eléctrico. Ecuación de Laplace (compilado)](notes/2015/practica/laplace-laboratorio-2-compilado.md):
  etiquetas `1, 2, 3, 4, 5`.

- [Trabajo de laboratorio Nº 9 bis: Ley de Faraday, versión DOCX](notes/2015/practica/ley-de-faraday-laboratorio-9-bis-version-docx.md):
  etiquetas `1, 2, 3, 4, 5`.

- [Trabajo de laboratorio Nº 9 bis: Ley de Faraday](notes/2015/practica/ley-de-faraday-laboratorio-9-bis.md):
  etiquetas `1, 2, 3, 4, 5`.

- [Trabajo de laboratorio Nº 4: Ley de Ohm. Asociación de resistencias](notes/2015/practica/ley-de-ohm-asociaciones-laboratorio-4.md):
  etiquetas `1, 2, 3`.

- [Trabajo de laboratorio Nº 4: Ley de Ohm. Asociación de resistencias (compilado)](notes/2015/practica/ley-ohm-laboratorio-4-compilado.md):
  etiquetas `1, 2, 3`.

- [Trabajo de laboratorio Nº 1: Potencial eléctrico. Mapeo del campo eléctrico](notes/2015/practica/potencial-electrico-mapeo-laboratorio-1.md):
  etiquetas `1, 2, 3, 5, 6, 7, 8, 9, 10, 11, 12, 13`.

- [Trabajo de laboratorio Nº 1: Potencial eléctrico. Mapeo del campo eléctrico (compilado)](notes/2015/practica/potencial-laboratorio-1-compilado.md):
  etiquetas `1, 2, 3, 5, 6, 7, 8, 9, 10, 11, 12, 13`.

- [Trabajo práctico Nº 16: Termometría](notes/2015/practica/termometria-laboratorio-16.md):
  etiquetas `1`.

- [Campo cero de dos cargas puntuales](notes/2019/practica/campo-cero-dos-cargas-puntuales.md):
  etiquetas `1, 2`.

- [Campo de inducción magnética: informe experimental](notes/2019/practica/campo-induccion-magnetica-informe.md):
  etiquetas `1, 2, 3, 5, 6, 7`.

- [Discretizando un sistema contínuo para cálculos de campos de distribuciones continuas de carga](notes/2019/practica/discretizacion-sistema-continuo.md):
  etiquetas `1`.

- [Fuerza magnética sobre elementos de corriente: informe experimental](notes/2019/practica/fuerza-magnetica-elementos-corriente-informe.md):
  etiquetas `1, 2, 3, 4, 5, 6, 7, 9`.

- [Unidad Temática III: Capacidad. Propiedades Eléctricas de la Materia](notes/2019/teoria/capacidad-condensadores-definicion-unidades.md):
  etiquetas `1`.

- [Leyes de Kirchhoff](notes/2019/teoria/leyes-kirchhoff-mallas-nodos-teoria.md):
  etiquetas `1, 2, 3, 4, 5`.

- [Maxwell: deducción de la ecuación de ondas](notes/2019/teoria/maxwell-deduccion-ecuacion-ondas-2018-06-22.md):
  etiquetas `13, *, 14, 15, 16`.

- [Ecuaciones de Maxwell: formas integral y diferencial](notes/2019/teoria/maxwell-ecuaciones-integrales-diferenciales-2018-06-22.md):
  etiquetas `1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12`.

- [Maxwell: energía, balance y vector de Poynting](notes/2019/teoria/maxwell-energia-balance-poynting-2018-06-22.md):
  etiquetas `**`.

## Procedencia y alcance del registro

Las correcciones de contenido están en los PR
[#2](https://github.com/apuntes-frre/isi-2008-fisica-ii/pull/2) y
[#3](https://github.com/apuntes-frre/isi-2008-fisica-ii/pull/3), con sus
decisiones finales reflejadas arriba. Las 222 etiquetas se localizaron mediante
el diff del commit `70a01b4`; las dos reparaciones iniciales corresponden a
`4a37c88` y `373706c`. No se presentan como correcciones definitivas las
versiones intermedias que fueron descartadas.

Las erratas del original que se conservaron y las discrepancias entre versiones
se explican también en las secciones de procedencia de cada apunte. El
[inventario](resources/common/inventario.json) conserva nombres y hashes de las
fuentes; la [cobertura](resources/common/cobertura.json) registra páginas y
verificación de GitHub; la
[auditoría](resources/common/auditoria-transcripcion.md) resume las reservas del
cierre. Este registro no sustituye las imágenes fuente ni declara recuperados
los fragmentos ilegibles.
