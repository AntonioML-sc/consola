
#### PROYECTO: IMAGEN FRONTAL CONTROLADOR DE VIDEOCONSOLA

#### Definición y alcance:

El objeto de este proyecto con fines de aprendizaje, que será el primero que realizo en HTML, es la reproducción aproximada de la imagen frontal de una videoconsola portátil o bien un controlador de videoconsola en un archivo HTML usando una hoja de estilos en cascada en CSS para modelar el aspecto de cada elemento. Para este efecto, se ha elegido el controlador xbox series X en su versión para pc.

#### Objetivos:

1- Familiarizarse con la estructura de un proyecto dividido en múltiples <div> con una estructura jerárquica.
2- Testear el uso de diversas formas de colocar los <div>, en especial el uso de flexbox, pero también el uso de márgenes y otros medios para posicionar o superponer unas secciones sobre otras.
3- Emplear las formas básicas para definir las dimensiones y estilos de las divisiones usadas.
4- Usar algunos elementos que reaccionen al usuario, en este caso al pasar el cursor sobre los elementos, hasta donde el uso de CSS permita.

#### Notas de desarrollo:

Este desarrollo abarcó 2 días y medio de trabajo y aprendizaje por experimentación.

El mejor criterio posible habitualmente consiste en diseñar en unidades relativas, preferiblemente em o como mal menor en px, para ayudar a conseguir un diseño responsive. Sin embargo, se decidió en este caso diseñar en mm con el fin de dar a la caja las dimensiones del dispositivo real, si bien no se pudo disponer de todas las medidas reales, menos aún reproducirlas. Esta decisión hizo más problemático el diseño si cabe y finalmente me conformé con una simple imitación, que para los objetivos del proyecto es aceptable.

El uso de la herramienta clip-path, empleado para conseguir formas complejas a partir de arcos, elipses, líneas y curvas polinómicas de grados 2 y 3 (curvas de Bézier) generó algunos problemas, como la necesidad de diseñar con medidas relativas y ciertas dificultades para la colocación de los elementos que las usaron, que hicieron más práctico el colocarlos con el ajuste de "position: absolute". Este método se usó también para superponer elementos que difícilmente habrían encajado en una distribución con flexbox. Las coordenadas usadas para las trayectorias svg del clip-path se escribieron directamente en el archivo index.html por tanteo, sin asistencia de ningún programa de CAD que las creara (nunca más!), lo cual ha hecho que la continuidad entre las diversas curvas no sea tipo C1 como habría sido deseable.

VERSIÓN ACTUAL: https://antonioml-sc.github.io/consola/

#### Bugs conocidos y posibles nuevos trabajos:

- Existe un bug que hace que el cable pierda la posición correcata en el eje X al hacer zoom por encima de las dimensiones del conjunto.

- Se plantea incorporar un archivo en JavaScript para dotar de movimientos a elementos que aún no los tienen, como los sticks. Hacer lo propio con los gatillos requerirá un refactor que separe a éstos entre sí y de la inserción del cable en 3 elementos.

- Pendiente de revisar el archivo styles.css para añadir comentarios que ayuden a la navegación y eliminar líneas innecesarias.

- Será bienvenido cualquier comentario o sugerencia.
