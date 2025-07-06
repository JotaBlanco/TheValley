ÍNDICE DE LA SESIÓN
● Concepto de aprendizaje no supervisado
● Tipos de aprendizaje no supervisado
○ Clustering
○ Detección de anomalías
○ Reducción dimensional
● Construcción de un modelo no supervisado
○ Definición del modelo
○ Entrenamiento
○ Persistencia
○ Predicción
● Algoritmos
○ K-Means
○ K-Medoids


● OBJETIVOS DE LA SESIÓN
El objetivo de la sesión es familiarizarse con el concepto de aprendizaje no supervisado, sus
tipos y cómo se construye un modelo de este tipo. Además se estudiarán los algoritmos de
clustering más utilizados, en particular K-Means.


● CONCEPTOS CLAVE
Aprendizaje no supervisado: Conjunto de algoritmos que tienen como objetivo aprender
patrones de datos no etiquetados.
Clustering: Subconjunto de algoritmos de aprendizaje no supervisado que tratan de agrupar
los datos de manera que datos en el mismo grupo sean similares y datos en grupos distintos
sean diferentes.
Detección de anomalías: Subconjunto de algoritmos de aprendizaje no supervisado que
tratan de determinar aquellos datos que difieren sustancialmente del resto en un mismo
dataset.
Reducción dimensional: Técnicas para disminuir el número de variables que caracterizan
una observación reteniendo una parte sustancial de la información presente en la
representación original.
Hiper parámetro: Parámetro que gobierna el comportamiento de un algoritmo que no es
aprendido directamente de los datos en el entrenamiento.
Centroide: Centro geométrico de las observaciones de un grupo. Punto medio de las
observaciones.
Medoid: Observación dentro de un grupo cuya disimilitud al resto de las observaciones de
ese grupo es mínima.



● SINOPSIS

Los algoritmos de aprendizaje no supervisado tienen como objetivo aprender patrones de la
estructura de los datos.
A diferencia del aprendizaje supervisado en el aprendizaje no supervisado los datos no
están etiquetados, es decir, no tenemos una variable objetivo que queramos predecir.
Los algoritmos de aprendizaje no supervisado pueden aportar un valor en sí mismo o
utilizarse como un paso previo para el entrenamiento de un modelo supervisado.
El análisis cluster o simplemente clustering tiene como objetivo agrupar observaciones de
manera que:
● Dentro de un mismo grupo las observaciones sean lo más similares posible.
● Las observaciones que se encuentran en grupos distintos son lo más distintas entre
ellas.
Para evaluar la similitud entre dos muestras utilizamos alguna métrica de distancia entre las
variables que las caracterizan
El objetivo de un algoritmo de detección de anomalías (también denominadas outliers) es
la detección de muestras que se desvían significativamente del resto de los datos.
Las técnicas de reducción dimensional tratan de transformar los datos desde un espacio
de alta dimensionalidad (datos con muchas columnas) a un espacio de dimensionalidad
menor, reteniendo una parte significativa de la información contenida en ellos.
El algoritmo K-Means es uno de los más utilizado en el análisis de clusters. Su objetivo es,
dado un número K de clusters, agrupar los datos en K grupos de manera que se minimice la
varianza intra-cluster.
La varianza intra-cluster es la suma de la distancia euclídea al cuadrado desde cada
muestra al centroide del cluster, siendo el centroide de un clúster el centro geométrico del
mismo, o lo que es lo mismo el punto medio.
K-Means construye los clusters de la siguiente manera:
● Inicialización de los centroides
Se crean k centroides. Una de las maneras más habituales (Método de Forgy) es tomar k
muestras existentes y elegirlas como centros.
Tras la inicialización se realizan dos pasos iterativamente:
● Paso de asignación
Cada muestra del dataset la asignamos al clúster representado por el centroide más
cercano a la misma.
● Paso de actualización
Re-calculamos las coordenadas de los centroides con las nuevas muestras de cada clúster.
El algoritmo termina cuando se alcanza la convergencia, es decir, cuando en el paso de
asignación ninguna muestra cambia de clúster.
El método de k-medoids es similar a k-means, sin embargo los centroides tienen que
coincidir con una muestra real del dataset, pasándose a llamar medoides o medoids.
Además la distancia no está restringida a ser la distancia euclídea.
Esto permite una serie de ventajas:
● Es menos sensitivo a outliers. El algoritmo de k-means, es muy sensible a valores
anómalos en el dataset pudiendo cambiar significativamente la configuración de los
clusters.
● Permite utilizar métricas arbitrarias para definir la similitud entre clusters, mientras
que k-means generalmente está limitado a la distancia euclídea para soluciones
eficientes.
● En principio, permite mayor interpretabilidad al tener una muestra representativa real
en cada uno de los clusters.
El algoritmo más utilizado es PAM (Partitioning around medoids) y es como sigue:
● Inicializamos los medoides seleccionando k muestras aleatoriamente.
● Asignamos cada muestra al cluster del medoid más similar según la métrica elegida.
● Para cada uno de los medoides cogemos el resto de muestras "no medoide" y
calculamos la función de coste a minimizar si esta fuera medoide y la otra no.
Cambiamos el medoide por la muestra "no medoide" que minimice la función de
coste.
● El algoritmo termina cuando ningún posible cambio de medoide a "no medoide"
reduce el coste.


● CASOS REALES ANALIZADOS EN LA SESIÓN:

En la sesión se van a analizar casos de uso reales de cada una de las técnicas de
aprendizaje no supervisado.
● EJERCICIOS PRÁCTICOS DURANTE LA SESIÓN:
En la sesión se hará un ejemplo de aplicación de algoritmos de clustering a la
segmentación de productos en una compañía de retail.
● ¿QUÉ HEMOS APRENDIDO EN CLASE?
Concepto de aprendizaje no supervisado y sus distintas ramas. Algoritmos
básicos de clustering. K-Means y K-Medoids.
● LECTURAS RECOMENDADAS
- Scikit-learn documentation on unsupervised learning
- “k-means++: The advantages of careful seeding” Arthur, David, and Sergei
Vassilvitskii, Proceedings of the eighteenth annual ACM-SIAM symposium on
Discrete algorithms, Society for Industrial and Applied Mathematics (2007)
- “Faster k-Medoids Clustering: Improving the PAM, CLARA, and CLARANS
Algorithms", Similarity Search and Applications, Springer International Publishing,
11807, pp. 171–187, arXiv:1810.05691