# Auditoría de transcripción de Física II

Revisión: 25/10/2026. La materia conserva límites documentales abiertos; no se
declara una transcripción íntegra sin pérdidas.

## Controles completados

- [x] Inventario canónico cotejado: 143 archivos, con sus 143 SHA-256 correctos;
  ningún archivo nuevo, ausente o alterado respecto del inventario.
- [x] 487 apuntes y 487 filas de cobertura, sin apuntes fuera del registro ni
  filas duplicadas. Las versiones se conservan por separado.
- [x] GitHub: 4896 expresiones esperadas y renderizadas; las dos notas nuevas
  tienen 29 expresiones verificadas, sin errores ni nodos sin renderizar.
- [x] Contenido legible de las diapositivas 26/40–42 de UT5 incorporado en dos
  notas, con los sectores dañados identificados y cuatro recortes como
  evidencia. Son 38 diapositivas completas y cuatro parciales, no 42
  recuperadas.
- [x] Imágenes nativas de las hojas manuscritas revisadas; no aportan una
  lectura inequívoca de los fragmentos señalados.
- [x] Duplicados de laboratorio 7, polarización, unidad 1, guía 01.1 y modelos
  de examen vinculados por SHA-256: no representan contenido docente adicional.
- [x] Páginas fuera de la asignación a apuntes de los compilados 47, 51 y 77
  contrastadas con el inventario: carátulas y páginas sin ejercicios registradas
  en sus observaciones de cobertura; no son ejercicios omitidos.
- [x] Bibliografía, curso externo, software y documentos de otras materias
  distinguidos del material docente en el inventario y la clasificación de
  complementarios. No se declara transcrito el libro de Sampallo ni el curso
  externo incluido en el CD.

## Búsqueda ampliada de fuentes

Se buscaron nombres y rutas de Física, Kirchhoff, brújula, fuerzas magnéticas,
elementos de corriente y modelos de parcial en todo `Facultad` del OneDrive
canónico. De 626 coincidencias de rutas, 143 pertenecen al inventario de Física
II. Fuera de esa carpeta, las coincidencias específicas de Física corresponden a
Física I, dos libros de Sears y los programas analíticos de Física I y II; las
restantes coincidencias de modelos de parcial pertenecen a otras materias. No se
identificó por nombre o ruta una copia alternativa de los cinco grupos
pendientes. Esta búsqueda no constituye una inspección del contenido de todos
los archivos de otras materias ni de archivos comprimidos ajenos al inventario.

El PR #2 tiene aprobado el control `Validate Transcription / content` para el
commit `f58d6692f6f41da361fba900db9d45722dc3d9a0`:
[ejecución verificada](https://github.com/apuntes-frre/isi-2008-fisica-ii/actions/runs/40152750381).
El resultado de CI valida los controles del repositorio; no resuelve las
lecturas ilegibles que se detallan a continuación.

## Bloqueos que requieren una fuente mejor o cotejo del usuario

| Material | Fragmento pendiente | Límite comprobado |
| -- | -- | -- |
| Informe de Kirchhoff, página 5 | Mallas: posición 1 Vcd/Veb/Vgb y posición 3 Vcd | Las fotografías incrustadas de 533 × 350 píxeles no permiten fijar esas cifras con certeza. |
| Informe de brújula, hoja normalizada 6 | Última cifra retocada de x para 30° | La fotografía original de 720 × 998 píxeles también conserva el retoque; no se sustituye por la tabla mecanografiada. |
| Informe de fuerza sobre corriente, página 7 | Rótulo de masa inferior y símbolo ausente de la plantilla | Fotografía original de 720 × 1280 píxeles; valor 7,5 g y cuentas legibles ya conservados, rótulo sin certeza y símbolo no representado. |

La diapositiva 26 cuenta ahora con una corrección editorial autorizada por el
usuario: sustitución de la velocidad en la energía cinética, B² en el numerador
final y notación legible. El apunte incluye una aclaración marcada con * y el
recorte original; las dos expresiones corregidas se verificaron en GitHub. Esta
intervención no recupera los glifos originales ni se extiende a las diapositivas
41–42. La diapositiva40 también quedó normalizada tras el cotejo del usuario,
sin aclaración al pie, y sus fórmulas modificadas fueron verificadas en GitHub.

El cotejo remoto de las diapositivas 41–42 quedó completado el25/10/2026. Se
normalizaron vectores y delimitadores, y se corrigieron con autorización del
usuario los coeficientes intercambiados de (13). Las derivadas y la ecuación de
circunferencia son coherentes; GitHub27/27expresiones verificado. El bloqueo de
UT5 queda resuelto mediante esta normalización y corrección, no mediante la
recuperación de glifos del PDF. Persisten los tres grupos manuscritos de la
tabla anterior.

El radio manuscrito del examen14 se transcribió como5m por indicación del
usuario, con una aclaración marcada con * que conserva la posible lectura5cm. El
original no permite confirmar la unidad: esta reserva sigue explícita en el
apunte. GitHub2/2expresiones, dato, aclaración e imágenes verificados.

## Pasos restantes

- [ ] Obtener una copia legible o una aclaración verificable de los cuatro
  grupos anteriores, manteniendo separada cualquier corrección editorial.
- [ ] Cotejar únicamente esos fragmentos, actualizar su procedencia y volver a
  validar los apuntes que cambien, incluida su presentación en GitHub.
- [ ] Cerrar los bloqueos documentales antes de declarar fidelidad al 100% y
  declarar la materia completa. El usuario autorizó expresamente fusionar los
  avances actuales el24/10/2026, manteniendo estos pendientes documentados.

El detalle por original, páginas, notas y versiones está en
[inventario.json](inventario.json), [cobertura.json](cobertura.json) e
[imposiciones.json](imposiciones.json). Los originales permanecen intactos en
OneDrive; las extracciones e imágenes de trabajo se conservan en caché local.
