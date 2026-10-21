# Corriente alterna: valores eficaces

Unidad Temática IX — Corriente Alterna

En alterna el valor medio de la tensión y de la corriente a lo largo de un ciclo
es cero ya que toman sucesivamente valores de igual magnitud pero de signo
contrario. Esto no significa que su efecto sea el mismo que tendría una tensión
o una corriente nula.

Por ejemplo, la disipación de energía en una resistencia por efecto Joule es
independiente del sentido en que circula la intensidad.

Para tener en cuenta este hecho se promedia a menudo el cuadrado de los valores
instantáneos y se toma la raíz cuadrada. El resultado es el valor eficaz de la
magnitud correspondiente (o valor rms en inglés). Este es el valor que dan los
voltímetros y amperímetros de c.a, mientras que en un osciloscopio leemos
normalmente el valor máximo de la tensión

Veremos que el valor eficaz de una corriente alterna, es el valor que tendría
una corriente continua que produciría la misma potencia que dicha corriente
alterna, al aplicarla sobre una misma resistencia.

Si F(t) es una función periódica de periodo T, su valor eficaz esta dado por:

```math
F_{eficaz}=\sqrt{\left\langle F(t)^2\right\rangle}=\left[\frac1T\int_0^T F(t)^2\,dt\right]^{1/2}
```

## Valores eficaces de la tensión y de la corriente

```math
\left\langle\varepsilon^2(t)\right\rangle=\left\langle\varepsilon_m^2\sin^2(\omega t)\right\rangle=\varepsilon_m^2\left\langle\sin^2(\omega t)\right\rangle
```

```math
\left\langle\sin^2(\omega t)\right\rangle=\frac1T\int_0^T\sin^2(\omega t)\,dt=\frac12
```

```math
\int\sin(a\cdot x)^2\,dx\ \longrightarrow\ \frac x2-\frac{\sin(2\cdot a\cdot x)}{4\cdot a}
```

```math
\left\langle\varepsilon^2(t)\right\rangle=\frac{\varepsilon_m^2}2\Rightarrow\varepsilon_{eff}=\sqrt{\left\langle\varepsilon^2(t)\right\rangle}=\frac{\varepsilon_m}{\sqrt2}
```

Del mismo modo, teniendo en cuenta que la constante de fase no influye en el
valor medio de $`\mathop{\mathrm{sen}}\nolimits^2(\omega t+\varphi)`$, el valor
eficaz de la intensidad será:

```math
\left\langle i^2(t)\right\rangle=\left\langle i_m^2\sin^2(\omega t+\phi)\right\rangle=i_m^2\left\langle\sin^2(\omega t+\phi)\right\rangle=\frac{i_m^2}2
```

```math
i_{eff}=\sqrt{\left\langle i^2(t)\right\rangle}=\frac{i_m}{\sqrt2}
```

## Procedencia y observaciones de transcripción

- Original: `2019/3er Parcial/2017 UT IX Corriente Alterna.pdf`, páginas 20–22
  de 34. Fecha impresa: 13/06/2018; el archivo se llama 2017 y está archivado en
  2019\.
- SHA-256: `9e7ec2ad4e867b5dc688982d6b052f2b16e926ee1adcfc55f7007697c05cf263`.
- Herramientas: preflight PyMuPDF4LLM, Poppler y recortes PyMuPDF. Páginas,
  expresiones y figuras del tramo cotejadas visualmente.
- La integral de la página 22, insertada como imagen en el original, se
  transcribe a LaTeX. Se conserva la alternancia sen/sin y φ/ϕ.
