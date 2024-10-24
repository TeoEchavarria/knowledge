---
title: Sigmoide - RNN
feed: show
date: 07-10-2024
---

En [[keras]]: `"sigmoid"`

$$sigma(z) = 1/(1+exp^(-z))$$
![[Funciones de activación.pdf#page=3&rect=50,400,519,763&color=red|Funciones de activación, p.3|400]]

> Problemas de clasificacion Binaria

> [!PDF|red] [[Funciones de activación.pdf#page=2&selection=12,0,20,38&color=red|Desventaja:]]
> > Cuando las entradas se vuelven pequeñas o grandes la función se concentra en $0$ o en $1$, llegando a una derivada cercana a $0$. Esto conlleva que no tenga gradiente a propagarse en estas zonas a través de la red, por lo que no queda casi nada para las capas inferiores. Esto se conoce como [[desvanecimiento del gradiente]]


### Solución:

Este problema es una de las razones por las que se utilizan otras funciones de activación, como **[[ReLU]]** (Rectified Linear Unit), que no sufre tanto de desvanecimiento del gradiente porque su derivada es constante en muchas zonas de su dominio.