# Resumen de Física II — generalización de la ley de Faraday

Un flujo magnético cambiante induce una fem y una corriente en una espira
conductora, por lo tanto produce un campo eléctrico que aun existe en ausencia
de la espira conductora. Considere una espira conductora de radio r situada en
un campo magnético uniforme perpendicular al plano de la espira. Si el campo
magnético cambia con el tiempo, se induce en la espira una fem, que implica la
presencia de un campo eléctrico inducido E, que debe ser tangente a la espira.
El trabajo invertido por el campo eléctrico al mover una carga de prueba q una
vez alrededor de la espira es igual a qƐ, o qE(2πr) puesto que la fuerza
eléctrica que actúa sobre la carga es qE y la circunferencia de la espira es
2πr. Por lo tanto,

```math
q\mathcal E=qE(2\pi r)
```

```math
E=\frac{\mathcal E}{2\pi r}
```

```math
E2\pi r=-\frac{d\phi_b}{dt}
```

Es posible que E no sea constante, y la trayectoria puede no ser circular, por
lo que la fem correspondiente a cualquier trayectoria cerrada puede expresarse
como $`\mathcal E=\oint E\cdot ds`$ . Por eso, la ley de la inducción de Faraday
puede escribirse de la forma general

```math
\oint\vec E\cdot d\vec s=-\frac{d\Phi_B}{dt}
```

El campo eléctrico inducido E es un campo no conservativo generado por un campo
magnético cambiante.

## Procedencia y observaciones

- Original: `2015/Resumen-Fisca-2.pdf`, páginas [36]; sectores delimitados por
  encabezados. SHA-256:
  `b9903f972224365c1a74b5d2732c9a34675c9b719da4c9c2d28e4a0f34e0b0cc`.
- PyMuPDF4LLM, Poppler y cotejo visual completo de los sectores; ecuaciones de
  imagen transcritas a LaTeX, figuras originales preservadas.
- Se conserva φb minúscula en el desarrollo frente a ΦB de la fórmula final.
