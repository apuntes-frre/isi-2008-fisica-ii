# Fuerza Magnética sobre elementos de corriente — informe del grupo 6: teoría y técnica

## INTRODUCCION TEORICA

Sobre un elemento de corriente $`I\,\overrightarrow{dl}`$, que está colocado en
una región donde existe un campo magnético $`\vec{B}`$ se produce una fuerza
elemental dada por

```math
d\vec{F}=I\,\overrightarrow{dl}\wedge\vec{B}\qquad(1)
```

1.- Vamos a usar la expresión (1) en el dispositivo de la figura Nº1, que
representa una barra recta conductora colocada en un campo Magnético
suministrado por un imán en forma de U. Cuando se hace circular corriente por la
barra aparece una fuerza de intensidad

```math
F=ILB\qquad(2)
```

![Figura Nº1 original: barra, imán en U, fuerza y corriente entrando al plano de la hoja](../../../resources/2015/fuerza-magnetica-barra.png)

Siendo L el ancho de la región donde existe campo.

Esta fuerza actúa mientras la barra se halla en el campo, si la intensidad de
esta fuerza es suficiente para vencer el rozamiento, la barra se desplaza.

![Figura Nº2 original: espira de lados a y b, imán y contactos](../../../resources/2015/fuerza-magnetica-espira-montaje.png)

2.- Consideremos ahora el dispositivo de la figura Nº2, cuando circula corriente
por la espira de lados a y b actúa una fuerza que la aparta de la posición
vertical, haciendo que forme un ángulo, para encontrar la forma este ángulo
depende de los otros parámetros que están involucrados, estudiemos el diagrama
de fuerzas de la figura N º3.

De la cual, se desprende la condición de equilibrio

```math
M(O,P)+M(O,Fm)=0\qquad(3)
```

Donde

```math
P=\mu(2a+b)g\qquad(4)
```

Siendo $`\mu`$ la densidad de masa por unidad de longitudy

```math
Fm=ILB\qquad(5)
```

La (3) puede rescribirse como

```math
Yc\,P\mathop{\mathrm{sen}}\nolimits\theta-a\,Fm\cos\theta=0\qquad(6)
```

Donde Yc es la distancia del eje de suspensión al centro de masa de la espira y
viene dada por:

```math
Yc=\frac{a(a+b)}{2a+b}\qquad(7)
```

Reemplazando (4), (5) y la (7) en la (6) resulta

```math
\mathop{\mathrm{tg}}\nolimits\theta=\frac{ILB}{(a+b)a\mu g}\qquad(8)
```

Para ángulos pequeños resulta

```math
\theta\approx\frac{ILB}{(a+b)a\mu g}\qquad(9)
```

De la (9) se desprende que como la geometría (a, b y L), la masa por unidad de
longitud L y los campos (g y B) son constantes existe una relación lineal entre
el ángulo de inclinación de la espira respecto de la normal y la corriente que
circula por la misma, siendo este el principio de funcionamiento de los
instrumentos eléctricos de medida de aguja.

![Figura Nº3 original: eje O, a, Yc, ángulos y diagrama de fuerzas de la espira](../../../resources/2015/fuerza-magnetica-diagrama-fuerzas.png)

## DESCRIPCIÓN DEL DISPOSITIVO

Para hacer la verificación experimental de la fórmula (1), emplearemos el
dispositivo de la figura Nº4, que representa dos bases de madera que tienen cada
uno en la parte superior dos barras metálicas que actuarán de electrodos planos,
estos están conectados a través del interruptor A con una fuente de corriente
continua.

![Figura Nº4 original: bases, barra móvil, electrodos, imán, interruptor A y fuente E](../../../resources/2015/fuerza-magnetica-dispositivo.png)

Sobre los electrodos planos se apoya una barra de aluminio, recta y de sección
cilíndrica y se coloca un imán en forma de U entre las bases y de modo que, la
barra de aluminio se ubique en el centro del "gap" del imán.

Para el análisis de la intensidad de la fuerza se reemplaza la barra recta de
aluminio y se reemplaza por una espira de lados a y b de la forma
![Forma original de la espira](../../../resources/2015/fuerza-magnetica-espira-forma.png)
y se emplea el circuito de la figura Nº5.

![Figura Nº5 original: espira, reóstato R, amperímetro A y fuente E](../../../resources/2015/fuerza-magnetica-circuito.png)

Sobre el lado interno de una de las bases está pegado un semicírculo graduado
que permite medir el ángulo de inclinación de la espira respecto de la
horizontal.

## MARCHA DE LA EXPERIENCIA

1\. Comprobación vectorial de la expresión (1):

1.1.- Haga el montaje de la figura Nº4

### PRECAUCIONES

En el montaje de la figura Nº4, debe tenerse presente que el valor de la
intensidad de corriente no debe superar el valor máximo de operación de la
fuente, de modo que basta dar pulsos (encendido y apagado) para comprobar que la
barra de aluminio se desplaza.

1.2.- Haga circular la corriente en un sentido, luego en otro: ¿Qué observa?
Dibuje los vectores correspondientes. ¿Cuáles son sus conclusiones?

1.3.-Haga circular la corriente en un sentido, y luego invertir los polos del
imán. ¿Qué observa? Dibuje los vectores correspondientes. ¿Cuáles son sus
conclusiones?

## Determinación del campo magnético de un imán natural

2.1Haga el montaje de la figura Nº 5.

2.2Mida las longitudes de la varilla según indica la figura Nº2

2.3Pese la varilla y determine su densidad lineal $`\mu`$

2.4 Variando el valor de la resistencia R del circuito de la figura Nº5, cambia
la intensidad de corriente que se registra en el amperímetro y la inclinación de
la espira respecto de la vertical empleando el semicírculo del montaje, podemos
confeccionar entonces la tabla de datos 1.

Tabla 1

<table>
<thead>
<tr><th>Corriente eléctrica I (A)</th><th>Ángulo (radianes)</th></tr>
</thead>
<tbody>
<tr><td></td><td></td></tr>
<tr><td></td><td></td></tr>
</tbody>
</table>

2.5 Realice un ajuste de curva, (por ejemplo emplee el método de cuadrados
mínimos si la gráfica se corresponde con una recta) con los mismos datos.

```math
A=\frac{N\sum xy-\sum x\sum y}{N\sum x^2-(\sum x)^2}
```

```math
B=\frac{\sum x^2\sum y-\sum x\sum y}{N\sum x^2-(\sum x)^2}
```

donde$`y(x)=Ax+B`$

2.6 Compare las pendientes de ambos métodos, indicando su significado.

## CONCLUSIÓN

Durante la primera parte de la experiencia el desplazamiento de la barra de
aluminio, en un campo magnético cuando por ella circula una corriente, ¿verifica
la expresión vectorial de la fuerza (1)? ¿Cómo lo comprueba?

Cuando se estudia la espira en el campo, que tipo de relación existe entreel
ángulo de inclinación y la intensidad I, ¿Es compatible con el desarrollo
teórico?

## Procedencia y observaciones

- Original: `2015/L8 Fza sobre elemento de cte G6 Aprobado.pdf`, páginas 3–6 de
  nueve. SHA-256:
  `fb2be56c4577a2058d5334daff09c1974e826f2fa3023bd5e6da74dcbca6a701`.
- PyMuPDF4LLM/Poppler cotejados con las cuatro páginas renderizadas. Ecuaciones
  rasterizadas recuperadas visualmente como LaTeX, sin sustituirlas por
  capturas; se conservan sus letras, denominadores, producto vectorial y
  numeración.
- Las cinco figuras numeradas y forma de la espira se cotejaron con los medios
  originales conservados de la guía y se reutilizan sin duplicar imágenes. Su
  orden de lectura sigue la exposición de este informe.
- Se conservan «la forma este ángulo», «longitudy», L como masa por unidad de
  longitud, «entreel» y la ausencia de espacio en 2.1Haga/2.2Mida/2.3Pese. El
  guion de corte «po-demos» de página 6 se reúne en «podemos».
- Se mantienen los encabezados horizontal/vertical/normal en sus respectivos
  párrafos, sin uniformarlos. El denominador de (8) y (9) incluye (a+b)aμg.
- Las sumatorias de ajuste no muestran índices: no se agregan. El numerador de B
  termina en «−ΣxΣy»; se conserva tal como aparece, sin reemplazarlo por una
  fórmula estadística corregida. «donde» aparece pegado a y(x).
- Tabla 1 tiene dos filas vacías. Las preguntas y el ajuste solicitado no se
  resuelven aquí. A diferencia de otras versiones de la guía, estas páginas no
  contienen bibliografía ni formulario nominal.
- El año de portada es 2016, aunque la carpeta sea 2015. Restan hoja manuscrita
  de página 7 y experiencias/resultados de páginas 8–9.

[Portada, objetivo y resumen](fuerza-corriente-informe-grupo-6-objetivo-resumen.md).
