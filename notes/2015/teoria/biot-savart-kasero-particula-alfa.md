# Biot–Savart — Anibal Kasero: partícula alfa

## Enunciado

Una partícula α (núcleo de He) recorre una trayectoria circular de radio0,45m en
un B =1,2Wb/m². Calcular:

a) Su velocidad.

b) Su período de revolución.

c) Su energía cinética en eV.

d) La d.d.p. bajo la cual tendría que ser acelerada para obtener esa energía
cinética.

Datos:

```math
m_p=1{,}67\times10^{-27}\;\mathrm{kg}\qquad;
q_p=1{,}6\cdot10^{-19}\;\mathrm C\qquad;
1\;\mathrm{eV}=1{,}6\cdot10^{-19}\;\mathrm J
```

## a) Velocidad

Nuestra partícula se mueve en una trayectoria circular debido al campo magnético
$`\vec B`$. La fórmula $`\vec F=m\vec a`$ queda idéntica a la que escribimos en
último lugar en el ejercicio anterior:

```math
qvB=\frac{mv^2}R
```

(aceleración centrípeta)

Fácilmente despejamos la velocidad:

```math
v=\frac{qRB}m
```

La carga de la partícula α es dos veces la carga de un protón

```math
q=2\cdot1{,}6\cdot10^{-19}\;\mathrm C=3{,}2\cdot10^{-19}\;\mathrm C
```

Mientras que la masa de una partícula α es cuatro veces la masa de un protón:

```math
m=4\cdot1{,}67\cdot10^{-27}\;\mathrm{kg}=6{,}68\cdot10^{-27}\;\mathrm{kg}
```

Ya tenemos todos los datos para hallar la velocidad:

```math
v=\frac{3{,}2\cdot10^{-19}\;\mathrm C\cdot0{,}45\;\mathrm m\cdot
1{,}2\;\mathrm{Wb}/\mathrm m^2}{6{,}68\cdot10^{-27}\;\mathrm{kg}}
=2{,}6\cdot10^7\;\mathrm m/\mathrm s
```

## b) Período

El período será el tiempo que demora en dar una vuelta y podemos hallarlo muy
fácilmente con la fórmula:

```math
d=vT
```

(distancia = velocidad × tiempo)

La distancia será una vuelta, $`d=2\pi R`$ y entonces:

```math
2\pi R=vT\quad\longrightarrow\quad T=\frac{2\pi R}v
=\frac{6{,}28\cdot0{,}45\;\mathrm m}{2{,}6\cdot10^7\;\mathrm m/\mathrm s}
```

Tenemos el período:

```math
T=1{,}1\cdot10^{-7}\;\mathrm s
```

## c) Energía cinética

```math
E_c=\frac12mv^2
```

```math
E_c=\frac12\cdot6{,}68\cdot10^{-27}\;\mathrm{kg}
\left(2{,}6\cdot10^7\;\mathrm m/\mathrm s\right)^2
=2{,}26\cdot10^{-12}\;\mathrm J
```

Pasamos a eV con la conversión dato:

```math
1\;\mathrm{MeV}=1\cdot10^6\;\mathrm{eV}\quad\longrightarrow\quad E_c=14\;\mathrm{MeV}
```

## d) Diferencia de potencial

Pensamos que esta energía es producida por una diferencia de potencial hacemos,

```math
E_c=qV\quad\longrightarrow\quad2{,}26\cdot10^{-12}\;\mathrm J
=3{,}2\cdot10^{-19}\;\mathrm C\cdot V
```

```math
V=7\cdot10^6\;\mathrm V
```

## Procedencia

- Original: `2015/Resueltos Fisica II Anibal Kaseros Ley de Biot-Sabat.pdf`,
  página52 desde el segundo enunciado, página53 y comienzo54 hasta el separador.
  SHA-256: `b4aeb8cc9f1fa04835d4817a067976cc3d3c07d57e18ca5dabd898b67e09d41e`.
- OCR español auxiliar y cotejo visual completo. Ecuaciones y redondeos del
  manuscrito conservados sin recalcular; esta solución pertenece a la fuente.
- La numeración inicial está retocada. La fuente pasa de julios a MeV sin
  escribir otro paso intermedio; no se añade una cuenta en eV.

[Anterior: masa ion](biot-savart-kasero-masa-ion.md) ·
[Siguiente: positron helice](biot-savart-kasero-positron-helice.md)
