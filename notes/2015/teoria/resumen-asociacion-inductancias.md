# Resumen de Física II — asociación de inductancias

## En serie

Supongamos tres inductores conectados en serie en un circuito, y debemos obtener
la inductancia de un inductor equivalente que los reemplace. La corriente que
pasa por los inductores en la misma

```math
I=I_1=I_2=I_3
```

La diferencia de potencial del inductor equivalente es igual a la suma de las
deferencias de potencial individuales.

```math
V=V_1+V_2+V_3
```

La diferencia de potencial en cada inductor es $`\Delta V_i=L_i\,dI/dt`$ por lo
tanto

```math
L\frac{dI}{dt}=L_1\frac{dI}{dt}+L_2\frac{dI}{dt}+L_3\frac{dI}{dt}
```

Al ser iguales las corrientes que pasan por los inductores, la rapidez de
variación de la corriente di/dt también deben ser las mismas, por lo tanto la
inductancia L del inductor equivalente es

```math
L=L_1+L_2+L_3
```

## En paralelo

Supongamos tres inductores conectados en paralelo en un circuito, y debemos
obtener la inductancia de un inductor equivalente que los reemplace. Los tres
inductores se encuentran a la misma diferencia de potencial.

```math
V=V_1=V_2=V_3
```

La corriente que debería pasar por el inductor equivalente, es la suma de las
corrientes individuales de cada inductor

```math
I=I_1+I_2+I_3
```

Por lo tanto
$`\frac{dI_{eq}}{dt}=\frac{dI_1}{dt}+\frac{dI_2}{dt}+\frac{dI_3}{dt}`$, como
$`\frac{dI_i}{dt}=\frac{\Delta V_i}{L_i}`$ entonces tenemos que

```math
\frac{\Delta V}{L_{eq}}=\frac{\Delta V_1}{L_1}+\frac{\Delta V_2}{L_2}+\frac{\Delta V_3}{L_3}
```

Cancelamos las diferencias de potenciales por ser las mismas y la inductancia
del inductor equivalente queda como

```math
\frac1L=\frac1{L_1}+\frac1{L_2}+\frac1{L_3}
```

## Procedencia y observaciones

- Original: `2015/Resumen-Fisca-2.pdf`, páginas [38, 39]; sectores delimitados
  por encabezados. SHA-256:
  `b9903f972224365c1a74b5d2732c9a34675c9b719da4c9c2d28e4a0f34e0b0cc`.
- PyMuPDF4LLM, Poppler y cotejo visual completo de los sectores; ecuaciones de
  imagen transcritas a LaTeX, diagramas originales preservados.
- Se conservan «en la misma», «deferencias» y di/dt del texto frente a dI/dt de
  las fórmulas.
