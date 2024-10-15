>[!note] Para que sirve?
>La idea de minimizar la funcion de costo, significa minimizar el error. Toma una [[redes neuronales|red neuronal]] y va bajando por la colina de los pesos para minimizar el error entre las predicciones

Es un algoritmo de optimizacion de parametros. Calcula la derivada parcial de la funcion de costo con respecto a cada uno de los parametros del modelo. 
$$ diff/(diff W) M S E(W)  $$
> Recordemos que el ![[MSE]]

El gradiente descendente en cada iteracion cambia los valores de $W$ con el objetivo de minimizar la funcion de costo 

$$W^text("nextstep") = W - eta times diff/(diff W) M S E (W) $$

Donde $eta=$ *tasa de aprendizaje* => El tamaño de los pasos cuesta abajo. 

![[LearningRate.jpg]]
Ocurren casos en los que la funcion de costo tiene 2 minimos. Un minimo local y un minimo global. Para esto se recomienda tener mas de una iteracion con una Iniciacion aleatoria diferente.

![[IrregularCostFunction.jpg]]



