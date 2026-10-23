# Resumen de Física II — modelo clásico de un conductor

Suponga un conductor como un arreglo de átomos con electrones libres. En
ausencia de un campo eléctrico, los electrones de conducción se mueven al azar a
través del conductor. Cuando es aplicado un campo eléctrico, los electrones
libres se arrastran lentamente en una dirección opuesta a la del campo
eléctrico, con una rapidez de arrastre promedio $`v_d`$ . En el modelo se hacen
las siguientes suposiciones:

1. El movimiento del electrón después de una colisión es independiente de su
   movimiento antes de la colisión.

1. La energía adquirida en exceso por los electrones en el campo eléctrico se
   pierde en los átomos del conductor cuando chocan electrones y átomos, (hace
   que la temperatura del conductor aumente)

Cuando un electrón libre de masa $`m_e`$ y carga q = -e se somete a un campo
eléctrico E experimenta una fuerza $`\vec F=q\vec E`$ . Para calcular su
aceleración se utiliza la segunda ley de Newton

```math
\vec a=\frac{\sum\vec F}{m}=\frac{q\vec E}{m_e}
```

Ya que el campo eléctrico es uniforme, la aceleración del electrón es constante.
Si $`v_i`$ es la velocidad inicial del electrón en el instante posterior a una
colisión (t=0), la velocidad del electrón en un tiempo muy breve t posterior
(antes de la siguiente colisión) es

```math
\vec v_f=\vec v_i+\vec a t=\vec v_i+\frac{q\vec E}{m_e}t
```

Si supone que las velocidades iniciales están distribuidas aleatoriamente sobre
todos los posibles valores, el valor promedio de vi es cero. El valor promedio
del segundo término de la ecuación (1) es $`(q\vec E/m_e)\tau`$ , donde τ es el
intervalo de tiempo promedio entre colisiones sucesivas. Ya que el valor
promedio de vf es igual a la velocidad de arrastre

```math
\vec v_{f,\mathrm{prom}}=\vec v_d=\frac{q\vec E}{m_e}\tau
```

El valor de τ depende del tamaño de los átomos del metal y el número de
electrones por unidad de volumen. Con esta expresión podemos reescribir la
ecuación de la densidad de corriente

```math
J=nqv_d=\frac{nq^2E}{m_e}\tau
```

Al comparar esta expresión con la ley de Ohm $`J=\sigma E`$ , se obtienen las
siguientes correspondencias para conductividad y resistividad de un conductor:

```math
\sigma=\frac{nq^2\tau}{m_e}
```

```math
\rho=\frac1\sigma=\frac{m_e}{nq^2\tau}
```

## Procedencia y observaciones

- Original: `2015/Resumen-Fisca-2.pdf`, páginas [20, 21]; sectores delimitados
  por encabezados. SHA-256:
  `b9903f972224365c1a74b5d2732c9a34675c9b719da4c9c2d28e4a0f34e0b0cc`.
- PyMuPDF4LLM, Poppler y cotejo visual completo de los sectores. Ecuaciones de
  imagen transcritas a LaTeX.
- Se conserva la referencia a ecuación(1) aunque la fórmula no lleva número
  visible.
