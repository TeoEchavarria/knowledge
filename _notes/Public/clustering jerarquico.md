---
title: Clustering Jerárquico
feed: show
date: 15-03-2025
tags: 
curso:
---
El [[clustering]] jerárquico es un enfoque que crea una estructura en forma de árbol (o dendrograma) que representa cómo se agrupan los datos a diferentes niveles de [[granularidad]]. Existen dos variantes principales:

- **Aglomerativo (bottom-up):**  
    Cada muestra inicia como su propio cluster. Luego, en cada iteración, se fusionan los dos clusters más cercanos según alguna medida de distancia (por ejemplo, la distancia Euclidiana o la similitud coseno). Este proceso se repite hasta que todos los puntos se unen en un único cluster o hasta que se detiene según algún criterio (por ejemplo, un umbral de distancia).
- **Divisivo (top-down):**  
    Se parte de un único cluster que contiene todos los puntos y, de forma iterativa, se van dividiendo en subclusters.

El dendrograma resultante te permite visualizar la relación entre clusters y decidir dónde "cortar" el árbol para obtener una partición que tenga sentido para tu aplicación.