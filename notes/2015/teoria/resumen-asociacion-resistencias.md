# Resumen de Física II — asociación de resistencias

## En serie

En una conexión en serie, la cantidad de carga Q sale de un resistor R 1, deberá
también entrar en el segundo resistor R2. Por lo tanto, la misma corriente
eléctrica pasa por los resistores

```math
I=I_1=I_2
```

donde I es la corriente de la batería.

Ya que la caída de voltaje de a a b es igual a I1R1 y la caída de voltaje de b a
c es I2R2

```math
\Delta V=I_1R_1+I_2R_2
```

La diferencia de potencial entre las terminales de la batería también está
aplicada a la resistencia equivalente $`E_{eq}`$

```math
\Delta V=IR_{\mathrm{eq}}
```

donde la resistencia equivalente tiene el mismo efecto en el circuito que en la
combinación en serie porque resulta de la misma corriente I en la batería. Al
combinar estas ecuaciones para $`\le V`$ se sustituyen los dos resistores en
serie por una sola resistencia equivalente, cuyo valor es la suma de las
resistencias equivalentes

```math
\Delta V=IR_{\mathrm{eq}}=I_1R_1+I_2R_2\quad\rightarrow\quad R_{\mathrm{eq}}=R_1+R_2
```

donde se cancelan las corrientes, porque son las mismas.

La resistencia equivalente de tres o más resistores conectados en serie es

```math
R_{\mathrm{eq}}=R_1+R_2+R_3+\cdots
```

Esta correspondencia indica que la resistencia equivalente de una combinación en
serie de resistores es la suma numérica de las resistencias individuales y
siempre es mayor que cualquier resistencia individual.

## En paralelo

Dos resistores conectados en una combinación en paralelo están conectados
directamente a través de las terminales de la batería, por lo tanto están a la
misma diferencia de potencial

```math
\Delta V=\Delta V_1=\Delta V_2
```

donde $`\Delta V`$ es el voltaje entre las terminales de la batería.

Cuando las cargas llegan al punto a, se dividen en dos; una parte pasa a través
de R1 y el resto a través de R2. Una unión es cualquier punto en un circuito
donde una corriente puede dividirse. Esta división resulta en menos corriente en
cada resistor. La corriente I que entra al punto a es igual a la corriente total

```math
I=I_1+I_2
```

donde I1 es la corriente en R1 e I2 es la corriente en R2. La corriente en la
resistencia equivalente $`R_{eq}`$ es

```math
I=\frac{\Delta V}{R_{\mathrm{eq}}}
```

donde la resistencia equivalente tiene el mismo efecto en el circuito que las
dos resistencias en paralelo, por lo tanto

```math
I=\frac{\Delta V}{R_{\mathrm{eq}}}=\frac{\Delta V_1}{R_1}+\frac{\Delta V_2}{R_2}\quad\rightarrow\quad\frac1{R_{\mathrm{eq}}}=\frac1{R_1}+\frac1{R_2}
```

donde cancelamos las diferencias de potenciales, por ser las mismas. Una
extensión de esta explicación a tres o más resistores en paralelo da:

```math
\frac1{R_{\mathrm{eq}}}=\frac1{R_1}+\frac1{R_2}+\frac1{R_3}+\cdots
```

De esta expresión se ve que el inverso de la resistencia equivalente de dos o
más resistores conectados en una combinación en paralelo es igual a la suma de
los inversos de las resistencias individuales. Además, la resistencia
equivalente siempre es menor que la resistencia más pequeña en el grupo.

## Procedencia y observaciones

- Original: `2015/Resumen-Fisca-2.pdf`, páginas [21, 22]; sectores delimitados
  por encabezados. SHA-256:
  `b9903f972224365c1a74b5d2732c9a34675c9b719da4c9c2d28e4a0f34e0b0cc`.
- PyMuPDF4LLM, Poppler y cotejo visual completo de los sectores. Ecuaciones de
  imagen transcritas a LaTeX.
- Se conservan Eeq en el texto frente a Req en las fórmulas, y el signo ≤V del
  párrafo, sin sustituirlo por ΔV.
