# Maxwell: deducción de la ecuación de ondas

Unidad Temática X — Ecuaciones de Maxwell

Aplicando el rotacional a la ley de Faraday (11)

```math
\vec\nabla\times\vec\nabla\times\vec E=-\vec\nabla\times\frac{\partial\vec B}{\partial t}\tag{13}
```

Empleando la identidad vectorial (\*) y que el rotor conmuta con la derivada
temporal

```math
\vec\nabla\times\vec\nabla\times\vec A=\vec\nabla(\vec\nabla\cdot\vec A)-\nabla^2\vec A\tag{*}
```

```math
\vec\nabla(\vec\nabla\cdot\vec E)-\nabla^2\vec E=-\frac{\partial(\vec\nabla\times\vec B)}{\partial t}\tag{14}
```

Teniendo en cuenta las ecuaciones (9) y (12) obtenemos:

```math
\nabla^2 E=\mu_0\varepsilon_0\frac{\partial^2 E}{\partial t^2}\tag{15}
```

Operando de manera similar sobre (12) y empleando (10) y (11) obtenemos para el
campo magnético

```math
\nabla^2 B=\mu_0\varepsilon_0\frac{\partial^2 B}{\partial t^2}\tag{16}
```

```math
\nabla^2\psi(r,t)-\frac1{v^2}\frac{\partial^2\psi(\vec r,t)}{\partial t^2}=0
```

Ecuación general de ondas

```math
\psi=\psi_o\cos(\vec k\cdot\vec r-\omega t)
```

```math
\omega=2\pi f=2\pi/T
```

```math
|\vec k|=\frac{2\pi}\lambda
```

(módulo del vector número de onda)

## Procedencia y observaciones de transcripción

- Original: `2019/3er Parcial/2017 UT X - Ecuaciones de Maxwell.pdf`, páginas
  21–22 de 44. Fecha impresa: 22/06/2018; el archivo se llama 2017 y está
  archivado en 2019.
- SHA-256: `a3fbcbd2a058fabe49a11845b069458b60cb348b3497ce7097a46a131603a856`.
- Herramientas: preflight y extracción PyMuPDF4LLM, Poppler, inspección y medios
  PyMuPDF. Todas las páginas, expresiones y figuras del tramo cotejadas
  visualmente.
- Se conservan las ecuaciones (13)–(16), la identidad (\*) y la alternancia de
  campos con y sin flecha del original.
