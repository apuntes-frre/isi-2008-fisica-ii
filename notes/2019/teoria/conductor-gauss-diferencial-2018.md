# Propiedades electrostáticas de un conductor

- En electrostática **el campo eléctrico es nulo dentro del conductor**. Si no
  fuese así, las cargas se moverían en su interior, y la situación exige que
  estén en reposo.
- ¿Dónde se ubican las cargas?. En la superficie, y distribuidas de manera que
  en el interior del conductor el campo eléctrico se anule.
- En la zona exterior inmediata a la superficie el campo eléctrico debe ser
  perpendicular a ella, dado que si tuviera una componente tangencial, la misma
  provocaría que las cargas superficiales se moviesen en respuesta a la fuerza
  tangencial resultante.
- **En un conductor en equilibrio, en su superficie el campo eléctrico es
  perpendicular.**
- La dirección del campo será hacia fuera si las cargas superficiales son
  positivas, caso contrario, hacia adentro.

## Forma diferencial de la Ley de Gauss

Ley de Gauss

```math
\oint\vec E\cdot\overrightarrow{ds}=\frac{q_{int}}{\varepsilon_o}=\frac1{\varepsilon_o}\oint\rho\,dV
```

Teorema de la Divergencia

```math
\oint\vec E\cdot\overrightarrow{ds}=\oint\vec\nabla\cdot\vec E\,dV
```

V arbitrario

```math
\oint\vec E\cdot\overrightarrow{ds}=\oint\vec\nabla\cdot\vec E\,dV=\frac1{\varepsilon_o}\oint\rho\,dV
```

```math
\vec\nabla\cdot\vec E=\frac\rho{\varepsilon_0}
```

Ecuación diferencial de Gauss

## Procedencia y observaciones de transcripción

- Original:
  `2019/1er Parcial/2018 UT I - Fuerza Eléctrica y Campo Elécrtico.pdf`, páginas
  41, 42 de 42.
- SHA-256: `326bb078ddbf25b43f166e198c175106027b686dde0d0ea9688c025795f46ca7`.
- El nombre del archivo indica 2018; ubicación canónica 2019. No consta autor ni
  fecha completa en estas páginas.
- Herramientas: PyMuPDF4LLM y Poppler para extracción; todas las expresiones y
  figuras cotejadas visualmente. Medios por recorte/render PyMuPDF; la captura
  de fórmulas y la figura oculta de líneas se recuperan desde sus franjas raster
  originales.
- Cubre la inferior de 41 y ambas de 42. Se conserva el símbolo de integral
  cerrada que el original usa también con dV, sin sustituirlo silenciosamente
  por integral de volumen. Se mantienen los subíndices o y 0 distintos.
