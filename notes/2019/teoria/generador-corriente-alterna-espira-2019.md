# Generador de corriente alterna y espira rotante

Unidad Temática VII — Electromagnetismo

## Rotating-Coil Generator

![Dos vistas de una bobina en un campo B, etiqueta coil](../../../resources/2019/fenomenos-induccion/rotating-coil.png)

Rotate coil: “change $`\Phi_B`$, induce $`\mathcal E`$”

Si tenemos N espiras de área A rotando con velocidad angular ω constante en un
campo B, el flujo magnético será

![Espiras de área A rotando a velocidad omega en un campo B](../../../resources/2019/fenomenos-induccion/espiras-rotando.png)

```math
\theta=\omega t\quad(M.C.U)
```

```math
\phi_B=\vec B\cdot\vec A=BA\cos(\theta)=BA\cos(\omega t)
```

```math
\varepsilon=-N\frac{d\phi_B}{dt}=NBA\omega\sin(\omega t)
```

```math
\varepsilon_{max}=NBA\omega\Rightarrow\varepsilon=\varepsilon_{max}\sin(\omega t)
```

Fem alterna

Ejemplo: Produccion de energía eléctrica en una central hidroeléctrica

## Generador de corriente alterna

![Esquema del generador de ca, anillos, escobillas, rotor y gráfica de fem](../../../resources/2019/fenomenos-induccion/generador-alterna.png)

```math
\varepsilon(t)=\varepsilon_{max}\sin(\omega t)
```

(a): Esquema de un generador de ca. Se induce una fem en la espira rotante. El
circuito se cierra a través de un circuito externo (lámpara). (b): Gráfica la
fem en función del tiempo.

El generador es un dispositivo que convierte la energía mecánica del rotor
externo en energía eléctrica

![Imagen estática: agua mueve el rotor, imán N S, bobina y lámpara](../../../resources/2019/fenomenos-induccion/generador-hidraulico.png)

![Esquema y gráfica repetidos en la página 24](../../../resources/2019/fenomenos-induccion/generador-alterna.png)

```math
\varepsilon(t)=\varepsilon_{max}\sin(\omega t)
```

Que pasaría si saco la lámpara y pongo una batería en su lugar

![Esquema estático de espira entre polos N y S y batería](../../../resources/2019/fenomenos-induccion/generador-bateria.png)

## Procedencia y observaciones de transcripción

- Original:
  `2019/2do Parcial/2019 UT VII - Fenómenos de Inducción Electromagnética.pdf`,
  páginas 20–25 de 67. Fecha impresa: 14/05/2019.
- SHA-256: `cbefa338a0f56f56079880a84f05a963257a6473febd8da50f944a67f2210a8f`.
- Herramientas: PyMuPDF4LLM, Poppler y recortes PyMuPDF; páginas, fórmulas y
  figuras del tramo cotejadas visualmente. No se añaden respuestas a preguntas
  vacías.
- Se transcriben los símbolos de las láminas inglesas y se conservan las
  imágenes estáticas del PDF. El esquema repetido de páginas 22 y 24 se conserva
  con su ecuación. La pregunta sobre la batería no tiene respuesta escrita.
