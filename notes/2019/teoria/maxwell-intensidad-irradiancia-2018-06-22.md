# Maxwell: intensidad e irradiancia

Unidad Temática X — Ecuaciones de Maxwell

## EL VECTOR DE POYNTING

```math
\vec S=\frac1{\mu_o}\vec E\times\vec B\qquad\text{pero}\qquad\vec B=\frac{\vec k\times\vec E}\omega
```

```math
\vec S=\frac{\vec E}{\mu_o}\times\frac{\vec k\times\vec E}\omega=\frac1{\mu_o\omega}\vec E\times(\vec k\times\vec E)=\frac{E^2}{\mu_o\omega}\vec k
```

(Schaum 22.18)

```math
\vec A\times(\vec B\times\vec C)=\vec B(\vec A\cdot\vec C)-\vec C(\vec A\cdot\vec B)
```

```math
\vec E(\vec r,t)=\eta_1 E_o\cos(\vec k\cdot\vec r-\omega t)
```

```math
\vec S=\frac{E^2}{\mu_o\omega}\vec k=\frac{E_o^2\cos^2(\vec k\cdot\vec r-\omega t)}{\mu_o\omega}\vec k
```

El módulo del vector de Pointing da la intensidad de la onda.

```math
S=\frac{E^2}{\mu_o\omega}k=\frac{E_o^2\cos^2(\vec k\cdot\vec r-\omega t)}{\mu_o\omega}k=\frac1{\mu_o}E_oB_o\cos^2(\vec k\cdot\vec r-\omega t)
```

En general el intervalo de tiempo en que se mide la intensidad es mucho mayor
que el periodo de la onda, por lo que en realidad se mide el valor medio.

```math
I=\left\langle|\vec S|\right\rangle=\left\langle\frac{E_o^2\cos^2(\vec k\cdot\vec r-\omega t)}{\mu_o\omega}|\vec k|\right\rangle=\frac{E_o^2k}{2\mu_o\omega}=\frac{E_o^2}{2\mu_o c}
```

```math
I=\frac12\varepsilon_0 c E_o^2=\frac1{2\mu_0}cB_o^2=\frac1{2\mu_0}E_oB_o
```

La Irradiancia es proporcional al cuadrado del campo eléctrico

## Procedencia y observaciones de transcripción

- Original: `2019/3er Parcial/2017 UT X - Ecuaciones de Maxwell.pdf`, páginas
  40–41 de 44. Fecha impresa: 22/06/2018; el archivo se llama 2017 y está
  archivado en 2019.
- SHA-256: `a3fbcbd2a058fabe49a11845b069458b60cb348b3497ce7097a46a131603a856`.
- Herramientas: preflight y extracción PyMuPDF4LLM, Poppler, inspección y medios
  PyMuPDF. Todas las páginas, expresiones y figuras del tramo cotejadas
  visualmente.
- Se conserva «Pointing» en el texto y la referencia Schaum 22.18. La ruta local
  externa de esa referencia queda registrada en la nota de balance de energía.
  Se conservan los subíndices o/0 del original.
