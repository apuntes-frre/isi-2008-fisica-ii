# Resumen de Física II — energía del inductor y densidad de energía magnética

## Energía almacenada en el campo de inducción magnética de una bobina

En un circuito LR parte de la energía suministrada por la batería aparece como
energía interna en la resistencia del circuito en tanto que la energía restante
es almacenada en el campo magnético del inductor. Si multiplicamos cada uno de
los términos de la ecuación $`\mathcal E-IR-L(dI/dt)`$ por I y reordenamos la
expresión,

```math
I\mathcal E=I^2R+LI\frac{dI}{dt}
```

Reconocemos IƐ como la rapidez a la cual la energía se suministra por la
batería, $`I^2R`$ como la rapidez a la cual se entrega energía al resistor y
LI(dI/dt) como la rapidez a la cual se almacena energía en el inductor. Si U
representa la energía almacenada en el inductor en cualquier instante, se puede
escribir la relación dU/dt con la cual se almacena energía de la forma

```math
\frac{dU}{dt}=LI\frac{dI}{dt}
```

Para determinar la energía total almacenada en el inductor en cualquier
instante, rescriba esta expresión de la forma $`dU=LI\,dI`$ e integre:

```math
U=\int dU=\int_0^I LI\,dI=L\int_0^I I\,dI
```

```math
U=\tfrac12LI^2
```

donde L es constante y ha sido retirada de la integral. La ecuación representa
la energía almacenada en el campo magnético del inductor cuando la corriente es
igual a I.

## Densidad de energía

Considere un solenoide cuya inductancia se conoce por la ecuación:

```math
L=\mu_0n^2V
```

donde n=N/ _l_ es el número de vueltas por unidad de longitud y V =A _l_ es el
volumen interior del solenoide.

El campo magnético de un solenoide es:

```math
B=\mu_0nI
```

Al sustituir la expresión para L y para $`I=B/\mu_0n`$ en la ecuación
$`U=\frac12LI^2`$, obtiene

```math
U=\tfrac12LI^2=\tfrac12\mu_0n^2V\left(\frac B{\mu_0n}\right)^2=\frac{B^2}{2\mu_0}V
```

La densidad de energía magnética, o la energía almacenada por cada unidad de
volumen en el campo magnético del inductor, es igual a

```math
u_B=\frac UV=\frac{B^2}{2\mu_0}
```

Esta expresión se aplica para cualquier región del espacio en el que exista un
campo magnético.

## Procedencia y observaciones

- Original: `2015/Resumen-Fisca-2.pdf`, páginas [40, 41]; sectores delimitados
  por encabezados. SHA-256:
  `b9903f972224365c1a74b5d2732c9a34675c9b719da4c9c2d28e4a0f34e0b0cc`.
- PyMuPDF4LLM, Poppler y cotejo visual completo de los sectores; ecuaciones de
  imagen transcritas a LaTeX, diagramas originales preservados.
- Se conserva la expresión de partida del párrafo sin añadirle =0. Se restituyen
  las fórmulas y el texto embebidos en la imagen de sustitución de página41.
