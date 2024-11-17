---
title: Cross-Entropy
feed: show
date: 16-11-2024
tags:
  - ai
  - ml
  - estadistica
curso:
---
Es una medida de la diferencia entre dos distribuciones de probabilidad: la verdadera distribución de los datos y la distribución predicha por un [[modelo]]. 

Se utiliza comúnmente en problemas de [[clasificacion]], como en [[redes neuronales]], para evaluar qué tan bien un modelo predice las etiquetas de las clases.

$$H(p,q) = - sum_i p(i) dot log q(i) $$
- $p(i)$ es la probabilidad verdadera (la distribución real de las etiquetas).
- $q(i)$ es la probabilidad predicha por el modelo.