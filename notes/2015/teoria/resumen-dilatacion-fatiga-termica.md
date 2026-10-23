# Resumen de Física II — dilatación y fatiga térmica

Suponga que un objeto tiene una longitud inicial Li a lo largo de alguna
dirección a una temperatura y la longitud aumenta en una cantidad $`\Delta L`$
para un cambio en temperatura $`\Delta T`$ , el coeficiente de expansión lineal
promedio se define como

```math
\alpha=\frac{\Delta L/L_i}{\Delta T}
```

α es constante para pequeños cambios de temperatura. Esta ecuación se puede
reescribir como

```math
\Delta L=\alpha L_i\Delta T
```

o como

```math
L_f-L_i=\alpha L_i(T_f-T_i)
```

donde Lf es la longitud final, Ti y Tf son las temperaturas inicial y final. La
constante de proporcionalidad α depende de cada material y tiene unidades de
$`({}^\circ C)^{-1}`$ . El área superficial y el volumen también cambian. El
cambio en el volumen está dado por

```math
\Delta V=\beta V_i\Delta T
```

donde β es el coeficiente de expansión volumétrica promedio. Para encontrar la
relación entre α y β, suponga que el coeficiente de expansión lineal promedio
del sólido es el mismo en todas direcciones. Considere una caja sólida cuyo
volumen a cierta temperatura Ti es Vi=lwh, si la temperatura cambia a
$`T_i+\Delta T`$ , su volumen también cambia a $`V_i+\Delta V`$

```math
\begin{aligned}
V_i+\Delta V&=(\ell+\Delta\ell)(w+\Delta w)(h+\Delta h)\\
&=(\ell+\alpha\ell\,\Delta T)(w+\alpha w\,\Delta T)(h+\alpha h\,\Delta T)\\
&=\ell wh(1+\alpha\,\Delta T)^3\\
&=V_i[1+3\alpha\,\Delta T+3(\alpha\,\Delta T)^2+(\alpha\,\Delta T)^3]
\end{aligned}
```

Al dividir ambos lados por Vi y aislar el término $`\Delta V/V_i`$ , se obtiene
el cambio fraccionario en volumen:

```math
\frac{\Delta V}{V_i}=3\alpha\,\Delta T+3(\alpha\,\Delta T)^2+(\alpha\,\Delta T)^3
```

Los términos $`3(\alpha\Delta T)^2`$ y $`(\alpha\Delta T)^3`$ , se desprecian
por no ser representativos para cambios pequeños de temperatura. Al hacer esta
aproximación, es claro que

```math
\frac{\Delta V}{V_i}=3\alpha\,\Delta T\quad\rightarrow\quad\Delta V=(3\alpha)V_i\Delta T
```

Y demostramos que

```math
\beta=3\alpha
```

El cambio de área en una placa rectangular está dada por

```math
\Delta A=2\alpha A_i\Delta T
```

## Fatiga de origen térmico

Supongamos una barra de sección A de un material sujeta por los extremos. Al
aumentar la temperatura en $`\Delta T`$ , debería producirse un cambio
longitudinal $`\Delta L/L=\alpha\Delta T`$ , pero como no se puede dilatar por
estar sujeta, la tensión debe aumentar hasta un valor suficiente para producir
el mismo cambio pero de sentido inverso. El módulo de compresión es

```math
Y=\frac{F/A}{\Delta L/L}
```

Donde A es el área de la sección transversal de la barra. Reemplazando
$`\Delta L/L`$ por $`\alpha\Delta T`$, nos queda la magnitud de la tensión
térmica resultante debido a un cambio de temperatura

```math
F=YA\alpha\Delta T
```

## Procedencia y observaciones

- Original: `2015/Resumen-Fisca-2.pdf`, páginas [73]; sectores delimitados por
  encabezados. SHA-256:
  `b9903f972224365c1a74b5d2732c9a34675c9b719da4c9c2d28e4a0f34e0b0cc`.
- PyMuPDF4LLM, Poppler y cotejo visual completo de los sectores; ecuaciones de
  imagen transcritas a LaTeX, figuras originales preservadas.
- Se restituye el párrafo completo embebido en la imagen del módulo Y y el orden
  de las fórmulas. Se conserva «módulo de compresión» del original.
