---
title: "Distribucion : Acumulada"
feed: show
date: 01-01-2021
---


Sea $p(x)$ su [[funcion masa de probabilidad]] Por lo que su distribucion acumulada va ser igual a  $$F(X) = P(X <= x)=sum_{x_i <= x} p(x_i)$$ 

En otras palabras es como sumar cada una de las probabilidades de $x$ hacia atras.

## [[variable aleatoria continua]]

Sea $f(x)$ su [[funcion densidad de probabilidad]] Por lo cual su distribucion acumulada va a ser igual a :  $$F(X) = integral_{-infinity}^infinity f(t) d t$$

### Propiedades

 $$0 <= F(x) <= 1$$ 
 $$text("Si ") x < y text(" Entonces")  F(x) < F(y)$$ 
 $$P(a <= X <= b) = P(X <= b) - P(X <= a) = F(b) - F(a)$$ 
