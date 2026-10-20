# Generalización de Faraday y forma diferencial

Unidad Temática VII — Electromagnetismo

## Generalización de la ley de Faraday

Para cualquier camino cerrado la fem puede expresarse como:

```math
\varepsilon=\oint\vec E\cdot\overrightarrow{dl}
```

donde

```math
\vec E=\vec E_{inducido}+\vec E_{electrostatico}
```

En general el campo eléctrico puede ser variable y el camino una curva cerrada
de forma arbitraria. Podemos expresar la ley de Faraday como:

```math
\oint\vec E\cdot\overrightarrow{dl}=-\frac{d\phi_B}{dt}
```

E es un campo no conservativo generado por un campo magnético variable

```math
\phi_B=\iint_S\vec B\cdot\overrightarrow{dA}\Rightarrow\varepsilon=-\frac d{dt}\left(\iint_S\vec B\cdot\overrightarrow{dA}\right)
```

```math
\varepsilon=\oint_C\vec E\cdot\overrightarrow{dl}=-\frac d{dt}\left(\iint_S\vec B\cdot\overrightarrow{dA}\right)
```

Si B depende de la posición y del tiempo y el circuito C es rígido y esta en
reposo

```math
\oint_C\vec E\cdot\overrightarrow{dl}=-\iint_S\frac{\partial\vec B}{\partial t}\cdot\overrightarrow{dA}
```

Usando el Teorema de Stokes

```math
\oint_C\vec E\cdot\overrightarrow{dl}=\iint_S(\nabla\times\vec E)\cdot\overrightarrow{dA}\Rightarrow
```

```math
\iint_S(\nabla\times\vec E)\cdot\overrightarrow{dA}=-\iint_S\frac{\partial\vec B}{\partial t}\cdot\overrightarrow{dA}\Rightarrow
```

Forma diferencial de la ley de Faraday

```math
\nabla\times\vec E=-\frac{\partial\vec B}{\partial t}
```

Si B no depende del tiempo:

```math
\frac{\partial\vec B}{\partial t}=0
```

```math
\nabla\times\vec E=0
```

E es estático y conservativo

## Diferencias entre el campo eléctrico electrostático y el campo eléctrico inducido

- Los campos eléctricos inducidos no están asociados a cargas, sino a
  variaciones temporales del flujo magnético.
- Las líneas del campo eléctrico inducido son líneas cerradas, mientras que las
  líneas de campo que representan al campo eléctrico electrostático nacen en las
  cargas positivas y mueren en las negativas.
- La diferencia de potencial entre dos puntos asociada a un campo eléctrico
  electrostático es independiente del camino recorrido (campo conservativo), de
  forma que se cumple

```math
\oint\vec E\cdot\overrightarrow{dl}=0
```

Para los campos eléctricos inducidos no se puede aplicar esta expresión, ya que
la fem inducida es distinta de cero cuando varía el flujo magnético. Por lo
tanto, el campo eléctrico inducido no es un campo conservativo.

```math
\varepsilon=\oint\vec E\cdot\overrightarrow{dl}\ne0
```

Se puede hablar de fem inducida para una trayectoria determinada sin necesidad
de que ésta coincida con un circuito físico.

## Pregunta: corriente constante

Si por una espira circular, circula una corriente constante en sentido horario.

a) Se genera campo magnético?

b) Cuál es su dirección y sentido?

c) Hay flujo a través del área de la espira?

d) Hay fem inducida?

## Pregunta: corriente variable

Si por una espira circular, circula una corriente variable (aumentando en el
tiempo) en sentido horario.

a) Se genera campo magnético?

b) Cuál es su dirección y sentido?

c) Hay flujo a través del área de la espira?

d) Hay fem inducida?

## Procedencia y observaciones de transcripción

- Original:
  `2019/2do Parcial/2019 UT VII - Fenómenos de Inducción Electromagnética.pdf`,
  páginas 35–40 de 67. Fecha impresa: 14/05/2019.
- SHA-256: `cbefa338a0f56f56079880a84f05a963257a6473febd8da50f944a67f2210a8f`.
- Herramientas: PyMuPDF4LLM, Poppler y recortes PyMuPDF; páginas y ecuaciones
  del tramo cotejadas visualmente; sin soluciones añadidas.
- Se preservan las dos preguntas y sus cuatro apartados sin respuestas. La
  formulación y la comparación con el campo electrostático pertenecen al
  material original.
