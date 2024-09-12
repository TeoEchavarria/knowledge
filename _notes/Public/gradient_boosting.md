---
title: Gradient Boosting
feed: show
date: 01-01-2021
---

Es un método de [[Machine Learning]] de ensamble que crea un [[modelo]] fuerte a partir de una serie de modelos débiles, típicamente árboles de decisión. 

A diferencia de [[ada boost]], que ajusta los pesos de las instancias.

Gradient Boosting mejora los modelos débiles minimizando una función de pérdida, que es una medida de cuán mal el modelo está haciendo predicciones. Se añaden sucesivamente nuevos modelos que se enfocan y mejoran los errores del modelo combinado anterior.

>[!note]+ Es igual que [[ada boost]]?
>  Imagina que los modelos son dos chefs mejorando una receta. AdaBoost prueba la sopa, encuentra que está muy salada, y en la siguiente tanda reduce la sal en los platos mal calificados. Repite, ajustando cada vez más hasta que la mayoría estén bien.
>  
>Gradient Boosting también prueba la sopa, pero en lugar de ajustar la sal directamente, averigua qué ingredientes adicionales pueden contrarrestar la salinidad excesiva y los agrega poco a poco, refinando la receta en cada iteración.

