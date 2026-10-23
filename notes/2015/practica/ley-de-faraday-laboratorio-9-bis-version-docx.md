# Trabajo de laboratorio Nº 9 bis: Ley de Faraday, versión DOCX

**OBJETIVOS:** Verificar la ley de Faraday y relación con el flujo magnético

## Resumen

Se presenta una experiencia que permite verificar la ley de Faraday y calcular
el flujo magnético. A partir de la ley de Faraday, se hace la fundamentación
teórica que justifica la relación entre fem inducida con el flujo magnético de
un imán.

La verificación experimental se logra haciendo oscilar un imán en el interior de
una bobina y se registra la fem inducida en la misma.

## Equipamiento necesario

Para una estación de trabajo

- 1 Soporte universal
- 1 Resorte
- 1 Imán
- 1 GLX Pasco configurado como voltímetro
- 1 Pendriver ( traer)

Para hacer el tratamiento de datos

- 1 PC más con utilitario tipo planilla de cálculo.

## Fundamentos teoricos

La ley de Faraday establece que las variación del flujo magnético en el tiempo,
a través de una espira es igual a la fuerza electromotriz generada en ella con
signo contrario, es decir

```math
e(t)=-\frac{d\varphi}{dt}
```

(1)

Entonces se puede

```math
d\varphi=-e(t)dt
```

(2)

Integrando se obtiene el flujo magnético

```math
\int_0^{\varphi}d\varphi=-\int_0^t e(t)dt
```

(3)

Entonces

```math
\varphi(t)=-\int_0^t e(t)dt
```

(4)

Si el registro de $`e(t)`$ es discreto y no continuo entonces $`e(t_k)`$ para
$`t_k`$ con $`k=0,1,2\ldots`$ Entonces se puede reescribir la integral

```math
\varphi(t_k)=-e(t_k)\Delta t_k
```

(5)

## Esquema del montaje

![Montaje: soporte, resorte, imán, bobina y GLX](../../../resources/2015/ley-de-faraday-montaje.png)

## Marcha de la experiencia

Luego de montar los elementos de acuerdo al esquema, Se hace oscilar el imán en
el interior de la bobina, provocando una variación del flujo magnético en la
misma que genera una fuerza electromotriz inducida $`e_k`$, la misma es
registrada en forma automática en cada instante $`t_k`$ con el GLX y con estos
datos se construye la siguiente tabla:

<!-- markdownlint-disable MD060 -->

| N | $`t_k`$ | $`e_k`$ | $`\varphi_k=e_k(t_k-t_{k-1}`$ |
| -- | -- | -- | -- |
|  |  |  |  |
|  |  |  |  |

<!-- markdownlint-enable MD060 -->

La última columna debe calcular.

## Procesamiento de datos

a) Haga una representación gráfica con los datos $`e(t)`$ y (t). b) Determine
gráficamente el período.

## Analisis de los resultados

a) Justifique por que la señal es periódica y de quien depende. b) Interprete
los picos positivos y negativos c) A que le atribuye que la señal no sea
perfectamente sinusoidal d) El área de $`e(t)`$ con qué está relacionado y cómo.

## Nota de transcripción

Versión DOCX independiente: integrales definidas, procedimiento más extenso y
tabla de dos filas. Se conserva la falta de signo menos y de paréntesis de
cierre en el encabezado de la última columna, y la ausencia de φ antes de (t) en
procesamiento. No se corrigen silenciosamente. El montaje coincide visualmente
con el de la versión PDF y se referencia la misma figura.

[Procedencia y comprobaciones](../../../resources/2015/fuentes.md).
