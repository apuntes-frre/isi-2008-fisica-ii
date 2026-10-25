# Resumen de Física II — permeabilidad, susceptibilidad y campos B,H,M

## Relación entre B, H y M. Permeabilidad y susceptibilidad magnética

Con objeto de diferenciar la acción de Bex debido a la corriente libre del Bm
debido a la corriente amperiana se define un nuevo vector H, denominado
intensidad magnética, como

```math
B_0=\mu_0\vec H
```

```math
\vec H=\frac{\vec B}{\mu_0}-\vec M
```

Las unidades de H en el SI son amperios/metro. Las fuentes de H son únicamente
las corrientes libres, no las de magnetización. La circulación de la intensidad
magnética H es igual a la corriente debida a las cargas libres que atraviesan el
área definida por el camino de integración

```math
\boxed{\int}\vec H\cdot\overrightarrow{dl}=I
```

En las sustancias paramagnéticas y diamagnéticas los vectores M y H están
relacionados mediante

```math
\vec M=\chi_m\vec H
```

donde $`\chi_m`$ es la **susceptibilidad magnética** de la sustancia, y está
dado por $`\chi_m=M/H`$ . Sustituyendo la relación entre M y H en la expresión
del campo magnético total, tenemos

```math
\mathbf B=\mu_0\mathbf H+\mu_0\mathbf M=\mu_0(\mathbf H+\chi_m\mathbf H)=\mu_0(1+\chi_m)\mathbf H
```

Como $`\mu=\mu_0(1+\chi_m)=\mu_0\mu_r`$ es la **permeabilidad magnética** del
medio, la ecuación anterior nos queda.

```math
\vec B=\mu\cdot\vec H
```

## Propiedades de B y H

Se cumple aún en presencia de materia

```math
\mathop{\boxed{\int}}_{Sup}\vec B\cdot d\vec S=0
```

La integral curvilínea de H sobre una trayectoria cerrada es igual a la
intensidad de corriente neta que atraviesa el área limitada por la trayectoria

```math
\boxed{\int}\vec H\cdot\overrightarrow{dl}=I
```

La ecuación anterior puede rescribirse como

```math
\boxed{\int}\vec B\cdot\overrightarrow{dl}=\mu_0 I_T
```

donde $`I_T`$ es la suma de la intensidad de corriente verdadera I y la de
magnetización $`I_m`$

## Procedencia y observaciones

- Original: `2015/Resumen-Fisca-2.pdf`, páginas [43]; sectores delimitados por
  encabezados. SHA-256:
  `b9903f972224365c1a74b5d2732c9a34675c9b719da4c9c2d28e4a0f34e0b0cc`.
- PyMuPDF4LLM, Poppler y cotejo visual completo de los sectores; ecuaciones de
  imagen transcritas a LaTeX, figuras originales preservadas.
- Se restituye μ=μ0(1+χm)=μ0μr que la extracción omitió. Las cuatro integrales
  tienen un rectángulo cruzando el signo integral en el PDF: se reproduce
  gráficamente con una integral en caja; no se adivina otro símbolo ni se
  corrige silenciosamente.
