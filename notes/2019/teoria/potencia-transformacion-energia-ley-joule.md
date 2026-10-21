# Potencia suministrada a un resistor. Ley de Joule

```math
P=Vi=i^2R=\frac{V^2}R
```

La ecuación general para la potencia suministrada a cualquier elemento de un
circuito es

```math
P=\frac{dW}{dt}=\frac{V\,dq}{dt}=Vi
```

Para el caso del resistor, utilizando la ley de Ohm podemos expresarla como

```math
P=i^2R
```

Ley de Joule

Es imposible tomar potencia eléctrica de un resistor, la potencia siempre fluye
hacia el resistor. ¿que pasa con la energía suministrada al mismo? Los
resistores no almacenan energía como los capacitores, sino que la disipan en
forma de calor al medio que lo rodea.

## Transformación de energía. Potencia. Ley de Joule

Consideremos un portador de carga q en un conductor cilíndrico homogéneo de
sección A y longitud L, bajo la influencia de un campo eléctrico E. El trabajo
que realiza el campo sobre la carga es:

```math
dW=\vec F\cdot\overrightarrow{dl}=q\vec E\cdot\overrightarrow{dl}
```

y la potencia

```math
p=\frac{dW}{dt}=q\vec E\cdot\frac{\overrightarrow{dl}}{dt}=q\vec E\cdot\vec v
```

Si el conductor tiene N portadores por unidad de volumen, la potencia total
suministrada es:

```math
dP=Np\,dV=Nq\vec E\cdot\vec v\,dV
```

```math
dP=Np\,dV=Nq\vec E\cdot\vec v\,dV
```

empleando

```math
\vec J=Nq\vec v
```

```math
dP=\vec E\cdot\vec J\,dV\Rightarrow P=\int_V\vec E\cdot\vec J\,dV
```

```math
dV=\overrightarrow{dA}\cdot\overrightarrow{dL}\Rightarrow P=\left(\int_L\vec E\cdot\overrightarrow{dL}\right)\left(\int_S\vec J\cdot\overrightarrow{dA}\right)
```

```math
\int_L\vec E\cdot\overrightarrow{dL}=\Delta V\quad\mathrm y\quad\int_S\vec J\cdot\overrightarrow{dA}=I
```

```math
P=\Delta V\,I=I^2R
```

Ley de Joule

## Procedencia y observaciones de transcripción

- Original: `2019/1er Parcial/2017 UT IV - Electrocinética.ppt.pdf`, páginas 27,
  28, 29 de 55.
- SHA-256: `5593bcdeb59339b25f4dfee074beac1812300dcec491fb423777a4e776ba1399`.
- El nombre del archivo indica 2017; se conserva bajo 2019 por su ubicación
  canónica. No consta autor en estas páginas.
- Herramientas: PyMuPDF4LLM, PyMuPDF y Poppler; cotejo visual de texto,
  fórmulas, tablas y diagramas. Figuras originales conservadas por recorte y
  render.
- Se transcribe también la fórmula diminuta oscura del margen superior izquierdo
  de la página 27, cotejada ampliada. Se conserva la repetición de dP entre las
  páginas 28 y 29 y el producto entre dA y dL tal como aparece.
