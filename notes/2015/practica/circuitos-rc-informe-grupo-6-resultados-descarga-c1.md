# Circuitos RC — informe del grupo 6: resultados de descarga C1

## Proceso de descarga (C1)

Datos:

Fuente de Alimentación CC: $`8{,}6\,\mathrm V`$.

Resistencia $`R_t:39000`$.

Capcidad $`C_t:1000\,\mu\mathrm F`$.

| Tiempo | Descarga C1 (V) | $`\mathrm{Vr}(t)=1-(\mathrm{Vt}/\mathrm{Vo})`$ | $`\mathrm{Ln}(\mathrm{Vr}(t))`$ |
| -- | -- | -- | -- |
| 0 | 8,3 | 0,035 | -3,356 |
| 10 | 6,5 | 0,244 | -1,410 |
| 20 | 5 | 0,419 | -0,871 |
| 30 | 3,9 | 0,547 | -0,604 |
| 40 | 3 | 0,651 | -0,429 |
| 50 | 2,4 | 0,721 | -0,327 |
| 60 | 1,9 | 0,779 | -0,250 |
| 70 | 1,4 | 0,837 | -0,178 |
| 80 | 1,1 | 0,872 | -0,137 |
| 90 | 0,9 | 0,895 | -0,111 |
| 100 | 0,7 | 0,919 | -0,085 |
| 110 | 0,5 | 0,942 | -0,060 |
| 120 | 0,4 | 0,953 | -0,048 |
| 130 | 0,3 | 0,965 | -0,036 |
| 140 | 0,3 | 0,965 | -0,036 |
| 150 | 0,2 | 0,977 | -0,024 |
| 160 | 0,2 | 0,977 | -0,024 |
| 170 | 0,1 | 0,988 | -0,012 |
| 180 | 0,1 | 0,988 | -0,012 |
| 190 | 0,1 | 0,988 | -0,012 |

## Determinación de La constante de Tiempo (Método Gráfico)

![Gráfica original Descarga C1 (V), tiempos 0 a 190 y líneas auxiliares azules](../../../resources/2015/circuitos-rc-informe-grupo-6/descarga-c1-experimental.png)

Aproximadamente la abscisa correspondiente a
$`V(t)=V*0{,}37=8{,}6*0{,}37=3{,}182\,\mathrm V`$.se encuentra en 40s.

```math
T_P\approx40\mathrm s.
```

```math
T_T=39\mathrm s
```

## Determinación de la Capacidad

```math
C=T/R\Rightarrow C=40\mathrm s/39000=1.10^{-3}\mathrm F.
```

```math
\Delta R=1950
```

```math
\Delta T=1\mathrm s
```

```math
\Delta C=\Delta T/R+(T*\Delta R)/R^2=1\mathrm s/39000+(39\mathrm s*1950)/(39000)^2=7{,}57*10^{-5}\mathrm F
```

```math
E\%=\Delta C/C*100=0{,}00000757\%
```

## Procedencia y observaciones

- Original: `2015/L3 Capacidad G6 Aprobado.pdf`, página 9 completa y tramo
  inicial de la 10, hasta el cálculo de E%. SHA-256:
  `586d5b26477b67b780929d52df3b218c54dca4ddfe6702e5f6e9d17b0ee5d320`.
- PyMuPDF4LLM y Poppler contrastados con las páginas renderizadas; cotejo de las
  20 filas, encabezados, expresiones y gráfica vectorial original.
- Se conserva «Capcidad» y se mantienen 5 y 3 de la tabla, distintos de 5,0 y
  3,0 de la hoja manuscrita. No se uniforman versiones ni redondeos.
- Se mantienen 40s para la determinación experimental y 39s en la sustitución de
  incertidumbre. El resultado E%=0,00000757% se transcribe tal como aparece, sin
  recomputarlo ni corregir su orden de magnitud.
- El exponente -5 de la incertidumbre se cotejó además en un recorte ampliado
  del PDF, ya que su signo es poco visible en el render reducido.
- Continúa
  [el resultado de carga](circuitos-rc-informe-grupo-6-resultados-carga-c1.md).
  El bloque «Proceso de Carga en Serie» de página 10 está transcrito por
  separado; no se duplica en este apunte.
- El año 2015 corresponde a la carpeta. No consta fecha impresa en este tramo.

## Navegación del informe

[Anterior](circuitos-rc-informe-grupo-6-resultados-carga-c1.md).
[Siguiente](circuitos-rc-informe-grupo-6-resultados-serie.md).
