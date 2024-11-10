---
title: Overfitting
feed: show
date: 2024-11-10
tags: []
curso: 
---

Es un problema en el que un modelo de machine learning aprende demasiado bien los detalles y el ruido de los datos de entrenamiento, hasta el punto de que pierde la capacidad de generalizar correctamente a datos nuevos.

![[overfitting.png]]

>[!note] [[underfitting]]

### **Para prevenir el overfitting:**

1. **Aumentar el volumen de datos de entrenamiento**: Proporcionar más datos al modelo ayuda a que aprenda patrones generales en lugar de detalles específicos o ruido del conjunto de entrenamiento.

2. **Regularización**: Incorporar términos de penalización en la función de pérdida, como L1 (Lasso) o L2 (Ridge), para limitar la complejidad del modelo y evitar que se ajuste demasiado a los datos de entrenamiento.
3. **Técnicas de [[dropout]]**: Durante el entrenamiento de redes neuronales, desactivar aleatoriamente ciertas neuronas en cada iteración para prevenir que el modelo dependa excesivamente de rutas específicas y mejore su capacidad de generalización.
4. **[[callbacks - early stopping]](detención temprana)**: Monitorear el rendimiento del modelo en un conjunto de validación y detener el entrenamiento cuando el rendimiento comienza a deteriorarse, evitando así que el modelo se ajuste demasiado a los datos de entrenamiento.
5. **Simplificar el modelo**: Reducir la complejidad del modelo disminuyendo el número de parámetros o seleccionando una arquitectura más sencilla para evitar que capture ruido en los datos.