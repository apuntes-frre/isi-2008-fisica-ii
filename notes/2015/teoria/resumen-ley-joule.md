# Resumen de Física II — trasformación de energía y ley de Joule

El trabajo que realiza el campo eléctrico sobre una carga es

```math
dW=\vec F\cdot d\vec l=q\vec E\cdot d\vec l
```

La potencia será:

```math
P=\frac{dW}{dt}=q\cdot\vec E\cdot\frac{d\vec l}{dt}=q\vec E\cdot\vec v
```

Si en el conductor existe N portadores de carga por unidad de volumen, la
potencia que se suministra al elemento de volumen será:

```math
dP=Np\,dV=Nq\vec E\cdot\vec v\cdot dVol
```

Y como $`\vec J=Nq\vec v`$ reemplazando nos queda

```math
dP=\vec J\vec E\cdot dVol
```

La potencia sobre todo el volumen será:

```math
P=\int_V\vec J\vec E\cdot dVol
```

Para el caso del conductor cilíndrico $`dV=dSdl`$ remplazando y ordenando

```math
P=\int_s\vec J\,d\vec S\int_L\vec E\cdot d\vec l
```

Tenemos que $`I=\int\vec Jd\vec S`$ y que $`\Delta V=\int\vec E d\vec l`$ ,
entonces

```math
P=I\cdot\Delta V\quad\text{O bien:}\quad P=I^2\cdot R
```

## Procedencia y observaciones

- Original: `2015/Resumen-Fisca-2.pdf`, páginas [22]; sectores delimitados por
  encabezados. SHA-256:
  `b9903f972224365c1a74b5d2732c9a34675c9b719da4c9c2d28e4a0f34e0b0cc`.
- PyMuPDF4LLM, Poppler y cotejo visual completo de los sectores. Ecuaciones de
  imagen transcritas a LaTeX.
- Se conservan «Trasformación», «N portadores», Np, dV/dVol y los productos tal
  como están impresos; no se añaden puntos entre J y E donde no aparecen.
