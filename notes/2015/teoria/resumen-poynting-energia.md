# Resumen de Física II — vector de Poynting y energía electromagnética

La rapidez de flujo de la energía en una onda electromagnética se representa
mediante un vector S, llamado vector de Poynting, que se define por la expresión

```math
\vec S=\frac1{\mu_0}\vec E\times\vec B
```

La magnitud del vector de Poynting representa la rapidez a la cual fluye la
energía a través de una superficie unitaria perpendicular a la dirección de
propagación de la onda. Por lo tanto, la magnitud S representa energía por
unidad de área. El vector está dirigido en la dirección de propagación de la
onda. Las unidades del SI para S son $`J/s\cdot m^2=W/m^2`$ . La magnitud S para
una onda plana es

```math
S=\frac{EB}{\mu_0}
```

Como B=E/c entonces

```math
S=\frac{E^2}{\mu_0c}=\frac{cB^2}{\mu_0}
```

S representa la rapidez instantánea por la cual fluye energía por unidad de
área. El promedio en el tiempo de S se llama intensidad de onda I. En el tiempo,
el promedio de $`\cos^2(kx-\omega t)`$ tiene un valor de 1/2, en consecuencia S
promedio queda como

```math
I=S_{\mathrm{prom}}=\frac{E_{\mathrm{máx}}B_{\mathrm{máx}}}{2\mu_0}=\frac{E_{\mathrm{máx}}^2}{2\mu_0c}=\frac{cB_{\mathrm{máx}}^2}{2\mu_0}
```

La densidad de energía instantánea uE asociada con un campo eléctrico se conoce
por la ecuación

```math
u_E=\tfrac12\epsilon_0E^2
```

La densidad de energía instantánea uB asociada con un campo magnético se conoce
por la ecuación

```math
u_B=\frac{B^2}{2\mu_0}
```

Como B=E/c y $`c=1/\sqrt{\mu_0\epsilon_0}`$

```math
u_B=\frac{(E/c)^2}{2\mu_0}=\frac{\epsilon_0\mu_0}{2\mu_0}E^2=\tfrac12\epsilon_0E^2
```

la densidad de energía instantánea asociada con el campo magnético es igual a la
densidad de energía instantánea asociada con el campo eléctrico, en ondas
electromagnéticas.

```math
u_B=u_E=\tfrac12\epsilon_0E^2=\frac{B^2}{2\mu_0}
```

La densidad de energía instantánea total u es igual a la suma de las densidades
de energía

```math
u=u_E+u_B=\epsilon_0E^2=\frac{B^2}{\mu_0}
```

La densidad de energía promedio, nos da de nuevo el factor 1/2, por lo tanto

```math
u_{\mathrm{prom}}=\epsilon_0(E^2)_{\mathrm{prom}}=\tfrac12\epsilon_0E_{\mathrm{máx}}^2=\frac{B_{\mathrm{max}}^2}{2\mu_0}
```

la intensidad de una onda electromagnética es igual a la densidad de energía
promedio multiplicada por la rapidez de la luz.

```math
I=S_{\mathrm{prom}}=cu_{\mathrm{prom}}
```

## Procedencia y observaciones

- Original: `2015/Resumen-Fisca-2.pdf`, páginas [56, 57]; sectores delimitados
  por encabezados. SHA-256:
  `b9903f972224365c1a74b5d2732c9a34675c9b719da4c9c2d28e4a0f34e0b0cc`.
- PyMuPDF4LLM, Poppler y cotejo visual completo de los sectores; ecuaciones de
  imagen transcritas a LaTeX, figuras originales preservadas.
- Se conserva la afirmación «S representa energía por unidad de área» y la
  expresión lineal J/s·m² de unidades, sin añadir agrupaciones ausentes.
