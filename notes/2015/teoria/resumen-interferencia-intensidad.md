# Resumen de Física II — distribución de intensidad de interferencia

Los bordes de las franjas brillantes no son nítidos; hay un cambio gradual de
brillante a oscuro. Ahora calcularemos la distribución de intensidad de luz
asociada con la configuración de interferencia de doble ranura.

Supongamos dos ranuras por donde sale luz con la misma frecuencia angular ω y
están en fase. La magnitud del campo eléctrico en el punto P en la pantalla es
la sobreposición de las dos ondas. Ya que ambas ondas tienen la misma amplitud
E0, los campos eléctricos debido a cada onda son

```math
E_1=E_0\mathop{\mathrm{sen}}\nolimits\omega t\quad\text{y}\quad E_2=E_0\mathop{\mathrm{sen}}\nolimits(\omega t+\phi)
```

Su diferencia de fase φ en P depende de la diferencia de trayectoria.

```math
\phi=\frac{2\pi}\lambda d\mathop{\mathrm{sen}}\nolimits\theta
```

Ahora aplicamos el principio de sobreposición y obtenemos campo eléctrico en el
punto P:

```math
E_P=E_1+E_2=E_0[\mathop{\mathrm{sen}}\nolimits\omega t+\mathop{\mathrm{sen}}\nolimits(\omega t+\phi)]
```

Para simplificar esta expresión, aplique la identidad trigonométrica y nos queda

```math
E_P=2E_0\cos\left(\frac\phi2\right)\mathop{\mathrm{sen}}\nolimits\left(\omega t+\frac\phi2\right)
```

El campo eléctrico en el punto P tiene la misma frecuencia ω que la luz en las
ranuras, pero la amplitud del campo $`2E_0\cos(\phi/2)`$ .

La expresión para la intensidad de luz en el punto P, es proporcional al
cuadrado de la magnitud del campo eléctrico

```math
I\propto E_P^2=4E_0^2\cos^2\left(\frac\phi2\right)\mathop{\mathrm{sen}}\nolimits^2\left(\omega t+\frac\phi2\right)
```

El valor promedio en el tiempo de
$`\mathop{\mathrm{sen}}\nolimits^2(\omega t+\phi/2)`$ es 1/2, por lo tanto, el
promedio de intensidad de luz en el punto P se escribe

```math
I=I_{\mathrm{máx}}\cos^2\left(\frac\phi2\right)
```

donde $`I_{max}`$ es la intensidad máxima en la pantalla. Al sustituir φ nos
queda de la intensidad de luz

```math
I=I_{\mathrm{máx}}\cos^2\left(\frac{\pi d\mathop{\mathrm{sen}}\nolimits\theta}{\lambda}\right)
```

## Procedencia y observaciones

- Original: `2015/Resumen-Fisca-2.pdf`, páginas [62, 63]; sectores delimitados
  por encabezados. SHA-256:
  `b9903f972224365c1a74b5d2732c9a34675c9b719da4c9c2d28e4a0f34e0b0cc`.
- PyMuPDF4LLM, Poppler y cotejo visual completo de los sectores; ecuaciones de
  imagen transcritas a LaTeX, figuras originales preservadas.
- La ecuación de fase se une a partir de dos fragmentos contiguos de la misma
  línea.
