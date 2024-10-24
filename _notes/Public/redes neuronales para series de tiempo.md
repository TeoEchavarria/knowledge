---
title: Redes Neuronales para series de tiempo
feed: show
date: 08-10-2024
---

Para el pronóstico de [[serie de tiempo|series de tiempo]] se debe tener en cuenta que los datos tienen una secuencia que no se debe alterar en el entrenamiento. Por tanto, la división de los datos se hace en el mismo orden temporal: los datos más lejanos se utilizan para el entrenamiento y los más recientes para validación y prueba.

![[DataSetTS.jpeg]]

## Estrategias para entrenar series de tiempo 

- Aplicarle transformaciones a la seried e tiempo - Con el fin de llegar a algo con una estacionalidad mas marcada **BUSCAR - (Diferenciacion y Logaritmica)**
- [[validacion cruzada]] - Lags
- [[escalado de variables]]
- [[Dropout]] - Luego de haber sobre ajustado el modelo, significa que puedo volver a un estado optimo, tengo que penalizar ese sobre entrenamiento
- [[callbacks - early stopping]]
- 