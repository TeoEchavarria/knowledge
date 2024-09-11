#ml #ai
# Ada Boost 

Es un [[algoritmo]] de [[Machine Learning]] de ensamble que combina múltiples clasificadores débiles para crear un clasificador fuerte. 

Los clasificadores débiles se añaden secuencialmente, enfocándose en los ejemplos más difíciles de clasificar correctamente en las rondas anteriores. 

En si en cada ronda crea un modelo nuevo que posteriormente se va a combinar con los demas pequeños modelos. 

>[!failure]+ [[overfitting]]
>Entre más clasificadores débiles utilices en AdaBoost, mayor es el riesgo de overfitting, especialmente si los datos contienen ruido o [[outliers]]. Por esta razón, una limpieza y preparación cuidadosa de los datos antes de aplicar AdaBoost (o cualquier otro algoritmo de machine learning) puede mejorar significativamente el rendimiento del modelo y reducir el riesgo de overfitting.

>[!note]+ Es igual que [[gradient_boosting]]?
>  Imagina que los [[modelo|modelos]] son dos chefs mejorando una receta. AdaBoost prueba la sopa, encuentra que está muy salada, y en la siguiente tanda reduce la sal en los platos mal calificados. Repite, ajustando cada vez más hasta que la mayoría estén bien.
>  
>Gradient Boosting también prueba la sopa, pero en lugar de ajustar la sal directamente, averigua qué ingredientes adicionales pueden contrarrestar la salinidad excesiva y los agrega poco a poco, refinando la receta en cada iteración.

