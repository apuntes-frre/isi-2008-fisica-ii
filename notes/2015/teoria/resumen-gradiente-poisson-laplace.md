# Resumen de Física II — gradiente, Poisson y Laplace

## El campo eléctrico como gradiente de potencial eléctrico

El campo eléctrico E y el potencial eléctrico V están estrechamente
relacionados, por lo tanto, se puede calcular el valor del campo eléctrico en
una región específica si el potencial eléctrico se conoce. Como

```math
\begin{aligned}\int_a^b dV&=V_b-V_a=-\int_a^b\vec E\,d\vec s\\-dV&=\vec E\,d\vec s\\\vec E&=-\frac{dV}{d\vec s}\end{aligned}
```

Si escribimos E en términos de vectores unitarios nos queda

```math
\vec E=-\left(\frac{\partial V}{\partial x}i+\frac{\partial V}{\partial y}j+\frac{\partial V}{\partial z}k\right)
```

En notación vectorial nos quedaría

```math
\vec E=-\vec\nabla\cdot V
```

donde $`\vec\nabla\cdot V`$ representa el gradiente de potencial. En cada punto,
el gradiente de potencial apunta en la dirección en la que V aumenta con más
rapidez con un cambio de posición. Por consiguiente, en cada punto la dirección
de E es la dirección en laque V disminuye mas rápidamente y siempre es
perpendicular a la superficie equipotencial.

Una superficie equipotencial es cualquier superficie formada por una
distribución continua de puntos con el mismo potencial eléctrico, y son
perpendiculares a las líneas de campo.

## Ecuaciones de Poisson y de Laplace

El campo eléctrico para distribuciones de cargas en reposo satisface las
siguientes propiedades.

```math
\nabla\cdot\vec E=\frac\rho{\epsilon_0}
```

```math
\vec E=-\vec\nabla\cdot V
```

Es posible reunir estas dos propiedades

```math
\nabla\cdot(-\nabla V)=-\frac\rho{\epsilon_0}
```

```math
\nabla^2\cdot V=\frac\rho{\epsilon_0}
```

que se conoce como ecuación de Poisson y se puede escribir como:

```math
\frac{\partial^2V}{\partial x^2}+\frac{\partial^2V}{\partial y^2}+\frac{\partial^2V}{\partial z^2}=\frac\rho{\epsilon_0}
```

Si en la región no hay carga la expresión se reduce a la ecuación de Laplace.

```math
\nabla^2\cdot V=0
```

```math
\frac{\partial^2V}{\partial x^2}+\frac{\partial^2V}{\partial y^2}+\frac{\partial^2V}{\partial z^2}=0
```

Vamos a obtener la ecuación en diferencia finita equivalente a la de Laplace en
dos dimensiones. Para ello suponemos que la función potencial eléctrico puede
ser desarrollada en serie de Taylor alrededor de un punto (x,y) entonces

```math
\Phi(x+h,y)\cong\Phi(x,y)+h\frac{\partial\Phi(x,y)}{\partial x}+\frac{h^2}2\frac{\partial^2\Phi(x,y)}{\partial x^2}\tag{1}
```

```math
\Phi(x-h,y)\cong\Phi(x,y)-h\frac{\partial\Phi(x,y)}{\partial x}+\frac{h^2}2\frac{\partial^2\Phi(x,y)}{\partial x^2}\tag{2}
```

sumando (1) y (2) y agrupando, obtenemos

```math
\frac{\partial^2\Phi(x,y)}{\partial x^2}=\frac{\Phi(x+h,y)-2\Phi(x,y)+\Phi(x-h,y)}{h^2}\tag{3}
```

de igual manera se obtiene la derivada segunda para y

```math
\frac{\partial^2\Phi(x,y)}{\partial y^2}=\frac{\Phi(x,y+h)-2\Phi(x,y)+\Phi(x,y-h)}{h^2}\tag{4}
```

sumando ahora la (3) y la (4) resulta

```math
\frac{\partial^2\Phi(x,y)}{\partial x^2}+\frac{\partial^2\Phi(x,y)}{\partial y^2}=\frac{\Phi(x+h,y)-4\Phi(x,y)+\Phi(x-h,y)+\Phi(x,y+h)+\Phi(x,y-h)}{h^2}=0
```

de donde se despeja la función potencial Φ(x,y) resultando

```math
\Phi(x,y)\cong\frac{\Phi(x+h,y)+\Phi(x-h,y)+\Phi(x,y+h)+\Phi(x,y-h)}4
```

El potencial en un punto es el promedio de los potenciales en los puntos
circundantes.

## Procedencia y erratas conservadas

- Original: `2015/Resumen-Fisca-2.pdf`, página10 desde el gradiente y página11
  completa. SHA-256:
  `b9903f972224365c1a74b5d2732c9a34675c9b719da4c9c2d28e4a0f34e0b0cc`.
- PyMuPDF4LLM, Poppler y cotejo visual completo. Fórmulas originales de imagen
  transcritas como LaTeX, con numeración1–4 y puntos de multiplicación
  conservados.
- Se preservan el divisor vectorial dV/ds y el punto entre ∇ y V. La ecuación
  intermedia contiene −ρ/ε0 pero la forma final de Poisson lleva +ρ/ε0; se
  conservan ambos signos y no se corrigen silenciosamente.
- El texto escribe «laque» y «mas»; el paso de Taylor usa Φ en lugar de V y los
  signos de aproximación del original se conservan. No se añaden términos de
  resto.
