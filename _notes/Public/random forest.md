---
title: Random Forest
feed: show
date: 01-01-2021
---

Es un algoritmo de [[Machine Learning]] que opera construyendo un [[conjunto]] de árboles de decisión durante el entrenamiento. Digamos que un arbol es el que a travez de un conjunto de datos construye un camino hacia el punto que queremos predecir.

Random Forest se enfoca en tomar muchos arboles, de ahi el nombre de **forest(bosque)** y con base a todos esos arboles tener una mejor perspectiva de tus datos.


![[random-forest-image.png|400]]

>[!note]+ Es igual que [[bagging]]?
>Comparten una lógica similar ya que ambos son técnicas de ensamble basadas en árboles y utilizan el método de [[bootstrap]] para generar múltiples conjuntos de datos de entrenamiento. Sin embargo, Random Forest introduce una capa adicional de aleatoriedad: en cada división de un árbol, se selecciona un subconjunto aleatorio de características en lugar de considerar todas las posibles características. Esto hace que Random Forest sea menos propenso a sobreajustar en comparación con Bagging.


