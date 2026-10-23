# Resumen de Física II — primer principio y transformaciones

## Primer principio Expresión matemática

La primera ley de la termodinámica es un caso especial de la ley de conservación
de energía que describe procesos que sólo cambian la energía interna y las
únicas transferencias de energía son mediante calor y trabajo:

```math
\Delta E_{\mathrm{int}}=Q+W
```

Una consecuencia importante de la primera ley de la termodinámica es que existe
una cantidad conocida como energía interna cuyo valor está determinado por el
estado del sistema. Por lo tanto, la energía interna es una variable de estado.

Cuando un sistema se somete a un cambio infinitesimal de estado en el que una
cantidad pequeña de energía dQ se transfiere mediante calor y una cantidad
pequeña de trabajo dW se invierte, la energía interna cambia en una cantidad
pequeña $`dE_{int}`$ . Debido a eso para procesos infinitesimales es posible
expresar la primera ley como

```math
dE_{\mathrm{int}}=dQ+dW
```

Casos especiales:

- Un **sistema aislado** no interactúa con sus alrededores. Por lo tanto no
  existen transferencia de energía por calor y el trabajo consumido en el
  sistema es cero; por tanto, la energía interna permanece constante.

- Un sistema que intercambia energía con su entorno, que comienza y termina en
  el mismo estado ( **Proceso cíclico** ). El cambio en la energía interna debe
  ser cero, por lo tanto, la energía Q agregada al sistema debe ser igual al
  negativo del trabajo W consumido en el sistema durante el ciclo.

```math
\Delta E_{\mathrm{int}}=0\quad\text{y}\quad Q=-W
```

En un diagrama PV, un proceso cíclico aparece como una curva cerrada.

- Una transformación donde W=0, $`\Delta E_{int}=Q`$

- Una transformación donde Q=0. $`\Delta E_{int}=-W`$

## Transformaciones: Adiabáticas, Isócoras e Isobáricas

Un proceso adiabático es aquel durante el cual no entra ni sale energía del
sistema por calor (aislado térmicamente); Q=0. Al aplicar la primera ley de la
termodinámica a un proceso adiabático se obtiene

```math
\Delta E_{\mathrm{int}}=W\;(\text{proceso adiabático})
```

Este resultado muestra que si un gas se comprime adiabáticamente de modo que W
sea positivo, en tal caso $`\Delta E_{int}`$ es positivo y la temperatura del
gas aumenta. Por lo contrario, la temperatura de un gas disminuye cuando el gas
se expande adiabáticamente.

Un proceso isobárico es aquel que presenta una presión constante, (el pistón
puede moverse libremente para estar en equilibrio)

```math
W=-P(V_f-V_i)\;(\text{proceso isobárico})
```

Un proceso isocórico es aquel en el cual el volumen es constante, (el pistón se
encuentra fijo). Al no cambiar el volumen, el trabajo es cero, por lo tanto,
toda la energía que se agregue mediante calor permanece en el sistema como un
aumento en su energía interna

```math
\Delta E_{\mathrm{int}}=Q\;(\text{proceso isovolumétrico})
```

## Procedencia y observaciones

- Original: `2015/Resumen-Fisca-2.pdf`, páginas [77]; sectores delimitados por
  encabezados. SHA-256:
  `b9903f972224365c1a74b5d2732c9a34675c9b719da4c9c2d28e4a0f34e0b0cc`.
- PyMuPDF4LLM, Poppler y cotejo visual completo de los sectores; ecuaciones de
  imagen transcritas a LaTeX, figuras originales preservadas.
- Se conserva ΔEint=−W del caso Q=0 aunque la expresión adiabática del mismo
  original dice ΔEint=W.
