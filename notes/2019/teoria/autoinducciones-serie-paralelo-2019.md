# Autoinducciones en serie y paralelo

Unidad Temática VII — Electromagnetismo

## Autoinducciones en serie

![Bobina L entre bornes a y b](../../../resources/2019/fenomenos-induccion/bobina-bornes.png)

Diferencia de potencial entre los extremos de una bobina

```math
V_a-V_b=L\frac{dI}{dt}
```

![Tres inductancias L1 L2 L3 en serie](../../../resources/2019/fenomenos-induccion/inductancias-serie.png)

![Inductancia equivalente L, corriente I y extremos x y](../../../resources/2019/fenomenos-induccion/inductancia-equivalente.png)

```math
\begin{cases}I=I_1=I_2=I_3\\V=V_1+V_2+V_3\end{cases}
```

```math
\begin{cases}\displaystyle V_1=L_1\frac{dI}{dt}\\\displaystyle V_2=L_2\frac{dI}{dt}\\\displaystyle V_3=L_3\frac{dI}{dt}\\\displaystyle V=L\frac{dI}{dt}\end{cases}\Rightarrow\begin{cases}\displaystyle L\frac{dI}{dt}=L_1\frac{dI}{dt}+L_2\frac{dI}{dt}+L_3\frac{dI}{dt}\\L=L_1+L_2+L_3\end{cases}
```

N autoinducciones en serie

```math
L=\sum_{i=1}^N L_i
```

## Autoinducciones en paralelo

![Tres inductancias L1 L2 L3 en paralelo, corrientes I1 I2 I3](../../../resources/2019/fenomenos-induccion/inductancias-paralelo.png)

![Inductancia equivalente del paralelo](../../../resources/2019/fenomenos-induccion/inductancia-equivalente.png)

```math
\begin{cases}\displaystyle V_1=L_1\frac{dI_1}{dt}=V\\\displaystyle V_2=L_2\frac{dI_2}{dt}=V\\\displaystyle V_3=L_3\frac{dI_3}{dt}=V\\\displaystyle V=L\frac{dI}{dt}\end{cases}
```

```math
\Rightarrow\begin{cases}I=I_1+I_2+I_3\\\displaystyle\frac{dI}{dt}=\frac{dI_1}{dt}+\frac{dI_2}{dt}+\frac{dI_3}{dt}\\\displaystyle\frac VL=\frac V{L_1}+\frac V{L_2}+\frac V{L_3}\\\displaystyle\frac1L=\frac1{L_1}+\frac1{L_2}+\frac1{L_3}\end{cases}
```

N autoinducciones en paralelo

```math
\frac1L=\sum_{i=1}^N\frac1{L_i}
```

## Procedencia y observaciones de transcripción

- Original:
  `2019/2do Parcial/2019 UT VII - Fenómenos de Inducción Electromagnética.pdf`,
  páginas 45–47 de 67. Fecha impresa: 14/05/2019.
- SHA-256: `cbefa338a0f56f56079880a84f05a963257a6473febd8da50f944a67f2210a8f`.
- Herramientas: PyMuPDF4LLM, Poppler y recortes PyMuPDF; todas las páginas,
  expresiones y figuras del tramo cotejadas visualmente. Se conserva el
  desarrollo original.
