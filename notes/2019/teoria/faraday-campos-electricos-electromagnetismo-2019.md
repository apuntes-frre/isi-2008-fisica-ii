# Generalización de Faraday y campos eléctricos: versión Electromagnetismo

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
\phi_B=\int_S\vec B\cdot\overrightarrow{dA}
```

```math
\varepsilon=\oint_C\vec E\cdot\overrightarrow{dl}=-\frac{d\phi_B}{dt}=-\frac d{dt}\left(\int_S\vec B\cdot\overrightarrow{dA}\right)
```

E es un campo no conservativo generado por un campo magnético variable

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

## Procedencia y observaciones de transcripción

- Original: `2019/2do Parcial/2019 UT VII Electromagnetismo.pdf`, páginas 35–37
  de 62. No consta fecha impresa; 2019 es del nombre del archivo.
- SHA-256: `eff3447774cadfcb2726a6caabbe8e257782276fce3e67dda465673d5ef67a6a`.
- Herramientas: PyMuPDF4LLM, Poppler y recortes PyMuPDF; páginas, expresiones y
  figuras del tramo cotejadas visualmente.
- Se conserva la integral simple de superficie del original. Este tramo no
  contiene el desarrollo diferencial ni las preguntas de la otra versión de
  Fenómenos de Inducción.
