# Flujo magnético y unidad wéber

Unidad Temática VII — Electromagnetismo

## De la experiencia deducimos que

- Solo se genera corriente si hay movimiento relativo entre la espira y el imán.
- En el instante en que cesa el movimiento cesa la corriente.
- Esta corriente es producida por una fem, que denominaremos fem inducida.
- La fem aparece en la espira cada vez que cambia la intensidad del campo
  magnético en la región del espacio que ocupa la espira.
- La fem inducida cambia la polaridad cuando se invierte el sentido del
  movimiento.
- En la generación de corrientes (fem) inducidas podemos distinguir dos
  elementos
  - El inducido, que es el circuito donde aparece la corriente (la espira)
  - El inductor, que es el agente que provoca el fenómeno (el imán)

## Flujo magnético

Se define el flujo del campo magnético a través de una superficie como el número
total de líneas de fuerza que atraviesan tal superficie. En términos
matemáticos, para un campo magnético constante y una superficie plana de área S,
el flujo magnético se expresa en la forma:

```math
\phi_B=\vec B\cdot\vec S=BS\cos(\theta)
```

![Campo B variable función de la posición y superficie gaussiana S](../../../resources/2019/fenomenos-induccion/flujo-superficie.png)

Si B es no homogéneo y S de forma arbitraria

```math
d\phi_B=\vec B\cdot\overrightarrow{dS}=B\cos(\theta)\,dS
```

```math
\phi_B=\int\vec B\cdot\overrightarrow{dS}=\int B\cos(\theta)\,dS
```

## Magnetic Flux

```math
\Phi_B=B_\perp A
```

El flujo depende de tres factores: el campo magnético B, la superficie S y el
ángulo θ entre B y dS, basta que cambie uno de ellos para que el flujo cambie.
En las experiencias de Faraday vimos cambia el campo magnético, por tanto cambia
el flujo que atraviesa el circuito.

En el Sistema Internacional la unidad de flujo magnético es el Wéber (Wb).

```math
1\mathrm{Wb}=1\mathrm T\,\mathrm m^2
```

Un wéber es el flujo magnético que, al atravesar un circuito de una sola espira
produce en la misma una fuerza electromotriz de 1 volt si se anula dicho flujo
en 1 segundo por decrecimiento uniforme.

## Procedencia y observaciones de transcripción

- Original:
  `2019/2do Parcial/2019 UT VII - Fenómenos de Inducción Electromagnética.pdf`,
  páginas 9–12 de 67. Fecha impresa: 14/05/2019.
- SHA-256: `cbefa338a0f56f56079880a84f05a963257a6473febd8da50f944a67f2210a8f`.
- Herramientas: PyMuPDF4LLM, Poppler y recortes PyMuPDF; cotejo visual de todas
  las páginas, expresiones y figuras del tramo. Se preservan el idioma de las
  láminas y las afirmaciones del original.
