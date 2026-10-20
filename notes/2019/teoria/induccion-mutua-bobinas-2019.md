# Inducción mutua entre bobinas

Unidad Temática VII — Electromagnetismo

## Inducción Mutua

En las experiencias de Faraday con dos bobinas arrolladas una sobre la otra y
aisladas eléctricamente, cuando variaba la intensidad de corriente que circulaba
por una de ellas, se generaba una corriente inducida en la otra. Esto es, en
esencia, el fenómeno de la inducción mutua. La variación de la intensidad de
corriente en una bobina da lugar a un campo magnético variable. Este campo
magnético origina un flujo magnético también variable que atraviesa la otra
bobina e induce en ella, de acuerdo con la ley de Faraday-Henry, una fuerza
electromotriz. Cualquiera de las bobinas del par puede ser el elemento inductor
y cualquiera el elemento inducido, de ahí el calificativo de mutua que recibe
este fenómeno de inducción.

![Bobinas concentricas aisladas, circuito y galvanómetro, repetidas en página 55](../../../resources/2019/fenomenos-induccion/bobinas-concentricas.png)

![Bobinas 1 y 2 con N1 N2 espiras y corrientes I1 I2](../../../resources/2019/fenomenos-induccion/bobinas-mutua.png)

Φ₂₁ Flujo en la bobina 2 debido a la corriente I1 en la bobina 1

Para una bobina de N espiras es

```math
L=\frac{N\Phi}I
```

Definimos la Inductancia mutua M₂₁ para de la bobina 2 con respecto a la bobina
1 como:

```math
M_{21}=\frac{N_2\Phi_{21}}{I_1}\Rightarrow\Phi_{21}=\frac{M_{21}I_1}{N_2}
```

Si I1 es variable genera en 2 una fem

```math
\varepsilon_2=-N_2\frac{d\Phi_{21}}{dt}=-N_2\frac{M_{21}}{N_2}\frac{dI_1}{dt}
```

```math
\varepsilon_2=-M_{21}\frac{dI_1}{dt}
```

Similarmente si I2 es variable genera en 1 una fem

```math
\varepsilon_1=-M_{12}\frac{dI_2}{dt}
```

```math
\varepsilon_2=-M_{21}\frac{dI_1}{dt}\qquad\varepsilon_1=-M_{12}\frac{dI_2}{dt}
```

En la Inductancia mutua la fem inducida en una bobina es siempre proporcional a
la velocidad de cambio de la corriente de la otra bobina

Se demuestra que

```math
M_{12}=M_{21}=M
```

por tanto:

```math
\varepsilon_2=-M\frac{dI_1}{dt}\quad\text{y}\quad\varepsilon_1=-M\frac{dI_2}{dt}
```

La unidad de inductancia mutua es el Henry

![Fotografía original de un cepillo y su base](../../../resources/2019/fenomenos-induccion/cepillo-inductivo.png)

![Bobina 1 base y bobina 2 mango, NB NH y longitud l](../../../resources/2019/fenomenos-induccion/bobinas-base-mango.png)

## Procedencia y observaciones de transcripción

- Original:
  `2019/2do Parcial/2019 UT VII - Fenómenos de Inducción Electromagnética.pdf`,
  páginas 55–58 de 67. Fecha impresa: 14/05/2019.
- SHA-256: `cbefa338a0f56f56079880a84f05a963257a6473febd8da50f944a67f2210a8f`.
- Herramientas: PyMuPDF4LLM, Poppler y recortes PyMuPDF; todas las páginas,
  expresiones y figuras del tramo cotejadas visualmente. Se conserva el
  desarrollo original.
- La página 58 sólo presenta fotografía y esquema; no se añade una explicación
  de funcionamiento. Se conserva «para de la bobina» de página 56.
