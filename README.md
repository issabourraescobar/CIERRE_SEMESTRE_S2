# CIERRE_SEMESTRE_S2

**Ejercicio Cierre de Semestre Big Data Sección 2**


Desarrollo.

**EJERCICIO 1.**

"Construya un script en R, que cuente la cantidad de elementos "positivo", "negativo" y "neutros"."

Antes de contar la cantidad de elementos es necesario crear las 100 variables aleatorias con el comando: "ejemplos = sample(c("positivo","negativo","neutro"),100, replace = TRUE)"

Teniendo las 100 V.A es posible contar los elementos con el comando: "table(ejemplos)"

Los resultados obtenidos son: 

**positivo:37, negativo:32, neutro:31.**


**EJERCICIO 2.**

"Experimente ejecutando el set.seed(10), previo a la creación de elementos aleatorios, sin ejecutarlo antes y comente, cómo impactó la implementación del set.seed(10) en los resultados."

Al ejecutar el comando "set.seed(10), este solo fija una cantidad especifica de valores del siguiente comando "ejemplos = sample(c("positivo", "negativo", "neutros"), 10, replace = TRUE)".

Elementos fijados:

**negativo:2, neutro:7, positivo:1**

Si se ejecuta el comando "ejemplos = sample(c("positivo", "negativo", "neutros"), 10, replace = TRUE)" sin fijar se obtienen elementos aleatorios.

Por ejemplo:

**negativo:5, neutro:4, positivo:1**


**EJERCICIO 3.**

"Asuma que los valores "positivo", "negativo" y "neutros" generados a partir de
set.seed(66), corresponde a los resultados recolectados de todas las noticias que hablan
sobre una crisis económica, ¿qué impacto tendría si se consideran o no los neutros?"

Al realizar nuevamente los pasos anteriores pero esta vez con 66 elementos a partir de la recoleccion de una noticia sobre la crisis económica

El comando a utilizar es el siguiente: "ejemplos = sample(c("positivo", "negativo", "neutros"), 66, replace = TRUE)"

Sin utilizar "set.seed(66)":

**negativo:25, neutros:21, positivo:20**

Con "set.seed(66)":

**negativo:20, neutros:20, positivo:26**

Para concluir, que sin utilizar el comando "set.seed(66)" el numero de neutros corresponden al 31,81%, 
si se utiliza el comando "set.seed(66) los elementos neutros sería el 30,3%, existiendo una diferencia de 1,51%.
Por lo que la omisión de este comando influenciaría las noticias negativas sobre las positivas, en caso contrario, las noticias
positivas sobrepasaría el numero en 6 noticias.


4.- "Construya un script capaz de calcular la probabilidad del conjunto de cartas que está por salir,
para crear datos de prueba utilizando la función sample considerando que han salido 31
cartas"

Se asume que el mazo contiene 52 cartas, y ya se han descartado 31 de ellas, queda un total de 21 cartas, se utiliza el comando sample
agrupando las cartas en altas, bajas y medianas. Con las siguientes probabilidades:

**altas: 7(33,33%), bajas: 4(19,05%), medianas: 10(47,62%)**
Obteniendo un total de: -3 puntos finales.


5.- "Si en el ejercicio anterior utilizamos la función set.seed. ¿Qué grupo de cartas tiene más
probabilidades de salir?"

Las probabilidades de salir cada grupo de cartas al aplicar el comando set.seed(21) son:

**altas: 4(19,05%), bajas: 10(47,62%), medianas: 7(33,33%).**

Por lo que el grupo de cartas que tiene mas probabilidades de salir son las bajas con un 47,62%.
