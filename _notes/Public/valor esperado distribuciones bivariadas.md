#distribuciones #probabilidad
# Valor Esperado de [[distribuciones bivariadas]]

Imagina que tienes una función g(X, Y) que combina los valores de X e Y de alguna manera. El valor esperado de esta función, $E[g(X, Y)]$, nos dice, en promedio, qué valor podemos esperar obtener al aplicar esta función a los pares de valores (x, y) que siguen la distribución conjunta de X e Y.

## Caso [[variable aleatoria discreta|Discreto]]

$$E[g(X, Y)] = sum sum g(x, y) dot p(x, y)$$

#### Explicación:

- $g(x, y)$: El valor de la función para cada par de valores $(x, y)$.
- $p(x, y)$: La probabilidad de que $X$ tome el valor $x$ y $Y$ tome el valor y simultáneamente.

## Caso [[variable aleatoria continua|Continuo]]

$$E[g(X, Y)] = integral integral g(x, y) dot f(x, y) d x d y$$

#### Explicación:

- $g(x, y)$: El valor de la función para cada par de valores $(x, y)$.
- $f(x, y)$: La densidad de probabilidad en el punto $(x, y)$.
