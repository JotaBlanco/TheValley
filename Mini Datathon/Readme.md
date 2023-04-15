# Contenido
En este módulo del máster habéis profundizado en los modelos de deep learning, así como aprendido sobre técnicas para diseñar soluciones de IA escalables y el despliegue de modelos en la nube. Hoy vamos a aprender una nueva filosofía de tratamiento de datos (streaming), que emplearemos para desplegar varios modelos de deep learning ya entrenados (disponibles en Huggingface) en la nube para acabar la clase con un chat con análisis de sentimiento en producción... y más!

### 01 - Introducción a streaming
El streaming es la filosofía perfecta para trabajar con datos en tiempo real. Veremos de qué va el streaming cubriendo:
- Streaming VS Batch
- PUB/SUB
- Kafka Topic

### 02 - Streaming con quix streams
Veremos cómo hacer streaming con la librería de Python [quix-streams](https://github.com/quixio/quix-streams):
- pub() - [Notebook pub()](https://colab.research.google.com/github/JotaBlanco/TheValley/blob/main/Mini%20Datathon/Notebooks/Quix_Streams_PUB.ipynb)
- sub() - [Notebook sub()](https://colab.research.google.com/github/JotaBlanco/TheValley/blob/main/Mini%20Datathon/Notebooks/Quix_Streams_SUB.ipynb)
- procesar datos

### 03 - Puesta en producción en la nube con Quix
Usaremos la plataforma de Quix para desplegar nuestro código. La plataforma de Quix está pensada para trabajar con datos en streaming, por lo que nos vendrá bien para desplegar nuestro código y modelos en este caso.
- overview de la plataforma
- ejemplo de detección de agitar el móvil

### 04 - Huggingface
[Huggingface](https://huggingface.co/) es una iniciativa open source donde podemos encontrar gran cantidad de modelos y bases de datos estado del arte en deep learning. Hoy usaremos esos modelos ya entrenados.
- investigando Huggingface (overview en la página web)
- probando algunos modelos (Notebook)

### 05 - Chat avanzado
Manos a la obra! Aquí construiréis una aplicación chat dónde cualquiera pueda participar con su QR, pero analizando el sentimiento de los mensajes en tiempo real y censurando los ofensivos!
- Construír topics de kafka necesarios
- Construir applicación chat
- Añadir análisis de sentimiento


# Materiales
- Notebook 1
- Notebook 2
- Notebook 3
- 
