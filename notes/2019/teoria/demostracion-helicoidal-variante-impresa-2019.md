# Demostración de la trayectoria helicoidal — variante impresa

> Transcripción del contenido legible de las diapositivas 40–42. `□` señala
> sectores con glifos dañados; no es una variable y no establece qué símbolo
> había allí. No se reproducen uno por uno los fragmentos de los delimitadores:
> su disposición exacta queda visible en los recortes originales. La marca «fi»
> impresa sobre algunas letras se conserva literalmente; no se convierte por
> conjetura en una flecha vectorial.

## Diapositiva 40

La velocidad v de la partícula forma un ángulo θ con el campo magnético B

```math
\overset{\mathrm{fi}}F=q(\overset{\mathrm{fi}}v\cdot\overset{\mathrm{fi}}B)=m\overset{\mathrm{fi}}a
```

```math
\overset{\mathrm{fi}}B=B_z\breve k\qquad
\overset{\mathrm{fi}}v=v_x\breve\imath+v_y\breve\jmath+v_z\breve k
```

```math
\overset{\mathrm{fi}}a=a_x\breve\imath+a_y\breve\jmath+a_z\breve k
=\frac{dv_x}{dt}\breve\imath+\frac{dv_y}{dt}\breve\jmath+\frac{dv_z}{dt}\breve k
```

La disposición matricial tiene delimitadores deteriorados:

```math
\overset{\mathrm{fi}}F=q\;\square\;
\begin{array}{ccc}
\breve\imath&\breve\jmath&\breve k\\
v_x&v_y&v_z\\
0&0&B_z
\end{array}
\;\square
=q(v_yB_z\breve\imath-v_xB_z\breve\jmath+0\breve k)
```

El sistema tiene delimitadores deteriorados; sus tres renglones legibles son:

```math
m\frac{dv_x}{dt}=qv_yB_z\qquad(1)
```

```math
m\frac{dv_y}{dt}=-qv_xB_z\qquad(2)
```

```math
m\frac{dv_z}{dt}=0\qquad(3)
```

El enlace gráfico entre los dos grupos de expresiones está deteriorado.

```math
v_y=\frac{m}{qB_z}\frac{dv_x}{dt}
```

```math
\frac{d^2v_x}{dt^2}+\square\frac{qB_z}{m}\square^{2}v_x=0\qquad(4)
```

```math
v_z=Cte
```

![Diapositiva 40 original: ejes, ecuaciones y glifos deteriorados](../../../resources/2019/fuerzas-magneticas-variante-impresa/diapositiva-40-deteriorada.png)

## Diapositiva 41

```math
\boxed{\omega=\frac{qB_z}{m}}\quad\square\quad
\frac{d^2v_x}{dt^2}+\omega^2v_x=0\qquad(6)
```

La solución general de (6) es:

```math
v_x(t)=A_1\sin(\omega t)+A_2\cos(\omega t)\qquad(7)
```

Utilizando (7) y empleando (5) obtenemos:

```math
v_y=\frac{m}{qB_z}\frac{dv_x}{dt}
```

```math
v_y(t)=A_1\cos(\omega t)-A_2\sin(\omega t)\qquad(8)
```

Para determinar las constantes necesitamos una condición inicial para v. Si en t
= 0 la velocidad es:

```math
\overset{\mathrm{fi}}v(0)=v_{0x}\breve\imath+v_{0y}\breve\jmath+v_{0z}\breve k
```

Los delimitadores del siguiente grupo están deteriorados:

```math
v_x(0)=A_2=v_{0x}
```

```math
v_y(0)=A_1=v_{0y}
```

```math
v_z(0)=v_{0z}=Cte
```

El enlace y los delimitadores del siguiente grupo también están deteriorados:

```math
v_x(t)=v_{0y}\sin(\omega t)+v_{0x}\cos(\omega t)\qquad(9)
```

```math
v_y(t)=v_{0y}\cos(\omega t)-v_{0x}\sin(\omega t)\qquad(10)
```

```math
v_z(t)=v_{0z}\qquad(11)
```

![Diapositiva 41 original: solución y condiciones iniciales deterioradas](../../../resources/2019/fuerzas-magneticas-variante-impresa/diapositiva-41-deteriorada.png)

## Diapositiva 42

Para determinar las coordenadas en función del tiempo debemos integrar las
ecuaciones de las velocidades:

Los delimitadores del grupo de coordenadas están deteriorados:

```math
x(t)=\frac{v_{0y}}{\omega}(1-\cos(\omega t))+
\frac{v_{0x}}{\omega}\sin(\omega t)\qquad(12)
```

```math
y(t)=\frac{v_{0y}}{\omega}[-1+\cos(\omega t)]+
\frac{v_{0x}}{\omega}\sin(\omega t)\qquad(13)
```

```math
z(t)=v_{0z}t\qquad(14)
```

Elevando al cuadrado (12) y (13) y sumando m.a.m y simplificando se obtiene:

```math
\square x(t)-\frac{v_{0y}}{\omega}\square^2+
\square y(t)+\frac{v_{0x}}{\omega}\square^2
=\frac{v_{0x}^{2}+v_{0y}^{2}}{\omega^2}\qquad(15)
```

Circunferencia con centro en:

```math
\square\frac{v_{0y}}{\omega},-\frac{v_{0x}}{\omega}\square\qquad(16)
```

y radio

```math
R=\frac{\sqrt{v_{0x}^{2}+v_{0y}^{2}}}{\omega}\qquad(17)
```

![Diapositiva 42 original: coordenadas y agrupación deteriorada](../../../resources/2019/fuerzas-magneticas-variante-impresa/diapositiva-42-deteriorada.png)

## Procedencia y límites de lectura

- Original: `2019/2do Parcial/UT 5 4 pag.pdf`, hoja 10 casillero 4 y hoja 11
  casilleros 1–2 (diapositivas 40–42 por orden de lectura).
- SHA-256: `134d9de661dcefd039d315a0e669b89c38bf02859d1d2d0806f15569b5006764`.
- Segunda impresión cotejada: `2019/2do Parcial/UT 5 6 pag.pdf`, hoja 7,
  casilleros 4–6; SHA-256
  `d80e499c858b45d8146a3e18152de704cefbb9d0009ea7f3717141f3543e7d9c`.
- Inspección de imágenes PDF con PyMuPDF, comparación con Poppler y los renders
  completos. No hay texto ni fuentes embebidas recuperables en estas hojas de la
  primera impresión; los defectos también aparecen en la segunda.
- Los recortes preservan los diagramas y permiten localizar cada glifo perdido.
  Las ecuaciones legibles están transcritas como LaTeX. Se mantienen el punto
  entre v y B de la primera ecuación, las marcas «fi», los versores con breve,
  la referencia a (5) sin número visible junto a la expresión, los coeficientes
  de (13) y el centro de (16), sin corregir ni rehacer la derivación.
- Pendiente: recuperar los símbolos que ocupan los sectores dañados a partir de
  una copia legible de esta impresión. No se trasladan silenciosamente flechas,
  productos vectoriales ni delimitadores de la versión de una diapositiva por
  página.
