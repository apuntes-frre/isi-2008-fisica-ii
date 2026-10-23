# Leyes de Kirchoff — informe del grupo 6: circuito III

## CIRCUITO III

### Ecuación de Nodos

```math
I_1-I_2-I_3=0
```

### Ecuación de Mallas

V)

```math
(R)I_1+(R_1+R_2)I_2=E_1
```

```math
(7{,}77\,\mathrm{k}\Omega)I_1+(6\,\mathrm{k}\Omega)I_2=16{,}72\mathrm V
```

VI)

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
(-6\,\mathrm{k}\Omega)I_1+(3{,}7\,\mathrm{k}\Omega)I_3=-1{,}38\mathrm V
\end{cases}
```

```math
\begin{aligned}
I_1&=1{,}58\,\mathrm{mA}\\
I_2&=0{,}74\,\mathrm{mA}\\
I_3&=0{,}83\,\mathrm{mA}
\end{aligned}
```

### Ecuaciones para VΔ

Ecuación para Vac

```math
\begin{aligned}
V_a+R.I_1&=V_c\\
V_c-V_a&=R.I_1\\
V_c-V_a&=7{,}77\mathrm{k}\Omega.1{,}58\,\mathrm{mA}\\
V_c-V_a&=12{,}28\mathrm V
\end{aligned}
```

Ecuación para Vcd

```math
\begin{aligned}
V_c+R_1.I_2&=V_d\\
V_d-V_c&=R_1.I_2\\
V_d-V_c&=2{,}7\mathrm{k}\Omega.0{,}74\,\mathrm{mA}\\
V_d-V_c&=2{,}01\mathrm V
\end{aligned}
```

Ecuación para Veb

```math
\begin{aligned}
V_e+R_2.I_2&=V_b\\
V_b-V_e&=R_2.I_2\\
V_b-V_e&=3{,}3\mathrm{k}\Omega.0{,}74\,\mathrm{mA}\\
V_b-V_e&=2{,}44\mathrm V
\end{aligned}
```

Ecuación para Vgb

```math
\begin{aligned}
V_g-R_4.I_3&=V_b\\
V_b-V_g&=-R_4.I_3\\
V_b-V_g&=-2{,}2\mathrm{k}\Omega.0{,}83\,\mathrm{mA}\\
V_g-V_b&=-1{,}83\mathrm V
\end{aligned}
```

Ecuación para Vcf

```math
\begin{aligned}
V_c-R_3.I_3&=V_f\\
V_f-V_c&=-R_3.I_3\\
V_f-V_c&=-1{,}5\mathrm{k}\Omega.0{,}83\,\mathrm{mA}\\
V_f-V_c&=-1{,}25\mathrm V
\end{aligned}
```

## Procedencia y observaciones

- Original: `2015/L6 Kirchoff G6 Aprobado.pdf`, página 15 desde «CIRCUITO III» y
  página 16 completa. SHA-256:
  `534403fde9ec3209246d64553b98096c417d8f500a5a5cc4424914482ac9ac79`.
- Todas las expresiones cotejadas contra ambas páginas renderizadas, con
  Poppler/PyMuPDF4LLM como apoyo; no se recalculan resultados.
- Se conserva la numeración V/VI de mallas. El sistema imprime 3,02 kΩ frente a
  7,77 kΩ de la sustitución de malla, I3 en el segundo término de su segunda
  fila e I1 en el primer término de su tercera fila. Las discrepancias no se
  corrigen silenciosamente.
- Se conserva la inversión Vb−Vg a Vg−Vb en la última línea de Vgb y todos los
  redondeos impresos: 12,28; 2,01; 2,44; −1,83 y −1,25 V.
- La figura anterior al título del circuito III en página 15 pertenece al
  circuito II y está conservada en su apunte de simulación. Las simulaciones de
  este circuito III están en páginas 17–19 y se guardan por separado.
- El año corresponde a la carpeta; estas páginas no tienen fecha impresa.

[Circuito II](kirchhoff-informe-grupo-6-circuito-dos.md).
