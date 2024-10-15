---
title: "Metodos Numericos : Orden de convergencia"
feed: show
date: 01-01-2021
---

Supongamos que  es sucesión que converge a , con , . Si existen constantes positivas  y  tales que

$$
lim_(n arrow infinity) (|p_(n+1) - p|)/(|p_n - p|^alpha) = lambda
$$

entonces $p_n_(n in NN)$ converge a $p$ con orden $alpha$ y una constante asintótica $lambda$.

O equivalentemente, existe una constante $C > 0$ tal que

$$
|p - p_(n+1)| <= C|p - p_n|^alpha text(" y ") forall n in NN.
$$

En general, entre $α$ mas grande, la convergencia es mas rapida.
- En particular si $α = 1$ la sucesion sera linealmente [[convergente]],  
- Si $α = 2$ la sucesion sera cuadraticamente [[convergente]].

>[!danger]+ Tener en cuenta
>Cuando se escoge un $alpha$ incorrecto esto puede hacer que la [[convergente|convergencia]] sea mas tardada

