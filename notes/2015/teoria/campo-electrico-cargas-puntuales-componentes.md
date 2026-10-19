# Campo eléctrico de una carga puntual y de un sistema de cargas

Conociendo en campo eléctrico, en un punto podemos conocer la fuerza eléctrica
sobre una carga en dicho punto

```math
\vec F_e=q*\vec E
```

Las unidades del campo eléctrico en el S.I. serán

```math
[\vec E]=\frac{[\vec F]}{[q]}=\frac{[Newton]}{[Coulomb]}=\frac{N}{C}
```

## Campo eléctrico de una carga puntual

```math
\vec E=\frac{\vec F_e}{q_0}=\frac1{4\pi\varepsilon_0}\frac1{q_0}\frac{q_0q}{r^2}\vec r
```

```math
\vec E=\frac1{4\pi\varepsilon_0}\frac q{r^2}\vec r
```

## Sistema de N cargas puntuales

Supongamos que tenemos ahora un sistema de N cargas puntuales. La fuerza que
actuará sobre una carga de prueba situada en un punto P del espacio estará dada
por:

```math
\vec F_e=\frac1{4\pi\varepsilon_0}\frac{q_0q_1}{r_1^2}\vec r_1+\frac1{4\pi\varepsilon_0}\frac{q_0q_2}{r_2^2}\vec r_2+\ldots+\frac1{4\pi\varepsilon_0}\frac{q_0q_n}{r_n^2}\vec r_n
```

```math
\vec F_e=\frac{q_0}{4\pi\varepsilon_0}\left(\frac{q_1}{r_1^2}\vec r_1+\frac{q_2}{r_2^2}\vec r_2+\ldots+\frac{q_n}{r_n^2}\vec r_n\right)
```

```math
\vec F_e=\frac{q_0}{4\pi\varepsilon_0}\sum_{i=1}^n\frac{q_i}{r_i^2}\vec r_i
```

```math
\vec E=\frac{\vec F_e}{q_0}=\frac1{4\pi\varepsilon_0}\sum_{i=1}^n\frac{q_i}{r_i^2}\vec r_i=\sum_{i=1}^n\vec E_i
```

```math
\vec E=\frac1{4\pi\varepsilon_0}\sum_{i=1}^n\frac{q_i}{r_i^2}\vec r_i
```

En caso de conocer las coordenadas espaciales de cada carga, el Campo Eléctrico
será posible expresarlo en término de sus componentes:

```math
Ex=\frac1{4\pi\varepsilon_0}\sum_{i=o}^n\frac{qi(xo-xi)}{\left[(xo-xi)^2+(yo-yi)^2+(zo-zi)^2\right]^{3/2}}
```

```math
Ey=\frac1{4\pi\varepsilon_0}\sum_{i=o}^n\frac{qi(yo-yi)}{\left[(xo-xi)^2+(yo-yi)^2+(zo-zi)^2\right]^{3/2}}
```

```math
Ez=\frac1{4\pi\varepsilon_0}\sum_{i=o}^n\frac{qi(zo-zi)}{\left[(xo-xi)^2+(yo-yi)^2+(zo-zi)^2\right]^{3/2}}
```

## Procedencia y observaciones de transcripción

- Original: `2015/UNIDAD 1 Fuerza electrica y campo electrico-1.pdf`,
  páginas11–13 de41. No constan autor ni fecha propios en estas páginas.
- SHA-256: `1130cc5160c8a6f87578f071f70595c679fb1535a8899aa02e13c9b0d093da07`.
- Herramientas: PyMuPDF y Poppler para localizar el texto; cotejo visual de
  todas las ecuaciones, recuperando los símbolos que la fuente privada no
  extrae. Expresiones transcritas en LaTeX.
- Se conserva «Conociendo en campo eléctrico», el límite **i=o** impreso en la
  página13 (frente a i=1 en la12), y las formas Ex, qi, xo, etc. de esa
  diapositiva. Las flechas de r se conservan como vectores y no se reemplazan
  por versores ni se agrega un factor1/r. Las relaciones de los recuadros se
  mantienen como expresiones separadas, incluidas las repetidas.
