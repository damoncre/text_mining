# Text Mining en Social Media
Este es el trabajo de la asignatura Text Mining en Social Media.

## Contenido del respositorio

Este es el contenido que hay en el repositorio:

* text_mining.pptx: Presentación utilizada en clase durante el "Pechakucha".
* pan-ap17_gender.r: Script con la implementación del caso de profiling por género.
* pan-ap17_variety.r: Script con la implementación del caso de profiling por variedad del lenguaje.
* paper.pdf: Artículo escrito sobre el caso de estudio planteado en la asignatura.


## Guía de ejecución
Previamente hay que instalar y cargar las librerías: qdap, XML, tm, splitstackshape y caret , junto con las necesarias de los algoritmos para poder ejecutar los scripts. Adicionalmente se debe cambiar el contenido de las variables path_training y path_test por la ruta donde estén ubicadas los ficheros de training y test respectivamente.

Para ejecutar el script pan-ap17_variety.r se pueden descomentar y comentar la variable swlist si se desea añadir o no stopwords. Adicionalmente se puede comentar la línea train_control que incluya method="none" y dejar la otra sin comentar si se desea utilizar cross validation. 

Cabe mencionar que en el script pan-ap17_gender.r se incluyen muchos más modelos, de modo que se pueden comentar y descomentar a placer la generación y entrenamiento de los distintos modelos de cara a no tener que esperar durante un largo tiempo si solo se quiere ejecutar un determinado algoritmo. Aunque este fichero tenga puesto como nombre gender, se puede cambiar en las variables bow_training y bow_test la clase a variety para probar todos los modelos para variedad del lenguaje.
