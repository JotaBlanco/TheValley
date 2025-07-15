# 🧠 Taller Práctico: Modelos No Supervisados

## Índice de la Sesión

- **Concepto de aprendizaje no supervisado**
- **Construcción de un modelo no supervisado**
  - Definición del modelo
  - Entrenamiento
  - Persistencia
  - Predicción
- **Intuición de la clusterización y las distancias**
  - Distribución de variables en los distintos clusters
  - Cálculos de distancias

---

## Objetivos

- Comprender el **aprendizaje no supervisado**, sus principales tipos y aplicaciones.
- Aprender a construir un modelo no supervisado **K-Means**.
- Desarrollar una intuición sólida sobre el concepto de clústers y distancias.

---


## Sinopsis

El **aprendizaje no supervisado** busca descubrir patrones en conjuntos de datos **sin etiquetas** (sin variable objetivo). Puede ser útil por sí mismo o como paso previo en modelos supervisados.

### Clustering

El **clustering** busca agrupar observaciones para que:

- Las del **mismo grupo** sean lo más similares posible.
- Las de **grupos distintos** sean lo más diferentes posible.

Esto se logra utilizando métricas de distancia (como la euclídea).

---
## K-Means

K-Means busca dividir los datos en **K grupos**, minimizando la **varianza intra-cluster** (suma de distancias al centroide).  
Pasos del algoritmo:

1. **Inicialización**: Se seleccionan K centroides iniciales (por ejemplo, con el método de Forgy).
2. **Asignación**: Cada muestra se asigna al centroide más cercano.
3. **Actualización**: Se recalculan los centroides de cada grupo.
4. **Convergencia**: El algoritmo termina cuando ya no cambian las asignaciones.

