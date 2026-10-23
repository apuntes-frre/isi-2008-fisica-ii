# Resumen de Física II — entropía

La entropía es una variable de estado, relacionada con la segunda ley de la
termodinámica, esta surge de estudios que hallaron que los sistemas aislados
tienden hacia el desorden, siendo la entropía una medida de este desorden. Un
micro-estado es una configuración particular de los componentes individuales del
sistema, mientras que un macro-estado es una descripción de las condiciones del
sistema desde un punto de vista macroscópico como presión, densidad y
temperatura.

La entropía en termodinámica involucra la transferencia de energía por calor
durante un proceso reversible. Considere cualquier proceso infinitesimal en el
que un sistema cambia de un estado de equilibrio a otro. Si $`dQ_r`$ es la
cantidad de energía transferida por calor cuando el sistema sigue una
trayectoria reversible entre los estados, el cambio en entropía dS es igual a
esta cantidad de energía para el proceso reversible dividida entre la
temperatura absoluta del sistema:

```math
dS=\frac{dQ_r}T
```

Se considera que la temperatura es constante porque el proceso es infinitesimal.
dS solo depende de los extremos, es independiente de la trayectoria real
seguida. Por lo tanto, el cambio en entropía para un proceso irreversible se
determina al calcular el cambio de entropía para un proceso reversible que
conecta los mismos estados inicial y final. Cuando el sistema absorbe energía,
dQr es positiva y la entropía del sistema aumenta, si el sistema expulsa
energía, dQr es negativa y la entropía del sistema disminuye.

Cuando calculamos el cambio en entropía para un proceso finito, por lo general T
no es constante. En consecuencia, debemos integrar:

```math
\Delta S=\int_i^f dS=\int_i^f\frac{dQ_r}T
```

el cambio en entropía $`\Delta S`$ de un sistema que va de un estado a otro es
independiente de la trayectoria, y solo depende del estado inicial y final.

## Procedencia y observaciones

- Original: `2015/Resumen-Fisca-2.pdf`, páginas [80]; sectores delimitados por
  encabezados. SHA-256:
  `b9903f972224365c1a74b5d2732c9a34675c9b719da4c9c2d28e4a0f34e0b0cc`.
- PyMuPDF4LLM, Poppler y cotejo visual completo de los sectores; ecuaciones de
  imagen transcritas a LaTeX, figuras originales preservadas.
- Se conservan las definiciones, el diferencial reversible y la integral entre
  estados, sin agregar desarrollos externos.
