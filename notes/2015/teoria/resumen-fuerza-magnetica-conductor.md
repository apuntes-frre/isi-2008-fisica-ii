# Resumen de Física II — fuerza magnética sobre conductores

Consideremos un segmento recto de alambre de longitud L y de área de sección
transversal A, que conduce una corriente I en un campo magnético uniforme B. La
fuerza magnética que se ejerce sobre una carga q en movimiento, con una
velocidad de arrastre $`v_d`$ , es igual a $`qv_d\times B`$ . Ya que el volumen
del segmento es AL, el número de cargas en el segmento es igual a nAL, siendo n
el número de cargas por unidad de volumen. Por esto, la fuerza magnética total
sobre el alambre de longitud L es

```math
\vec F_B=(q\vec v_d\times\vec B)nAL
```

Como la corriente en el alambre es igual a I= nqvdA

```math
\vec F_B=I\vec L\times\vec B
```

donde L es un vector que apunta en la dirección de la corriente I y que tiene
una magnitud igual a la longitud L del segmento. Observe que esta expresión se
aplica sólo a un segmento de alambre recto en un campo magnético uniforme.

Ahora considere un segmento de alambre de forma arbitraria de sección
transversal uniforme en un campo magnético, según se observa en la figura 29.18.
De la ecuación 29.10 se concluye que la fuerza magnética que se ejerce sobre una
longitud dsde un pe-queño segmento de vector en presencia de un campo B es igual
a

```math
d\vec F_B=I\,d\vec s\times\vec B
```

Para calcular la fuerza total $`F_B`$ que actúa sobre el alambre, se integra por
toda la longitud del alambre. Donde a y b representan los puntos extremos del
alambre.

```math
\vec F_B=I\int_a^b\overrightarrow{ds}\times\vec B=I(l_b-l_a)\times\vec B
```

Como podemos ver, la fuerza sobre el conductor depende de la longitud entre los
puntos a y b.

## Procedencia y observaciones

- Original: `2015/Resumen-Fisca-2.pdf`, páginas [29]; sectores delimitados por
  encabezados. SHA-256:
  `b9903f972224365c1a74b5d2732c9a34675c9b719da4c9c2d28e4a0f34e0b0cc`.
- PyMuPDF4LLM, Poppler y cotejo visual completo de los sectores; ecuaciones de
  imagen transcritas a LaTeX, figuras originales preservadas.
- Se preservan las referencias a figura29.18 y ecuación29.10, que no se
  reproducen aquí, y «dsde un pe-queño» del texto. La resta lb−la aparece sin
  flechas en el original.
