# 🧠 Taller Práctico: Modelos No Supervisados

## Índice de la Sesión

- **Concepto de aprendizaje no supervisado**
- **Tipos de aprendizaje no supervisado**
  - Clustering
  - Detección de anomalías
  - Reducción dimensional
- **Construcción de un modelo no supervisado**
  - Definición del modelo
  - Entrenamiento
  - Persistencia
  - Predicción
- **Algoritmos**
  - K-Means
  - K-Medoids

---

## Objetivos

- Comprender el **aprendizaje no supervisado**, sus principales tipos y aplicaciones.
- Aprender a construir un modelo no supervisado.
- Conocer y aplicar los algoritmos de clustering más utilizados, con especial atención a **K-Means**.

---

## Conceptos Clave

- **Aprendizaje no supervisado**: Técnicas que identifican patrones en datos no etiquetados.
- **Clustering**: Agrupación de datos en grupos de observaciones similares.
- **Detección de anomalías**: Identificación de observaciones que difieren significativamente del resto.
- **Reducción dimensional**: Transformación de datos a un espacio con menos variables, manteniendo la mayor cantidad de información posible.
- **Hiperparámetro**: Parámetro configurable del modelo que no se aprende directamente a partir de los datos.
- **Centroide**: Punto medio (geométrico) de un grupo de datos.
- **Medoide**: Observación representativa dentro de un grupo, con mínima disimilitud respecto al resto.

---

## Sinopsis

El **aprendizaje no supervisado** busca descubrir patrones en conjuntos de datos **sin etiquetas** (sin variable objetivo). Puede ser útil por sí mismo o como paso previo en modelos supervisados.

### Clustering

El **clustering** busca agrupar observaciones para que:

- Las del **mismo grupo** sean lo más similares posible.
- Las de **grupos distintos** sean lo más diferentes posible.

Esto se logra utilizando métricas de distancia (como la euclídea).

---

## Algoritmos de Clustering

### K-Means

K-Means busca dividir los datos en **K grupos**, minimizando la **varianza intra-cluster** (suma de distancias al centroide).  
Pasos del algoritmo:

1. **Inicialización**: Se seleccionan K centroides iniciales (por ejemplo, con el método de Forgy).
2. **Asignación**: Cada muestra se asigna al centroide más cercano.
3. **Actualización**: Se recalculan los centroides de cada grupo.
4. **Convergencia**: El algoritmo termina cuando ya no cambian las asignaciones.

### K-Medoids

Similar a K-Means, pero los **centroides deben ser observaciones reales del dataset** (medoides) y puede usar cualquier métrica de distancia.

Ventajas:

- **Menor sensibilidad a outliers.**
- **Mayor flexibilidad** en métricas de similitud.
- **Mayor interpretabilidad** (los representantes del grupo son datos reales).

**Algoritmo más común:** `PAM` (Partitioning Around Medoids):

1. Selección aleatoria de K medoides.
2. Asignación de cada muestra al medoide más similar.
3. Evaluación de posibles cambios de medoide que reduzcan el coste.
4. Finaliza al no haber mejoras posibles.

---

## Casos Realesss

Durante la sesión se analizarán ejemplos reales de:

- **Clustering**
- **Detección de anomalías**
- **Reducción dimensional**

---

## Ejercicio Práctico

Se aplicarán algoritmos de clustering a la **segmentación de productos** en una empresa de retail.

---

## ¿Qué Hemos Aprendido?

- Fundamentos del aprendizaje no supervisado y sus variantes.
- Algoritmos clave como **K-Means** y **K-Medoids**.

---

## Lecturas Recomendadas

- [Scikit-learn: Documentación sobre aprendizaje no supervisado](https://scikit-learn.org/stable/unsupervised_learning.html)
- Arthur, D. & Vassilvitskii, S. _["k-means++: The advantages of careful seeding"](https://theory.stanford.edu/~sergei/papers/soda06-kmeans.pdf)_, ACM-SIAM Symposium on Discrete Algorithms (2007)
- “Faster k-Medoids Clustering: Improving the PAM, CLARA, and CLARANS Algorithms", in _Similarity Search and Applications_, Springer (2019). [arXiv:1810.05691](https://arxiv.org/abs/1810.05691)