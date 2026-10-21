# Maxwell: energía, balance y vector de Poynting

Unidad Temática X — Ecuaciones de Maxwell

## DENSIDAD Y FLUJO DE ENERGÍA ELECTROMAGNÉTICA

Si en una región del espacio existen campos eléctrico y magnético variables en
el tiempo, la densidad volumétrica de energía electromagnética debida a los
campos esta dada por:

La densidad de la energía electromagnética instantánea total

```math
u=\frac12\varepsilon_o E^2+\frac12\frac{B^2}{\mu_o}
```

Faraday

```math
\vec\nabla\times\vec E=-\frac{\partial\vec B}{\partial t}
```

Ampere Maxwell

```math
\vec\nabla\times\vec B=\mu_o\left(\vec J_C+\varepsilon_o\frac{\partial\vec E}{\partial t}\right)
```

Multiplicando escalarmente a izquierda por $`\vec B/\mu_0`$ y $`\vec E/\mu_0`$
respectivamente

```math
\frac{\vec B}{\mu_o}\cdot\vec\nabla\times\vec E=-\frac{\vec B}{\mu_o}\cdot\frac{\partial\vec B}{\partial t}
```

```math
\frac{\vec E}{\mu_o}\cdot\vec\nabla\times\vec B=\vec E\cdot\left(\vec J_C+\varepsilon_o\frac{\partial\vec E}{\partial t}\right)
```

Restando miembro a miembro

```math
\frac{\vec B}{\mu_o}\cdot\vec\nabla\times\vec E-\frac{\vec E}{\mu_o}\cdot\vec\nabla\times\vec B=-\vec E\cdot\vec J_C-\left(\varepsilon_o\vec E\cdot\frac{\partial\vec E}{\partial t}+\frac{\vec B}{\mu_o}\cdot\frac{\partial\vec B}{\partial t}\right)\tag{**}
```

```math
\vec\nabla\cdot(\vec A\times\vec B)=\vec B\cdot(\vec\nabla\times\vec A)-\vec A\cdot(\vec\nabla\times\vec B)
```

El miembro de la izquierda se puede expresar como:

(Schaum 22.40)

```math
\frac{\vec B}{\mu_o}\cdot\vec\nabla\times\vec E-\frac{\vec E}{\mu_o}\cdot\vec\nabla\times\vec B=\vec\nabla\cdot\left(\frac{\vec E\times\vec B}{\mu_o}\right)
```

definimos

```math
\vec S=\frac{\vec E\times\vec B}{\mu_o}
```

Vector de Poynting

De la expresión de la densidad de energía EM =>

```math
u=\frac12\varepsilon_o E^2+\frac12\frac{B^2}{\mu_o}
```

```math
\varepsilon_o\vec E\cdot\frac{\partial\vec E}{\partial t}+\frac{\vec B}{\mu_o}\cdot\frac{\partial\vec B}{\partial t}=\frac{\partial u}{\partial t}
```

Reemplazando estos resultados en la ecuación (\*\*)

```math
\vec\nabla\cdot\vec S=-\vec E\cdot\vec J_C-\frac{\partial u}{\partial t}\ \longrightarrow\ \frac{\partial u}{\partial t}=-\vec\nabla\cdot\vec S-\vec E\cdot\vec J_C
```

La ecuación previa representa el balance local de energía del campo EM. Si
integramos en una zona del espacio de volumen V y superficie Σ.

```math
\int_V\frac{\partial u}{\partial t}\,dV=-\int_V\vec\nabla\cdot\vec S\,dV-\int_V\vec E\cdot\vec J_C\,dV
```

```math
\int_V\frac{\partial u}{\partial t}\,dV=\frac d{dt}\left[\int_V u\,dV\right]=\frac{dW}{dt}\qquad\text{donde}\quad U=\int_V u\,dV
```

W es la energía electromagnética total contenida en V. Aplicando el teorema de
la divergencia tenemos:

```math
\int_V\vec\nabla\cdot\vec S\,dV=\oint_\Sigma\vec S\cdot d\vec A
```

Podemos expresar finalmente la ecuación de balance de energía como:

```math
\underbrace{\frac{dW}{dt}}_{(1)}=-\underbrace{\oint_\Sigma\vec S\cdot d\vec A}_{(2)}-\underbrace{\int_V\vec E\cdot\vec J_C\,dV}_{(3)}
```

La ecuación se reitera en la página 39:

```math
\underbrace{\frac{dW}{dt}}_{(1)}=-\underbrace{\oint_\Sigma\vec S\cdot d\vec A}_{(2)}-\underbrace{\int_V\vec E\cdot\vec J_C\,dV}_{(3)}
```

(1): representa el cambio en el tiempo de la energía electromagnética contenida
en el volumen V.

(2): representa la energía del campo EM que fluye a través de la superficie Σ.
El vector de Poynting representa la energía que atraviesa Σ por unidad de
superficie y de tiempo.

(3): representa la potencia de perdida por efecto Joule. Esa energía es
entregada a las partículas contenidas en V.

```math
P=\int_V\vec E\cdot\vec J_C\,dV
```

## Observación sobre la notación original

La página 38 usa W en la derivada temporal y U para la integral de energía. Se
conserva esa variación sin corregirla silenciosamente. Las referencias «Schaum
22.40» y, en la nota siguiente, «Schaum 22.18» apuntan en el PDF a un archivo
local externo:
`../../Libros Física/Schaum Mathematical Handbook Of Formulas And Tables.pdf`;
ese archivo no está incorporado como enlace relativo al repositorio.

## Procedencia y observaciones de transcripción

- Original: `2019/3er Parcial/2017 UT X - Ecuaciones de Maxwell.pdf`, páginas
  35–39 de 44. Fecha impresa: 22/06/2018; el archivo se llama 2017 y está
  archivado en 2019.
- SHA-256: `a3fbcbd2a058fabe49a11845b069458b60cb348b3497ce7097a46a131603a856`.
- Herramientas: preflight y extracción PyMuPDF4LLM, Poppler, inspección y medios
  PyMuPDF. Todas las páginas, expresiones y figuras del tramo cotejadas
  visualmente.
- Se conservan las referencias (\*\*), Schaum 22.40 y los tres términos
  numerados del balance. Las referencias locales externas se registran como
  texto, sin crear enlaces rotos.
