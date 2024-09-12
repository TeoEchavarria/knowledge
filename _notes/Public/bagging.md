---
title: Bagging
feed: show
date: 01-01-2021
---

Es una técnica de ensamble en [[machine learning]] donde múltiples [[modelos|modelo]] (generalmente del mismo tipo) se entrenan en subconjuntos de datos ligeramente diferentes. 

Imagina un grupo de estudiantes *(los modelos)* que estudian para un examen *(el problema de predicción)*. Cada estudiante practica con una selección aleatoria de preguntas *(subconjuntos de datos)* con algunas repeticiones. 

Al final, para responder a una nueva pregunta *(hacer una predicción)*, todos los estudiantes dan su opinión y la respuesta más común *(voto mayoritario)* se selecciona como la respuesta final.

>[!note]+ Es igual que [[random forest]]?
>Comparten una lógica similar ya que ambos son técnicas de ensamble basadas en árboles y utilizan el método de [bootstrap](app://obsidian.md/bootstrap) para generar múltiples conjuntos de datos de entrenamiento. Sin embargo, Random Forest introduce una capa adicional de aleatoriedad: en cada división de un árbol, se selecciona un subconjunto aleatorio de características en lugar de considerar todas las posibles características. Esto hace que Random Forest sea menos propenso a sobreajustar en comparación con Bagging.

>[!note]+ Es igual que [[bagging]]?
>Aunque Voting y Bagging involucran múltiples modelos, Voting combina diferentes tipos de modelos y Bagging usa múltiples versiones del mismo tipo de [[modelo]].

