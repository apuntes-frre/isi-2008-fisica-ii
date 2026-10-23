# Resumen de Física II — ecuación de continuidad

La densidad de corriente J y la densidad de carga ρ, en una región no son
cantidades independientes, sino que están relacionadas en cada punto por una
ecuación diferencial, llamada ecuación de la continuidad. Esta relación se basa
en el principio de conservación de la carga. Dada una superficie arbitraria
cerrada S, la corriente eléctrica que entra en el volumen V encerrado, está dada
por

```math
I=\frac{dQ}{dt}=-\oiint_{sc}\vec J\cdot d\vec S
```

El signo menos es porque el versor superficie es siempre hacia afuera y se desea
considerar que I es positiva cuando el flujo neto de carga es del exterior de V
hacia su interior. Empleando el teorema de la divergencia se puede escribir:

```math
\oiint_{sc}\vec J\cdot d\vec S=\iiint_V\nabla\cdot\vec J\,dV
```

Por otro lado se tiene

```math
I=\frac{dQ}{dt}=\frac d{dt}\iiint_V\rho(x,y,z,t)\,dV=\iiint_V\frac{\partial\rho}{\partial t}\,dV
```

La última integral es válida porque se toma un volumen fijo y la derivada
temporal actúa solo sobre la función ρ(x,y,z,t), de modo que cuando la derivada
se introduce dentro de la integral, ésta se convierte en una derivada parcial
respecto del tiempo. Reuniendo las dos expresiones anteriores resulta

```math
\iiint_V\frac{\partial\rho}{\partial t}\cdot dV=-\iiint_V\nabla\cdot\vec J\,dV
```

Lo cual puede reescribirse

```math
\iiint_V\left(\frac{\partial\rho}{\partial t}+\nabla\cdot\vec J\right)dV=0
```

Pero como el volumen V es completamente arbitrario, entonces la única forma que
se cumpla es que el integrando se anule, esto es:

```math
\frac{\partial\rho}{\partial t}+\nabla\cdot\vec J=0
```

## Procedencia y observaciones

- Original: `2015/Resumen-Fisca-2.pdf`, páginas [19]; sectores delimitados por
  encabezados. SHA-256:
  `b9903f972224365c1a74b5d2732c9a34675c9b719da4c9c2d28e4a0f34e0b0cc`.
- PyMuPDF4LLM, Poppler y cotejo visual completo de los sectores; fórmulas de
  imagen transcritas a LaTeX y figuras originales preservadas.
- Se conserva el punto de producto ante dV en la igualdad de integrales y la
  notación sc del original.
