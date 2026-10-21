# Calorimetría: propuesta de experiencia con agua y mate

> Fuente: `2019/lab arduino/Calorimetria.docx`. SHA-256:
> `f0a31808cb7bd769b39d18184b3e2e22345672bb2f155f51f9417e8915fb4770`. Original
> sin autor o fecha explícitos, conservado bajo 2019/lab arduino. Conversión
> Pandoc a GFM, inspección XML y PDF de LibreOffice de cuatro páginas completas
> cotejadas. No contiene medios incrustados.

**Verificar el material de X elemento averiguando su calor especifico**
utilizando tablas con valores conocidos. El experimento se realizara de la misma
manera que lo describe el laboratorio de clase, solo que utilizaremos diferentes
elementos como aluminio, cobre, hierro, madera, etc.

Buscar una ecuación en donde relaciones un intervalo de tiempo y el calor
especifico para poder averiguar, calculando el calor especifico del aluminio de
un termo cuanto tiempo podrá contener el calor del agua.

Calcular el calor especifico del agua para poder conocer la temperatura y
relacionar con el calentamiento del agua para un mate.

______________________________________________________________________

**Calor especifico:** la cantidad de energía que se debe suministrar a un gramo
de sustancia para que su temperatura aumente en un grado centígrado.

La **capacidad calorífica específica**, **calor específico** o **capacidad
térmica específica** es
una [magnitud física](https://es.wikipedia.org/wiki/Magnitud_f%C3%ADsica) que se
define como la cantidad de calor que hay que suministrar a la unidad de masa de
una sustancia
o [sistema termodinámico](https://es.wikipedia.org/wiki/Sistema_termodin%C3%A1mico) para
elevar su [temperatura](https://es.wikipedia.org/wiki/Temperatura) en una
unidad; esta se mide en varias escalas.

**Calcular el calor especifico del agua para poder conocer la cantidad de
energía (cantidad de calor) que debo suministrar al agua para un termo de mate y
obtener una temperatura ideal para el mismo.**

Se define como calor (Q) a la cantidad de energía intercambiada desde un cuerpo
mas caliente hacia uno mas frio.

Definimos la capacidad calorífica de un cuerpo o sustancia como:
$`C = \frac{\mathrm{\Delta}Q}{\mathrm{\Delta}T}`$ (1), donde
$`\mathrm{\Delta}Q`$ es la cantidad de calor que debe intercambiar para efectuar
un cambio $`\mathrm{\Delta}T`$ (donde este será la diferencia entre agua a
temperatura ambiente y la temperatura ideal para un mate).

El calor especifico definimos como $`c = \frac{C}{M}`$ (2), donde M es la masa
de agua y C la capacidad calorífica.

**Considerando que mientras mayor sea la masa de agua, mayor será la cantidad de
calor. (obtenemos grafica de** **la cantidad de calor en función del masa)**

De aquí podemos de (1) y (2) obtenemos que la cantidad de calor necesario para
elevar la temperatura de M gramos de agua es:

$`\mathrm{\Delta}Q = M\ c\ \mathrm{\Delta}T`$ (3)

## Determinar el equivalente en agua k

### Introducción

El recipiente donde se realizan las experiencias en las que se producen
variaciones de calor se llama calorímetro. Se trata de un recipiente que
contiene el líquido en el que se va a estudiar la variación del calor y cuyas
paredes y tapa deben aislarlo al máximo del exterior.

El "equivalente en agua del calorímetro " es la cantidad de agua que absorbe o
desprende el mismo calor que el calorímetro y sus accesorios.\
En esta experiencia se busca determinar el equivalente en agua del calorímetro
como experiencia previa a la determinación del calor específico de un sólido
en la parte 2 de este trabajo práctico.

En este caso se analiza el balance de energía que ocurre hasta alcanzar el
equilibrio térmico entre el agua que se encuentra en el calorímetro y el
propio calorímetro, agitador y termómetro (CAT) ambos a temperatura ambiente y
el agua calentada hasta alcanzar una temperatura previamente definida. Como el
calor específico del agua es conocido y considerando que CAT es de agua, la
única incógnita es cuanto vale esa masa ficticia de agua (k) que intercambia
la misma cantidad de calor que el CAT.

### Procedimiento

En un calorímetro de mezclas (recipiente de telgopor), se coloca una masa M de
agua a una temperatura Ti del ambiente. Por otro lado se calienta a una
temperatura conocida T una masa m de agua y luego se la vierte en el
calorímetro y se agita suavemente el recipiente hasta que alcance el equilibrio
térmico a la temperatura Tf .

Entonces, el calor que cede la masa m de agua caliente tiene que ser igual al
calor que absorbe el calorímetro de mezclas y el agua M. Por lo tanto: donde:

```math
Q_{\mathrm{abs}}=-Q_{\mathrm{ced}}
```

```math
Q_{\mathrm{abs}}=(M c_{\mathrm{H2O}}+m_c\cdot c_c+m_t\cdot c_t+m_a\cdot c_a)\cdot(\mathrm{Tf}-\mathrm{Ti})
```

```math
Q_{\mathrm{ced}}=m c_{\mathrm{H2O}}(T-\mathrm{Tf})
```

con:\
mc = masa del calorímetro, cc = calor específico del calorímetro\
mt = masa del sensor de temperatura, ct = calor específico del sensor de
temperatura ma = masa del agitador y. ca= calor específico del agitador.\
cH2O = calor específico del agua\
Tf = Temperatura final del calorímetro\
Ti= Temperatura inicial del calorímetro.\
T = Temperatura inicial de la masa m de agua\
Si llamamos k al equivalente en agua del calorímetro, donde:

```math
k=(m_c\cdot c_c+m_t\cdot c_t+m_a\cdot c_a)/c_{\mathrm{H2O}}
```

entonces:

```math
\mathbf{k =}\frac{\mathbf{m}\left(\mathbf{T}-\mathbf{Tf}\right)}{\mathbf{Tf - Ti}}-\mathbf M
```

Pasos de la Experiencia para la determinación del equivalente en agua k:

1. 1  Tomar el recipiente de telgopor (calorímetro), pesarlo en la balanza y
   etiquetarlo con el valor de su masa.

1. 2  Llenar hasta aproximadamente la mitad de su altura con agua corriente y
   volverlo a pesar. La diferencia entre esta cantidad y la del punto 1, nos da
   la masa M de agua. Sumergir el sensor de temperatura en el interior del
   líquido del recipiente

1. 3  Calentar agua en un termo hasta un valor de aproximadamente 80 C (se lo
   puede determinar con el datalogger).

1. 4  Iniciar la recolección de datos con el datalogger.

1. 5  Verter parte del agua caliente en el calorímetro teniendo cuidado de no
   llenarlo. Este procedimiento debe realizarse lo más rápido posible para
   evitar pérdidas de calor.

1. 6  Registrar la evolución de temperatura en función del tiempo hasta que
   ambas puntas sensoras registren la misma temperatura Tf. Usar el agitador
   para uniformar la temperatura.

1. 7  Determinar nuevamente el peso de este recipiente y por diferencia se
   obtiene la masa m del agua caliente .

## 2 – Determinación del calor específico de un sólido

### Introducción

Ahora usamos el equivalente obtenido para obtener con precisión el calor
específico de un sólido.\
Si a un calorímetro de equivalente en agua k conocido y con una cierta cantidad
m1 de agua en su interior a temperatura T1 se le introduce una masa m2 de un
material a temperatura T2 cuyo calor específico se desconoce, siendo
$`T_1\lt T_2`$ se tiene:

```math
Q_{\mathrm{abs}}=-Q_{\mathrm{ced}}
```

```math
Q_{\mathrm{abs}}=(m_1+k)c_{\mathrm{H2O}}\cdot(\mathrm{Tf}-T_1)
```

```math
Q_{\mathrm{ced}}=m_2c(T_2-\mathrm{Tf})
```

con c = calor específico del material ~~desconocido,~~ conocido

se tiene que:

```math
c=[(m_1+k)c_{\mathrm{H2O}}\cdot(\mathrm{Tf}-T_1)]/m_2(T_2-\mathrm{Tf})
```

despejando obtenemos:
$`\text{c}_{\text{H2O}}\text{=}\mathbf{\ }\frac{\text{c m2 (T2-Tf)}}{\text{(m1+k)(Tf-T1)}}`$

**Aplicando (3) calculo la cantidad de energia necesaria para calentar el agua
para un mate perfecto.**

## Observaciones de transcripción

Se conserva la propuesta sin resultados ni cálculos añadidos, la doble
numeración de los siete pasos, la tachadura «desconocido,» seguida de «conocido»
y las erratas del texto. Se mantienen el balance Qabs=−Qced junto a la expresión
positiva de Qced, la forma lineal con barra del despeje de c y la fórmula final
que despeja cH2O. Las definiciones e hipervínculos son los del documento. Las
páginas corresponden al PDF normalizado, no a una paginación impresa del DOCX.
