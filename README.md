# Exercicios resueltos módulo de Modelos de Intelixencia Artificial.

## Resolución de problemas mediante búsquedas.

---

## Ejercicio 1

Considérese el problema de encontrar un camino, en la situación representada en la figura, desde la posición $i$ hasta la posición $e$. El NPC (*non-player character*) puede moverse de forma horizontal y vertical, un solo cuadrado en cada movimiento (cada movimiento tiene coste uno). Las zonas sombreadas impiden el paso del NPC a través de ellas.

### Algoritmos aplicados respectivamente:

Aplicaremos los distintos algoritmos de búsqueda que se tratan en las sesiones del módulo para resolver el problema, en el siguiente orden:

1. Búsqueda en anchura.
2. Búsqueda en profundidad.
3. Búsqueda de coste uniforme.
4. Algoritmos **A** y **A***.

### Preguntas específicas:

1. En la búsqueda en profundidad, el límite de profundidad es 5:
   - Describe qué sucede.
   - Indica el tipo de fracaso (si lo hay).
   - ¿Qué sucede si aumentamos el límite de profundidad a 6?

### Respuestas:

   - Lo que ocurre al aplicarle el límite de profundidad 5 es que el algoritmo acaba pasándose del propio límite y no es posible llegar a los nodos objetivos hasta la profundidad 6 (7 incluyendo cuando llega al nodo objetivo).
   - En este caso y como es mencionado anteriormente, existe un fracaso del valor de corte dado que la solución del problema se haya dentro del límite de profundidad.
   - Que en este caso si llegaríamos a hallar la solución.

---

## Ejercicio 2

### Preguntas específicas:

1. La heurística utilizada en el algoritmo **A** previamente, ¿es admisible? ¿Por qué?
   - ¿Podemos decir que el algoritmo es **A***?

### Respuesta:
  - Sí, la heurística es admisible porque nunca sobreestima el costo real al objetivo. Esto significa que el algoritmo garantiza una solución óptima. Como el algoritmo utiliza la función f(n)=g(n)+h(n)f(n)=g(n)+h(n), podemos decir que es A*.
  
---

## Ejercicio 3

En el hipotético caso de que el servicio Google Maps empleara el algoritmo de **búsqueda por coste uniforme** para encontrar la ruta más corta (en km) entre dos localidades, calcula la solución que ofrecería para la ruta **Ourense-Calatayud** dadas las siguientes distancias kilométricas:

| Trayecto            | Distancia en km      |
| :------------------ | :------------------:|
| Ourense, Ponferrada | 175                 |
| Ourense, Benavente  | 236                 |
| Ponferrada, León    | 113                 |
| Ponferrada, Benavente | 125               |
| Benavente, León     | 75                  |
| Benavente, Valladolid | 112               |
| Benavente, Palencia | 112                 |
| Palencia, León      | 131                 |
| Palencia, Valladolid | 48                 |
| Palencia, Osorno    | 49                  |
| Palencia, Burgos    | 92                  |
| León, Osorno        | 121                 |
| Osorno, Burgos      | 59                  |
| Valladolid, Aranda  | 95                  |
| Burgos, Aranda      | 84                  |
| Aranda, Osma        | 58                  |
| Osma, Calatayud     | 140                 |
| Osma, Soria         | 58                  |
| Burgos, Soria       | 143                 |
| Burgos, Logroño     | 150                 |
| Logroño, Soria      | 106                 |
| Soria, Calatayud    | 91                  |

### Ejercicio resuelto en el .pdf.
