## Recycler view

El widget **RecyclerView** es una versión más flexible y avanzada de **ListView**. Este widget es un contenedor para mostrar grandes conjuntos de datos que se pueden desplazar de manera muy eficiente al mantener una cantidad limitada de vistas. Usa el widget RecyclerView cuando tengas conjuntos de datos cuyos elementos cambien en tiempo de ejecución sobre la base de la acción del usuario o los eventos de la red.

La clase RecyclerView simplifica la pantalla y la manipulación de grandes conjuntos de datos al proporcionar lo siguiente:

+ Administradores de diseño para el posicionamiento de elementos
+ Animaciones predeterminadas para las operaciones comunes con elementos, como quitar o agregar elementos.
También tienes la flexibilidad para definir administradores de diseño personalizados y animaciones para los widgets RecyclerView.

Para usar el widget **RecyclerView**, tienes que especificar un adaptador y un administrador de diseño. Para crear un adaptador, extiende la clase **RecyclerView.Adapter**. Los detalles de la implementación dependen de las especificaciones de tu conjunto de datos y los tipos de vistas.

Un administrador de diseño posiciona las vistas de artículos dentro de un **RecyclerView** y determina cuándo volver a usar las vistas de elementos que ya no están visibles para el usuario. Para reutilizar una vista, un administrador de diseño puede solicitarle al adaptador que reemplace el contenido de la vista con un elemento diferente del conjunto de datos. De esta manera, cuando se reciclan las vistas se mejora el rendimiento al evitar la creación de vistas innecesarias o realizar búsquedas costosas de findViewById().

RecyclerView te proporciona estos administradores de diseño incorporados:

+ LinearLayoutManager muestra elementos en una lista de desplazamiento horizontal o vertical.
+ GridLayoutManager muestra elementos en una cuadrícula.
+ StaggeredGridLayoutManager muestra elementos en una cuadrícula escalonada.