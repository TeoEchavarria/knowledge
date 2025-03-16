---
title: Valor Esperado Condicional
feed: show
date: 01-01-2021
---
Imaginemos que tenemos dos [[variable aleatoria|variables aleatorias]], $X$ y $Y$, que están relacionadas de alguna manera. El valor esperado condicional de $X$ dado $Y=y$, denotado como $E[X|Y=y]$, nos dice cuál es el promedio que esperamos obtener para $X$, si ya sabemos que $Y$ toma el valor $y$.

>[!example] 
>Supongamos que X representa la altura de una persona y Y representa su género (0 para mujer, 1 para hombre). El valor esperado condicional $E[X|Y=0]$ nos dirá cuál es la altura promedio de las mujeres en nuestra población."]

## Propiedades

- **Linealidad**: El valor esperado condicional es una operación lineal. Es decir, $$E[a X+ b Y | Z ] = a E[X|Z] + b E[Y|Z]$$ , donde $a$ y $b$ son constantes.
- **Ley de las expectativas totales**: Esta ley relaciona el valor esperado incondicional con los valores esperados condicionales. Para una [[variable aleatoria discreta]] $Z$, tenemos: $$E[X] = sum E[X|Z=z] dot P(Z=z)$$ 

Para una [[variable aleatoria continua]] $$Z: E[X] = integral E[X|Z=z] dot f_Z(z) d z$$
- **[[varianza]] [[probabilidad condicional|condicional]]: Podemos definir la varianza condicional de $X$ dado $Y=y$ de manera similar a la varianza incondicional, pero utilizando la distribución condicional de $X$ dado $Y=y$.
