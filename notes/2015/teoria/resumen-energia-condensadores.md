# Resumen de Física II — energía en condensadores y campos eléctricos

Suponga que q es la carga del capacitor en un determinado instante durante el
proceso de carga. En ese mismo momento, la diferencia de potencial a través del
capacitor es V=q/C. El trabajo necesario para transferir un incremento de carga
dq de la placa que tiene una carga -q a la placa que tiene una carga q es

```math
dW=\Delta V\,dq=\frac qC\,dq
```

El trabajo total requerido para cargar el capacitor desde q=0 hasta una carga
final q=Q es

```math
W=\int_0^Q\frac qC\,dq=\frac1C\int_0^Q q\,dq=\frac{Q^2}{2C}
```

El trabajo invertido al cargar el capacitor se presenta como una energía
potencial eléctrica U almacenada en el mismo. Es posible expresar la energía
potencial almacenada en el capacitor con carga como (1)

```math
U=\frac{Q^2}{2C}=\frac12Q\Delta V=\frac12C(\Delta V)^2
```

Este resultado es aplicable a cualquier capacitor, sea cual fuere su geometría.
En la práctica, existe un límite para la energía (o carga) máxima que se puede
almacenar, ya que en un valor lo suficientemente grande de V ocurrirá finalmente
una descarga entre las placas. Consideramos la energía almacenada en un
capacitor como si estuviera almacenada en el campo eléctrico producido entre las
placas al cargar el capacitor. Esta descripción es aceptable porque el campo
eléctrico es proporcional a la carga del capacitor. En el caso de un capacitor
de placas paralelas, la diferencia de potencial está relacionada con el campo
eléctrico mediante la correspondencia V=Ed. Además, su capacitancia es
$`C=e_0A/d`$ . Si sustituye estas expresiones en (1), obtiene

```math
U=\frac12\frac{\epsilon_0A}d(E^2d^2)=\frac12(\epsilon_0Ad)E^2
```

En vista de que el volumen ocupado por el campo eléctrico es Ad, la energía por
cada unidad de volumen $`u_E=U/Ad`$ , conocida como densidad de energía, es

```math
u_E=\frac12\epsilon_0E^2
```

Esta expresión es válida de manera general, independientemente de la fuente del
campo eléctrico. Es decir, la densidad de energía en cualquier campo eléctrico
en un punto dado es proporcional al cuadrado de la magnitud del campo eléctrico.

## Procedencia y observaciones

- Original: `2015/Resumen-Fisca-2.pdf`, página14 desde «Energía» hasta
  «Dieléctricos». SHA-256:
  `b9903f972224365c1a74b5d2732c9a34675c9b719da4c9c2d28e4a0f34e0b0cc`.
- PyMuPDF4LLM, Poppler y cotejo visual de todo el sector. Cinco ecuaciones de
  imagen transcritas como LaTeX; fórmulas en línea cotejadas con el original.
- Se mantienen las referencias(1), la notación e0 del texto frente a ε0 de las
  fórmulas y U/Ad sin añadir paréntesis al cociente lineal del original.
