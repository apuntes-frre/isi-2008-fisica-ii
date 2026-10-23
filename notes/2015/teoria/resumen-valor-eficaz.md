# Resumen de Física II — valor eficaz

En electricidad y electrónica, en corriente alterna, el valor cuadrático medio
(rms), de una corriente variable es denominado **valor eficaz** . Se define como
el valor de una corriente rigurosamente constante (corriente continua) que al
circular por una determinada resistencia óhmica pura produce los mismos efectos
caloríficos ( _igual potencia disipada_ ) que dicha corriente variable
(corriente alterna). De esa forma una corriente eficaz es capaz de producir el
mismo trabajo que su valor en corriente directa.

El valor eficaz de una corriente alterna $`I=I_0\cos(\omega t+\varphi)`$ se
define como la raíz cuadrada del valor cuadrático medio de la corriente

```math
I_{\mathrm{ef}}=\sqrt{\langle I^2(t)\rangle}
```

```math
I_{\mathrm{ef}}=\sqrt{\langle I_o^2\cos^2(\omega t+\varphi)\rangle}=\sqrt{\frac{I_o^2}T\int_0^T\cos^2(\omega t+\varphi)dt}=\frac{I_o}{\sqrt2}
```

Como se podrá observar, el valor eficaz es independiente de la frecuencia o
periodo de la señal. Ahora analicemos la energía disipada en la resistencia en
un diferencial de tiempo

```math
dW=R[I(t)]^2dt=RI_o^2\cos^2(\omega t+\varphi)dt
```

La energía disipada en un periodo T es

```math
W=RI_o^2\int_0^T\cos^2(\omega t+\varphi)dt=\frac{RI_o^2}2T=RI_{\mathrm{ef}}^2T
```

Este valor de energía corresponde al valor de energía disipada por efecto Joule
en la resistencia R durante el periodo T si por esta circula una corriente
continua de valor

## Procedencia y observaciones

- Original: `2015/Resumen-Fisca-2.pdf`, páginas [48, 49]; sectores delimitados
  por encabezados. SHA-256:
  `b9903f972224365c1a74b5d2732c9a34675c9b719da4c9c2d28e4a0f34e0b0cc`.
- PyMuPDF4LLM, Poppler y cotejo visual completo de los sectores; ecuaciones de
  imagen transcritas a LaTeX, figuras originales preservadas.
- Se elimina el marcado automático ausente del PDF y se restituye la corriente
  I=I0 cos(ωt+φ). La última frase en página49 termina en «una corriente continua
  de valor» sin fórmula visible: no se completa.
