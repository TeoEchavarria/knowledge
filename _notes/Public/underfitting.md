---
title: Unferfitting
feed: show
date: 2024-11-10
tags: []
curso: 
---
Es el problema opuesto al [[overfitting]]. Ocurre cuando un modelo de machine learning es demasiado simple para capturar la estructura o los patrones presentes en los datos. Como resultado, el modelo no se ajusta bien ni a los datos de entrenamiento ni a los datos nuevos, lo que conduce a un rendimiento deficiente en ambos casos.

![[overfitting.png]]

### Para prevenir el underfitting:

1. **Aumentar la complejidad del modelo**: Utilizar modelos más sofisticados o agregar más parámetros para que el modelo pueda capturar patrones más complejos presentes en los datos.  
2. **Seleccionar características relevantes**: Incluir variables que aporten información significativa y eliminar aquellas que no contribuyan al modelo, mejorando así su capacidad para aprender relaciones importantes.
3. **Entrenar por más tiempo**: Asegurarse de que el modelo tenga suficiente tiempo de entrenamiento para aprender adecuadamente los patrones en los datos, evitando detener el proceso prematuramente.
4. **Ajustar hiperparámetros**: Modificar parámetros como la tasa de aprendizaje, el número de capas o neuronas en una red neuronal, entre otros, para mejorar el rendimiento del modelo y evitar un ajuste insuficiente.