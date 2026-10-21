# Materiales magnéticos, paramagnetismo y ley de Curie

Unidad Temática VIII — Magnetismo en Medios materiales

## Materiales Magnéticos

De acuerdo con sus propiedades se clasifican en:

- Paramagnéticos: débilmente atraído por campos magnéticos intensos (Aluminio,
  Aire, Platino, Sodio).
- Diamagnéticos: débilmente repelidos por campos magnéticos intensos (Plata,
  Cobre, Agua, Mercurio).
- Ferromagnéticos: fuertemente atraídos por campos magnéticos intensos.
  Presentan fenómenos de histéresis y dominios magnéticos. Hierro, níquel,
  cobalto y aleaciones. Gadolinio y Disprosio.

Considerando la permeabilidad magnética y la susceptibilidad magnética tenemos
que:

```math
\mu=\mu_0(1+\chi_m)\qquad\begin{cases}\mu\gt\mu_0&\text{Sustancia Paramagnética}\\\mu\lt\mu_0&\text{Sustancia Diamagnética}\end{cases}
```

Debido a que χm es muy pequeño para sustancias paramagnéticas y diamagnéticas.

```math
\mu\cong\mu_0
```

Para sustancias paramagnéticas y diamagnéticas

En sustancias ferromagnéticas μ es típicamente algunos cientos de veces mas
grande que μ0 (esto implica que χm es muy grande para sustancias
ferromagnéticas)

## Paramagnetismo

Los materiales paramagnéticos presentan momentos dipolares permanentes
independientemente de si existe o no campo B externo. Se origina en el Spin de
los electrones y su giro alrededor del núcleo. A temperatura ambiente la
agitación térmica es suficiente par mantener las orientaciones al azar. En
presencia de B una fracción f de los dipolos se orienta según el campo,
estableciéndose una magnetización neta.

```math
f=\frac{\mu B}{3kT}\rightarrow M=nf\mu=\frac{n\mu^2B}{3kT}
```

n: átomos por unidad de volumen

```math
B=\mu_0H\rightarrow M=\frac{n\mu^2\mu_0H}{3kT}\rightarrow\chi_m=\frac MH=\frac{n\mu^2\mu_0}{3kT}
```

Ley de Curie

La susceptibilidad magnética χm y la magnetización son inversamente
proporcionales a la temperatura T.

- T: temperatura absoluta (ºK)
- K: constante de Boltzman
- μ0: permeabilidad magnética del vacio.

```math
0\lt\chi_m\le1
```

Pequeña pero positiva., como resultado de la presencia de átomos o iones que
tienen momento magnético permanente

Los momentos interactúan débilmente, y en ausencia de campo magnético externo
están orientados al azar. Si existe campo magnético externos los momentos
tienden a alinearse con el, pero la temperatura ambiente es suficiente para
desordenarlos y randomizar sus orientaciones. Pierre Curie (1859-1906) y otros
hallaron experimentalmente que la magnetización de una sustancia paramagnética
es proporcional al campo magnético aplicado e inversamente proporcional a la
temperatura absoluta.

```math
M=C\frac{B_0}T
```

Ley de Curie

C: Cte de Curie

Si B0/T aumenta, todos los átomos se alinean a B, y tenemos el valor de
saturación. Una sustancia ferromagnética, al aumentar T, para determinado valor
de la misma la sustancia pierde su magnetización residual y se vuelve
paramagnética. Esa temperatura critica se denomina Temperatura de Curie.

## Procedencia y observaciones de transcripción

- Original:
  `2019/2do Parcial/2019 UT VIII - Magnetismo en Medios materiales.pdf`, páginas
  12–15 de 21. No consta fecha impresa; 2019 es del nombre del archivo.
- SHA-256: `5d97f163bf24ba9b9d9317dbe7faec1a00e5fab87621e3849d37756083e8f919`.
- Herramientas: PyMuPDF4LLM, Poppler y recortes PyMuPDF; páginas, expresiones y
  figuras del tramo cotejadas visualmente.
- Se conserva «suficiente par», «positiva.,», «campo magnético externos»,
  «Boltzman» y la unidad ºK del original. Las relaciones matemáticas fueron
  reconstruidas contra las páginas, no inferidas del texto extraído.

## Versión impresa de seis diapositivas

El archivo `2019/2do Parcial/UT 8 6 pag.pdf` (SHA-256
`d2d2d0f25fb3fdf3e79399ff0127bd753745d6368a9511122ae7f7076e1f09b2`) reproduce
estas diapositivas en las páginas 2, 3 de cuatro. Se cotejaron texto,
expresiones y figuras contra la versión individual; no contiene contenido
adicional en este tramo. La correspondencia por diapositiva está en
[el registro de imposiciones](../../../resources/common/imposiciones.json).
