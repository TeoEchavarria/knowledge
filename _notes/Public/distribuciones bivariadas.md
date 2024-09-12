---
title: "Distribucion : Bivariadas"
feed: show
date: 01-01-2021
---

Son distribuciones de probabilidad que describen el comportamiento conjunto de dos [[variable aleatoria|variables aleatorias]]. Estas distribuciones ayudan a entender cómo las dos variables están relacionadas y cómo varían juntas.

## Distribuciones Bivariadas [[variable aleatoria discreta|Discreta]]

Se usan cuando ambas variables aleatorias pueden tomar valores específicos (discretos). La distribución conjunta se representa mediante una [[funcion masa de probabilidad]] de probabilidad conjunta $p(x,y)$ que da la probabilidad de que las variables $X$ y $Y$ tomen valores específicos simultáneamente.

$$p(x, y) = P(X = x, Y = y)$$
$$P((X, Y) in A) = sum sum_((x,y) in A) p(x, y)$$

## Distribuciones Bivariadas [[variable aleatoria continua]]

Se aplican cuando las variables aleatorias pueden tomar cualquier valor dentro de un rango continuo. La distribución conjunta se representa mediante una [[funcion densidad de probabilidad]] conjunta $f(x,y)$ que describe la probabilidad de que $X$ y $Y$ se encuentren dentro de un área específica en su espacio de valores.

Sea entonces $A$ una v.a. donde $A subset.eq RR^2$. Y su funcion acumulada se denota como $F(x,y)$

$$F(x,y) = integral_(-oo)^x integral_(-oo)^y f(t,s) d s dot d t$$

>[!example]
>- Supongamos que solo hay tres categorías de altura: **baja, media, y alta**, y tres categorías de cantidad de comida: **poca, moderada, y mucha**.
>- Si observas cómo se distribuyen los invitados entre estas categorías, puedes crear una tabla donde cada celda representa la probabilidad de que un invitado tenga una cierta **altura** y coma una cierta **cantidad** de comida.
>- Por ejemplo, podrías encontrar que hay una alta probabilidad de que las personas altas coman mucha comida, mientras que las personas bajas tienden a comer menos.



