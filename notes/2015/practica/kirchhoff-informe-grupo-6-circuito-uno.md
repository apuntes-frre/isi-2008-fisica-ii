# Leyes de Kirchoff — informe del grupo 6: resultados y circuito I

## 1) Verificación de las leyes de nudos

| Pos. | R (K ) | I1 (mA) | I2 (mA) | I3 (mA) | I1+I2+I3 (mA) |
| -- | -- | -- | -- | -- | -- |
| 1 | 3,02 | 2,9 | -1,2 | -1,6 | 0,1 |
| 2 | 5,01 | 2,1 | -0,9 | -1,1 | 0,1 |
| 3 | 7,77 | 1,6 | -0,7 | -0,8 | 0,1 |

## 2) Verificación de las leyes de malla

| Pos. | R (K ) | E1 (V) | E2 (V) | Vac (V) | Vcd (V) | Veb (V) | Vcf (V) | Vgb (V) | Vac+Vcd+Veb | Vcd+Veb+Vgb+Vcf |
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
| 1 | 3,02 | 16,72 | 1,38 | 9,00 | 3,40 | 4,25 | -2,50 | -3,72 | 16,65 V | 1,43 V |
| 2 | 5,01 | 16,72 | 1,38 | 11,00 | 2,60 | 3,22 | -1,79 | -2,62 | 16,82 V | 1,41 V |
| 3 | 7,77 | 16,72 | 1,38 | 12,40 | 1,99 | 2,53 | -1,24 | -1,82 | 16,92 V | 1,46 V |

## CIRCUITO I

### Ecuación de Nodos

```math
I_1-I_2-I_3=0
```

### Ecuación de Mallas

I)

```math
(R)I_1+(R_1+R_2)I_2=E_1
```

```math
(3{,}02\,\mathrm{k}\Omega)I_1+(6\,\mathrm{k}\Omega)I_2=16{,}72\mathrm V
```

II)

```math
(-R_1-R_2)I_2+(R_3+R_4)I_3=-E_2
```

```math
(-6\,\mathrm{k}\Omega)I_2+(3{,}7\,\mathrm{k}\Omega)I_3=-1{,}38\mathrm V
```

### Sistema de Ecuaciones INTENSIDADES

```math
\begin{cases}
I_1-I_2-I_3=0\\
(3{,}02\,\mathrm{k}\Omega)I_1+(6\,\mathrm{k}\Omega)I_3=16{,}72\mathrm V\\
(-6\,\mathrm{k}\Omega)I_2+(3{,}7\,\mathrm{k}\Omega)I_3=-1{,}38\mathrm V
\end{cases}
```

```math
\begin{aligned}
I_1&=2{,}99\,\mathrm{mA}\\
I_2&=1{,}28\,\mathrm{mA}\\
I_3&=1{,}71\,\mathrm{mA}
\end{aligned}
```

### Ecuaciones para VΔ

Ecuación para Vac

```math
\begin{aligned}
V_a+R.I_1&=V_c\\
V_c-V_a&=R.I_1\\
V_c-V_a&=3{,}02\mathrm{k}\Omega.2{,}99\,\mathrm{mA}\\
V_c-V_a&=9{,}02\mathrm V
\end{aligned}
```

Ecuación para Vcd

```math
\begin{aligned}
V_c+R_1.I_2&=V_d\\
V_d-V_c&=R_1.I_2\\
V_d-V_c&=2{,}7\mathrm{k}\Omega.1{,}28\,\mathrm{mA}\\
V_d-V_c&=3{,}45\mathrm V
\end{aligned}
```

Ecuación para Veb

```math
\begin{aligned}
V_e+R_2.I_2&=V_b\\
V_b-V_e&=R_2.I_2\\
V_b-V_e&=3{,}3\mathrm{k}\Omega.1{,}28\,\mathrm{mA}\\
V_b-V_e&=4{,}22\mathrm V
\end{aligned}
```

Ecuación para Vgb

```math
\begin{aligned}
V_g-R_4.I_3&=V_b\\
V_b-V_g&=-R_4.I_3\\
V_b-V_g&=-2{,}2\mathrm{k}\Omega.1{,}71\,\mathrm{mA}\\
V_g-V_b&=-3{,}76\mathrm V
\end{aligned}
```

Ecuación para Vcf

```math
\begin{aligned}
V_c-R_3.I_3&=V_f\\
V_f-V_c&=-R_3.I_3\\
V_f-V_c&=-1{,}5\mathrm{k}\Omega.1{,}71\,\mathrm{mA}\\
V_f-V_c&=-2{,}56\mathrm V
\end{aligned}
```

## Procedencia y observaciones

- Original: `2015/L6 Kirchoff G6 Aprobado.pdf`, páginas 6–7 de 20. SHA-256:
  `534403fde9ec3209246d64553b98096c417d8f500a5a5cc4424914482ac9ac79`.
- PyMuPDF4LLM y Poppler contrastados con ambas páginas renderizadas; todas las
  celdas y ecuaciones cotejadas visualmente. Los símbolos perdidos en extracción
  se recuperaron del original, sin resolver ni recalcular.
- El encabezado de resistencia de las tablas imprime «(K )», sin Ω visible: se
  conserva. Los resultados de la segunda tabla tienen V dentro de sus celdas.
- El sistema de página 7 usa I3 en el segundo término de su segunda ecuación,
  aunque la ecuación de malla de página 6 usa I2. Se preserva la discrepancia.
  El resultado I2 aparece positivo, distinto del signo de la medición en tabla.
- En Vgb, las tres primeras líneas usan Vb−Vg y la última Vg−Vb: se mantienen
  ambas orientaciones y el resultado negativo, sin corregirlo.
- El título «Ecuaciones para VΔ» conserva el delta como subíndice en el
  original. El año corresponde a la carpeta; estas páginas no están fechadas.
- La hoja manuscrita de página 5 y las simulaciones desde página 8 se cotejan
  por separado; este lote no les atribuye cobertura.

[Fundamentos y técnica](kirchhoff-informe-grupo-6-fundamentos-tecnica.md).
