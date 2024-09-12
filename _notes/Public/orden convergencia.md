---
title: "Metodos Numericos : Orden de convergencia"
feed: show
date: 01-01-2021
---

Supongamos que  es sucesión que converge a , con , . Si existen constantes positivas  y  tales que

$$
\lim_{n \to \infty} \frac{|p_{n+1} - p|}{|p_n - p|^\alpha} = \lambda
$$

entonces $\{p_n\}_{n\in\mathbb{N}}$ converge a $p$ con orden $\alpha$ y una constante asintótica $\lambda$.

O equivalentemente, existe una constante $C > 0$ tal que

$$
|p - p_{n+1}| \leq C|p - p_n|^\alpha \quad \forall n \in \mathbb{N}.
$$

En general, entre $α$ mas grande, la convergencia es mas rapida.
- En particular si $α = 1$ la sucesion sera linealmente [[convergente]],  
- Si $α = 2$ la sucesion sera cuadraticamente [[convergente]].

>[!danger]+ Tener en cuenta
>Cuando se escoge un $\alpha$ incorrecto esto puede hacer que la [[convergente|convergencia]] sea mas tardada

