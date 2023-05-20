ALGORITMOS DE ORDENAMIENTO
Son procedimientos que nos permiten ordenar información de una manera especial basándonos en un criterio de ordenamiento, el resultado de salida deberá ser un reordenamiento de la entrada.
Un ordenamiento eficiente es importante al usar algoritmos como los de búsqueda/fusión ya que requieren listas ordenadas para una ejecución rápida.

CLASIFICACIÓN - en función de la ubicación de los datos que se están ordenando:

Ordenamientos internos: Son aquellos en los que los valores a ordenar están en memoria principal. Los algoritmos de ordenamiento interno se diseñan teniendo en cuenta la limitación de la memoria principal y buscan maximizar la eficiencia y minimizar el uso de recursos. Estos algoritmos operan directamente en los datos almacenados en la memoria RAM y realizan las comparaciones y manipulaciones necesarias para lograr el ordenamiento deseado.
Algunos ejemplos: Heapsort, Treesort, Quicksort, Mergesort.

Ordenamientos externos: Son aquellos en los que los valores a ordenar son más grandes que los que nuestra memoria puede abarcar y un tipo de memoria más lenta (ej. disco duro) tiene que utilizarse en el proceso. Los algoritmos de ordenamiento externo se diseñan teniendo en cuenta la necesidad de leer y escribir datos en bloques y minimizar las operaciones de E/S (entrada/salida) costosas en términos de tiempo.
Algunos ejemplos: Polyphase sort, Mergesort externo.

¿Cómo se ordenan los datos?

Ordenamiento por comparación: Este tipo de algoritmos ordena los elementos comparándolos entre sí utilizando operaciones de comparación como "mayor que" o "menor que".
Ej. Tree sort: Utiliza árboles binarios para organizar los datos, los valores más pequeños van en el subárbol izquierdo y los más grandes en el derecho.

Ordenamiento no comparativo: Estos algoritmos no se basan en la comparación directa de elementos. En su lugar, utilizan propiedades particulares de los elementos o datos para realizar el ordenamiento.
Ej. Counting Sort: Utiliza un arreglo auxiliar para contar el número de elementos distintos y luego reconstruye la lista ordenada.

COMPLEJIDAD TEMPORAL
La complejidad temporal se refiere al tiempo que tarda en ejecutarse el programa en función del tamaño del conjunto de datos que se está ordenando, ésto es un indicador clave de la eficiencia de un algoritmo.
La complejidad temporal se mide en términos de la notación Big-O, los programas con una notación más baja son más eficientes.

NOTACIÓN BIG-O

O(1) - Complejidad constante: Indica que el algoritmo tiene un tiempo de ejecución constante, independientemente del tamaño de los datos de entrada. Es la notación más eficiente, ya que realiza una cantidad fija de operaciones.

O(log n) - Complejidad logarítmica: Indica que el tiempo de ejecución del algoritmo aumenta de manera logarítmica a medida que crece el tamaño de los datos de entrada. Los algoritmos con esta complejidad suelen dividir el problema en partes más pequeñas en cada iteración, lo que resulta en un crecimiento lento del tiempo de ejecución.

O(n) - Complejidad lineal: Indica que el tiempo de ejecución del algoritmo aumenta de manera proporcional al tamaño de los datos de entrada. Los algoritmos con complejidad lineal realizan una operación por cada elemento en el conjunto de datos.

O(n log n) - Complejidad n logarítmica: Indica que el tiempo de ejecución del algoritmo aumenta en proporción al producto del tamaño de los datos de entrada y el logaritmo del tamaño de los datos. Es común en algoritmos de ordenamiento eficientes como Mergesort y Quicksort.

O(n^2) - Complejidad cuadrática: Indica que el tiempo de ejecución del algoritmo aumenta de manera cuadrática a medida que crece el tamaño de los datos de entrada. Los algoritmos con esta complejidad suelen tener bucles anidados que realizan una operación para cada par de elementos.

O(2^n) - Complejidad exponencial: Indica que el tiempo de ejecución del algoritmo aumenta de manera exponencial a medida que crece el tamaño de los datos de entrada. Los algoritmos con esta complejidad suelen tener una explosión combinatoria y se vuelven rápidamente impracticables para conjuntos de datos grandes.

Hay otras complejidades, como O(n!) factorial y O(n^n) exponencial polinómico, son aún menos eficientes y se vuelven impracticables para conjuntos de datos moderados o grandes.

ALGORITMOS TRABAJADOS EN ÉSTE PROYECTO

BUBBLE SORT - O(n^2)
Es un sencillo algoritmo de ordenamiento que funciona revisando cada elemento de la lista que va a ser ordenada con el siguiente, intercambiándolos de posición si están en el orden equivocado. Es necesario revisar varias veces toda la lista hasta que no se necesiten más intercambios.
También es conocido como el método del intercambio directo. Dado que solo usa comparaciones para operar elementos, se lo considera un algoritmo de comparación, siendo uno de los más sencillos de implementar.

INSERTION SORT - O(n^2)
Es un sencillo algoritmo de ordenamiento que funciona dividiendo la lista (entrada) en dos partes: una parte ordenada y una parte no ordenada. Al principio, la parte ordenada contiene solo el primer elemento de la lista, luego compara el elemento actual con los elementos en la parte ordenada, si el elemento actual es menor que un elemento en la parte ordenada, se desplaza ese elemento hacia la derecha para hacer espacio para el elemento actual.

SELECTION SORT - O(n^2)
Es un algoritmo de ordenamiento que recorre la lista en busca del elemento más pequeño y lo intercambia con el primer elemento. El proceso se repite iterativamente hasta que todos los elementos estén en su lugar final.

QUICK SORT - O(n log n)
Es un algoritmo de ordenamiento eficiente que utiliza el enfoque de "dividir y conquistar". Selecciona un elemento llamado "pivote" de la lista y organiza los demás elementos alrededor del pivote, dividiendo así la lista en dos subconjuntos. Uno de los subconjuntos contiene elementos menores que el pivote, y el otro contiene elementos mayores. Luego, se aplica el mismo proceso de forma recursiva a los subconjuntos, dividiéndolos aún más y ordenándolos.
