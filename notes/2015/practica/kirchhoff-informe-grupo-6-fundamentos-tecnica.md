# Leyes de Kirchoff — informe del grupo 6: fundamentos y técnica

LABORATORIO Nº 6 Leyes de Kirchoff

![Fotografía de portada del grupo en el laboratorio](../../../resources/2015/kirchhoff-informe-grupo-6/grupo-laboratorio.png)

CARRERA: Ingeniería en Sistemas de la Información

CATEDRA: Física II

GRUPO N°: 6

INTEGRANTES:

- CARDOZO, Edgar Oscar
- DIEZ, Gabriel Fernando
- FERREYRA, Eduardo
- MATIJASEVIC, Emerson Gabriel
- PÉREZ, Milagros

## TRABAJO DE LABORATORIO Nº 6

TEMA: LEYES DE KIRCHOFF

### OBJETO DE LA EXPERIENCIA

Comprobación experimental de las Leyes de Kirchhoff.

### FUNDAMENTOS TEORICOS

Para averiguar cómo se distribuyen las corrientes en una red de conductores se
recurre a las leyes de Kirchoff. Antes de enunciarlas recordemos lo que se
entiende por nudo, rama y malla en una red.

NUDO: Todo punto donde convergen tres o más conductores.

RAMA: Todos los elementos (resistencias, generadores,....) comprendidos entre
dos nudos adyacentes.

MALLA: Todo circuito cerrado que puede ser recorrido volviendo al mismo punto de
partida sin pasar dos veces por el mismo elemento.

Evidentemente la intensidad de corriente será la misma en cada uno de los
elementos de una rama.

Para los nudos y las mallas tenemos las siguientes leyes:

### PRIMERA LEY DE KIRCHOFF (Ley de Nudos)

“La suma algebraica de las corrientes que concurren a un nudo es nula”

```math
\sum I=0
```

Considerando positivas las intensidades que se dirigen al nudo y negativas las
que parten del mismo.

### SEGUNDA LEY DE KIRCHOFF (Ley de Mallas)

“La suma algebraica de las f.e.m. en una malla cualquiera menos la caída de
tensión en los elementos de la misma malla es igual a cero”

```math
\sum E-\sum R.I=0
```

Para aplicar esta segunda ley, será preciso asignar un sentido convencional de
circulación positiva para cada malla, y considerar positivas las intensidades y
F.e.m. que concuerdan con dicho sentido convencional y negativas las que no
concuerdan.

### CIRCUITO AEMPLEAR

![Circuito original con fuentes E1 y E2, resistencia variable R, R1 a R4, amperímetros, nodos A a G y B prima, corrientes i1 a i3 y mallas I y II](../../../resources/2015/kirchhoff-informe-grupo-6/circuito-experimental.png)

## TÉCNICA OPERATIVA

### VERIFICACIÓN DE LAS LEYES DE NUDOS

1.- Se selecciona un valor de R1 con el multímetro en la escala conveniente
ajustando el cero del óhmetro para la escala elegida.-

Con el circuito abierto y las puntas del óhmetro en AC se calibra el valor de
R.-

2.- Para las lecturas de las tres corrientes se coloca el multímetro en la
escala apropiada como amperímetro intercalándolo en cada rama como se observa en
la figura.-

3.- Luego se repite el proceso para otros valores de R y se completa la tabla
siguiente:

| Pos. | R | i1 | i2 | i3 | i1+i2+i3 |
| -- | -- | -- | -- | -- | -- |
| 1 |  |  |  |  |  |
| 2 |  |  |  |  |  |
| 3 |  |  |  |  |  |

### VERIFICACIÓN DE LAS LEYES DE MALLA

1.- Para los mismos valores de R medir con el voltímetro la tensión en cada uno
de los elementos del circuito (resistencias y fem) .-

Con el multímetro en Vdc seleccionando la escala conveniente y las puntas en C y
D se lee la tensión en la resistencia R2, de igual manera se procede con las
demás resistencias:

R1= en A y C , R3= en E y B , R4= en C y F , R5= en G y B

2.- Teniendo en cuenta el sentido de circulación de las corrientes, completar la
siguiente tabla asignandoun sentido de recorrido a las dos mallas tal cual se
muestra en la figura:

| Pos | E1 | E2 | Vac | Vcd | Veb | Vbg | Vfc | Vac+Vcd+Veb | Vcd+Veb+Vbg+Vfc |
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
| 1 |  |  |  |  |  |  |  |  |  |
| 2 |  |  |  |  |  |  |  |  |  |
| 3 |  |  |  |  |  |  |  |  |  |

38

3.- Realice los cálculos teóricos para los tres casos planteados y compare con
los obtenidos en forma práctica.

### Datos

E1= medir

E2= medir

R = medir

```math
R1=2{,}7\,\mathrm{k}\Omega
```

```math
R2=3{,}3\,\mathrm{k}\Omega
```

```math
R3=1{,}5\,\mathrm{k}\Omega
```

```math
R4=2{,}2\,\mathrm{k}\Omega
```

4.- Utilizando el programa Workbencho similar arme el mismo circuito.

Justifique las diferencias, si las hubiere.

## Procedencia y alcance

- Original: `2015/L6 Kirchoff G6 Aprobado.pdf`, páginas 1–4 de 20. SHA-256:
  `534403fde9ec3209246d64553b98096c417d8f500a5a5cc4424914482ac9ac79`.
- PyMuPDF4LLM y Poppler contrastados con las cuatro páginas renderizadas. Las
  sumatorias se recuperaron por lectura visual porque la extracción pierde sus
  letras. Se conservaron la fotografía y el circuito original; este último está
  dividido en bandas en el PDF y se renderizó completo, sin redibujarlo.
- Se conservan las grafías Kirchoff/Kirchhoff, «AEMPLEAR», «asignandoun»,
  «Workbencho» y el número suelto 38 al pie de la segunda tabla. No se corrigen
  silenciosamente los nombres de resistencias: el circuito rotula R y R1–R4,
  mientras las instrucciones mencionan R1–R5 y las conexiones citadas arriba.
- Ambas tablas tienen tres filas de posiciones y campos de medición vacíos; no
  se completan con resultados posteriores. Las solicitudes de medición, cálculo
  y simulación se conservan sin resolver.
- La carpeta es 2015; estas páginas no tienen fecha impresa. Restan las páginas
  5–20 del informe, con hoja manuscrita, resultados, cálculos y simulaciones.
