# TheValley
Preparación de clases a impartir en  el MDS+ de The Valley del curso 2020/2021.

# Clase 1 - Análisis Exploratorio
Introducción al análisis exploratorio: 
- cómo importar un dataset en colab
- cómo hacer comprobaciones básicas sobre el mismo
- cómo limpiar el dataset (formatos, nulos)
- cómo realizar transformaciones básicas sobre el dataframe
- cómo extraer la distribución de las variables

Los materiales que utilizaremos son:
- [Presentación](https://docs.google.com/presentation/d/1IT6OVy9YS_sbgHF2oU9D0L--fZiyUfij7NxVhu3cAdg/edit?usp=sharing) | [Presentación formato claro](https://docs.google.com/presentation/d/1H04gE9N6dTgWJ7o9tgxZIHyXMNRD8HB97EKwotOWUng/edit?usp=sharing)
- [Notebook explicación EDA](https://colab.research.google.com/github/JotaBlanco/TheValley/blob/main/Notebooks/01-proceso-analisis-exploratorio/01___Proceso_analisis_exploratorio__sin_resolver_ejercicios.ipynb#scrollTo=cnHRaho3rsXS) | [Notebook explicación EDA con ejercicios resuelto](https://colab.research.google.com/github/JotaBlanco/TheValley/blob/main/Notebooks/01-proceso-analisis-exploratorio/01___Proceso_analisis_exploratorio.ipynb)  
- [Notebook ejercicio 1 EDA](https://colab.research.google.com/github/JotaBlanco/TheValley/blob/main/Notebooks/01-proceso-analisis-exploratorio/EJERCICIO_1__proceso_analisis_exploratorio_sin_resolver.ipynb#scrollTo=exi-HUGCoCae)   |   [Notebook ejercicio 1 EDA Resuelto](https://colab.research.google.com/github/JotaBlanco/TheValley/blob/main/Notebooks/01-proceso-analisis-exploratorio/EJERCICIO_1__proceso_analisis_exploratorio.ipynb)
- [Notebook ejercicio 2 EDA](https://colab.research.google.com/github/JotaBlanco/TheValley/blob/main/Notebooks/01-proceso-analisis-exploratorio/EJERCICIO_2__proceso_analisis_exploratorio_sin_resolver.ipynb)   |   [Notebook ejercicio 2 EDA Resuelto](https://colab.research.google.com/github/JotaBlanco/TheValley/blob/main/Notebooks/01-proceso-analisis-exploratorio/EJERCICIO_2__proceso_analisis_exploratorio.ipynb)



# Clase 2 - Análisis Exploratorio Visual
Recordamos y desarrollamos conceptos básicos sobre el EDA, poniendo el foco en la visualización de los datos.  
- pequeño repaso Python: [paréntesis, corchetes, objetos y más](https://colab.research.google.com/github/JotaBlanco/TheValley/blob/main/Notebooks/00___Peque%C3%B1o_repaso_de_formatos_tipos_par%C3%A9ntesis_corchetes.ipynb)
- pequeño repaso análisis exploratorio:  [ejercicio Titanic](https://colab.research.google.com/github/JotaBlanco/TheValley/blob/main/Notebooks/01-proceso-analisis-exploratorio/EJERCICIO_1__proceso_analisis_exploratorio.ipynb)
- cómo visualizar información siguiendo buenas prácticas
- cómo utilizar matplotlib.pyplot
- cómo emplear las funciones principales de Pyplot: plt.plot(), plt.bar(), plt.scatter(), plt.hist()
- cómo aprovecharnos de la estética de Seaborn
- cómo generar reports automáticos con pandas-profiling

Los materiales que utilizaremos son:
- [Presentación](https://docs.google.com/presentation/d/1N7MPSC7ntM-0ZEHlrN5xRTpT4uNDyU_o53GBvnojUx8/edit) | [Presentación formato claro](https://docs.google.com/presentation/d/1YS2POSE2xxyebvRIvpgQF5JQdAWE4ZkogvI7oKnqNoc/edit?usp=sharing)
- [Notebook explicación EDA visual](https://colab.research.google.com/github/JotaBlanco/TheValley/blob/main/Notebooks/02-analisis-exploratorio-visual/02___Analisis_exploratorio_visual_sin_resolver.ipynb#scrollTo=cnHRaho3rsXS) | [Notebook explicación EDA visual resuelto](https://colab.research.google.com/github/JotaBlanco/TheValley/blob/main/Notebooks/02-analisis-exploratorio-visual/02___Analisis_exploratorio_visual.ipynb)
- EJERCICIO 3 EDA Visual: [Versión Fácil](https://colab.research.google.com/github/JotaBlanco/TheValley/blob/main/Notebooks/02-analisis-exploratorio-visual/EJERCICIO_3___sin_resolver_nivel_FACIL.ipynb) | [Versión Complicada](https://colab.research.google.com/github/JotaBlanco/TheValley/blob/main/Notebooks/02-analisis-exploratorio-visual/EJERCICIO_3___sin_resolver_nivel_DIFICIL.ipynb) | [Versión Resuelta](https://colab.research.google.com/github/JotaBlanco/TheValley/blob/main/Notebooks/02-analisis-exploratorio-visual/EJERCICIO_3___EDA_Visual_Covid.ipynb). 
- EJERCICIO 4 EDA Visual: [Versión Fácil](https://colab.research.google.com/github/JotaBlanco/TheValley/blob/main/Notebooks/02-analisis-exploratorio-visual/EJERCICIO_4___sin_resolver_FACIL.ipynb) | [Versión Complicada](https://colab.research.google.com/github/JotaBlanco/TheValley/blob/main/Notebooks/02-analisis-exploratorio-visual/EJERCICIO_4___sin_resolver_DIFICIL.ipynb) | [Versión Resuelta](https://colab.research.google.com/github/JotaBlanco/TheValley/blob/main/Notebooks/02-analisis-exploratorio-visual/EJERCICIO_4___EDA_Visual_Barsa_Madrid.ipynb). 
- EJERCICIO 5 EDA Visual (Difícil): [Ejercicio sin resolver](https://colab.research.google.com/github/JotaBlanco/TheValley/blob/main/Notebooks/02-analisis-exploratorio-visual/EJERCICIO_5___EDA_Visual_Funcion_Scatter_sin_resolver.ipynb) | [Solución](https://colab.research.google.com/github/JotaBlanco/TheValley/blob/main/Notebooks/02-analisis-exploratorio-visual/EJERCICIO_5___EDA_Visual_Funcion_Scatter.ipynb).

# Clase 3 - Análisis Causal, Univariante y Multivariante
Un análisis EDA profundo suele desembocar en un estudio de las relaciones entre variables. Con esto se intenta comprender los mecanismos que dan lugar a nuestros datos. En esta sesión nos centraremos en:
- cómo hacer un análisis univariante (estudio de una variable)
- cómo hacer un análisis multivariante (estudio de la relación entre dos o más variable)
- por qué es importante una óptica causal
- cuáles son las posibles fuentes de una correlación:
  - azar
  - relación causal
  - presencia de confounder
  - ajuste por collider

Los materiales que utilizaremos son:
- [Presentación](https://docs.google.com/presentation/d/13ITTrYV95OhS3C5wYkUICPNn0etweGA4-PicSZP14Lk/edit?usp=sharing) | [Presentación formato claro](https://docs.google.com/presentation/d/1WNWGnLUyiGqwFf92V3V_szu3QTD_0EQY5GZjhFgen5Q/edit#slide=id.gbb72ec861c_0_558)
- NOTEBOOKS de explicación con ejemplos:
  - 3A - Análisis univariante: [Original](https://colab.research.google.com/github/JotaBlanco/TheValley/blob/main/Notebooks/03-analisis-univariante-causal-multivariante/03_A___Analisis_univariante_sin_resolver.ipynb) | [Resuelto](https://colab.research.google.com/github/JotaBlanco/TheValley/blob/main/Notebooks/03-analisis-univariante-causal-multivariante/03_A___Analisis_univariante.ipynb)
  - 3B - Análisis multivariante: [Original](https://colab.research.google.com/github/JotaBlanco/TheValley/blob/main/Notebooks/03-analisis-univariante-causal-multivariante/03_B___Analisis_multivariante_sin_resolver.ipynb) | [Resuelto](https://colab.research.google.com/github/JotaBlanco/TheValley/blob/main/Notebooks/03-analisis-univariante-causal-multivariante/03_B___Analisis_multivariante.ipynb)
  - 3C - Análisis causal: [Original](https://colab.research.google.com/github/JotaBlanco/TheValley/blob/main/Notebooks/03-analisis-univariante-causal-multivariante/03_C___Introducci%C3%B3n_analisis_causal_sin_resolver.ipynb) | [Resuelto](https://colab.research.google.com/github/JotaBlanco/TheValley/blob/main/Notebooks/03-analisis-univariante-causal-multivariante/03_C___Introducci%C3%B3n_analisis_causal.ipynb)
