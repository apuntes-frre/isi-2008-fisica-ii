# Fuerza de Lorentz y movimiento circular y helicoidal

Unidad Temática V — Fuerzas Magnéticas sobre cargas y elementos de corriente

## Movimiento de una carga con E y B estacionarios

![Carga positiva entre placas, campos E B y fuerzas opuestas Fe y Fm](../../../resources/2019/fuerzas-magneticas/campos-cruzados.png)

Los campos E y B desvían ambos las trayectorias de las cargas en movimiento,
pero lo hacen de modos diferentes. Fe es paralela a E y Fm es perpendicular a v.
La dirección y sentido de Fm esta dada por el producto vectorial (v x B). En la
figura se suponen campos homogéneos.

```math
\begin{cases}\overrightarrow{Fe}=q\vec E\\\overrightarrow{Fm}=q\vec v\times\vec B\end{cases}\Rightarrow\vec F=\overrightarrow{Fe}+\overrightarrow{Fm}=q\left[\vec E+\vec v\times\vec B\right]
```

Fuerza de Lorentz

## Partícula con carga q y velocidad v perpendicular a B uniforme

![Órbita circular de una carga positiva, fuerzas centrípetas y B entrante](../../../resources/2019/fuerzas-magneticas/movimiento-circular.png)

```math
\sum F=ma_c\qquad\begin{cases}\sum F=F_B=qvB\\a_c=\dfrac{v^2}r\end{cases}
```

```math
qvB=\frac{mv^2}r\qquad r=\frac{mv}{qB}
```

Frecuencia ciclotrón

```math
\omega=\frac vr=\frac{qB}m\Rightarrow T=\frac{2\pi}{\omega}=\frac{2\pi r}v=\frac{2\pi m}{qB}
```

V permanece constante en módulo => M.C.U.

## V forma un ángulo θ con B

![Componentes de v paralela y perpendicular a B y trayectoria helicoidal](../../../resources/2019/fuerzas-magneticas/movimiento-helicoidal.png)

Componentes de la velocidad, paralela y perpendicular al campo magnético B

```math
v_{//}=v\cos(\theta)\qquad v_\perp=v\mathop{\mathrm{sen}}\nolimits(\theta)
```

La componente paralela no es afectada por la fuerza magnética (MRU)

```math
F_\perp=qv_\perp B=ma_t=m\frac{v_\perp^2}R\Rightarrow R=\frac{mv_\perp}{qB}=\frac{mv}{qB}\mathop{\mathrm{sen}}\nolimits(\theta)
```

Frecuencia ciclotrón

```math
\omega=\frac{v_\perp}R=\frac{qB}m
```

periodo

```math
T=\frac{2\pi}{\omega}
```

```math
v_{//}\text{ es constante}\qquad x=v_{//}t=v\cos(\theta)\,t\qquad\mathrm{Paso}=v\cos(\theta)\,T
```

Superposición de un MCU en el plano zx y un MRU en la dirección x

El movimiento en el plano x-y es una circunferencia de radio R, ω es la
velocidad angular (Cte), por lo que el movimiento es un MCU. A ω se la denomina
frecuencia ciclotrón. En la dirección z tenemos que la velocidad es constante =>
MRU. El movimiento compuesto resulta en un helicoide. El periodo del MCU es:

```math
T=\frac{2\pi}{\omega}=\frac{2\pi m}{qB_z}
```

El paso del helicoide es el espacio que recorre en la dirección z en un periodo
T:

```math
z(t=T)=v_{0z}T=\frac{2\pi m v_{0z}}{qB_z}
```

## Procedencia y observaciones de transcripción

- Original:
  `2019/2do Parcial/2019 UT V - Fuerzas Magnéticas sobre cargas y elementos de corriente.pdf`,
  páginas 17–20 de 42.
- SHA-256: `383fdb6f46e1627fbe65cf259b89a480bd4b4cc61821cbfc466fa3e4a63ceb29`.
  2019 corresponde al nombre del archivo; no consta fecha impresa en estas
  páginas.
- Herramientas: PyMuPDF4LLM, Poppler y recortes PyMuPDF; páginas, expresiones y
  diagramas del tramo cotejados visualmente. No se añaden soluciones.
- Se mantienen a_t de la expresión de página 19 y sus referencias a plano
  zx/dirección x, aunque la página 20 use plano x-y/dirección z. No se corrigen
  los ejes ni los enunciados.
