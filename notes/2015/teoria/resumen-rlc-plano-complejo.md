# Resumen de Física II — análisis del RLC en el plano complejo

```math
e^{j\omega t}=\cos(\omega t)+j\mathop{\mathrm{sen}}\nolimits(\omega t)
```

```math
\mathop{\mathrm{Re}}\nolimits(V_o e^{j\omega t})=V_o\cos(\omega t)
```

Si aplicamos las leyes de Kirchhoff al circuito tenemos que

```math
\Delta V=L\frac{dI}{dt}+RI+\frac qC
```

Como $`\Delta V=V_0e^{j\omega t}`$ y I = dq/dt tenemos que

```math
L\frac{d^2q(t)}{dt^2}+R\frac{dq(t)}{dt}+\frac{q(t)}C=V_o e^{j\omega t}
```

Como $`q(t)=q_0e^{j\omega t}`$

```math
\frac{dq(t)}{dt}=j\omega q_0(\cos\omega t+j\mathop{\mathrm{sen}}\nolimits\omega t)
```

```math
\frac{d^2q(t)}{dt^2}=-\omega^2q_0(\cos\omega t+j\mathop{\mathrm{sen}}\nolimits\omega t)
```

Reemplazamos estas dos expresiones en la ecuación anterior y nos queda

```math
-\omega^2Lq_o e^{j\omega t}+j\omega Rq_o e^{j\omega t}+\frac{q_o e^{j\omega t}}C=V_o e^{j\omega t}
```

Cancelamos el termino $`e^{j\omega t}`$ y despejamos q0

```math
q_o=\frac{V_o}{-\omega^2L+j\omega R+\frac1C}
```

Como $`q(t)=q_0e^{j\omega t}`$

```math
q(t)=\left(\frac{V_o}{-\omega^2L+j\omega R+\frac1C}\right)e^{j\omega t}
```

Si ahora derivamos esta expresión con respecto al tiempo tendremos la expresión
de la corriente eléctrica I(t) en función del tiempo

```math
i(t)=\frac{dq(t)}{dt}=\left(\frac{j\omega V_o}{-\omega^2L+j\omega R+\frac1C}\right)e^{j\omega t}
```

```math
i(t)=\frac{dq(t)}{dt}=\left(\frac{V_o}{R+j\left(\omega L-\frac1{\omega C}\right)}\right)e^{j\omega t}
```

Donde el denominador es la impedancia Z del circuito

```math
Z=R+j\left(\omega L-\frac1{\omega C}\right)
```

```math
Z=|Z|e^{j\theta}
```

```math
|Z|=\sqrt{R^2+\left(\omega L-\frac1{\omega C}\right)^2}\qquad\theta=\mathop{\mathrm{atan}}\nolimits\left(\frac{\omega L-\frac1{\omega C}}R\right)
```

La ecuación de la corriente en función del tiempo nos queda

```math
i(t)=\frac{dq(t)}{dt}=\left(\frac{V_o}{|Z|}\right)e^{j(\omega t-\theta)}
```

```math
i(t)=\left(\frac{V_o}{|Z|}\right)e^{j(\omega t-\theta)}=\left(\frac{V_o}{|Z|}\right)\left(\cos(\omega t-\theta)+j\mathop{\mathrm{sen}}\nolimits(\omega t-\theta)\right)
```

```math
I(t)=\mathop{\mathrm{Re}}\nolimits[i(t)]=\frac{V_o}{|Z|}\cos(\omega t-\theta)
```

La amplitud de la corriente depende de los valores de los elementos del circuito
R, L y C. Se define la impedancia compleja del circuito, tiene dimensión de
resistencia eléctrica, esto es ohm

```math
Z=R+j\left(\omega L-\frac1{\omega C}\right)
```

Existe una diferencia de fase ϴ entre la diferencia de potencial aplicado
$`V(t)=V_0\cos(\omega t)`$ y la corriente que circula
$`I(t)=I_0\cos(\omega t-\theta)`$

La frecuencia angular ω de la fem que excita al circuito y la respuesta del
circuito, es decir, la corriente tiene la misma frecuencia angular.

La diferencia de potencial sobre cada elemento de circuito, se puede presentar
en forma vectorial

```math
V_o=I_o|Z|=I_o\sqrt{R^2+\left(\omega L-\frac1{\omega C}\right)^2}=\sqrt{(RI_o)^2+\left(\omega LI_o-\frac1{\omega C}I_o\right)^2}
```

```math
V_o=\sqrt{(V_R)^2+(V_L-V_C)^2}\qquad\theta=\mathop{\mathrm{atan}}\nolimits\left[\frac{V_L-V_C}{V_R}\right]
```

## Procedencia y observaciones

- Original: `2015/Resumen-Fisca-2.pdf`, páginas [50, 51]; sectores delimitados
  por encabezados. SHA-256:
  `b9903f972224365c1a74b5d2732c9a34675c9b719da4c9c2d28e4a0f34e0b0cc`.
- PyMuPDF4LLM, Poppler y cotejo visual completo de los sectores; ecuaciones de
  imagen transcritas a LaTeX, figuras originales preservadas.
- Se conservan o/0 en subíndices según cada expresión y atan como operador del
  original. El factor Io posterior a 1/ωC está fuera del denominador en el
  original.
