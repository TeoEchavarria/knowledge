---
title: Puntos de balanceo
feed: show
date: 18-12-2024
tags:
  - estadistica
  - ml
curso:
---
> [!PDF|note] [[clase7.pdf#page=21&selection=6,0,7,82&color=note|clase7, p.21]]
> > Es una observación en el espacio de las predictoras, alejada del resto de la muestra y que puede controlar ciertas propiedades del [[modelo]] ajustado.
> 

Estos puntos pueden tener un impacto significativo en el modelo de regresión, afectando propiedades como los coeficientes estimados y otras estadísticas de resumen, como el [[r-cuadrado]] y los errores estándar de los coeficientes estimados.

> Los puntos de balanceo se pueden identificar a través de su influencia en la [[matriz sombrero]]

![[clase7.pdf#page=22&rect=45,61,418,96&color=note|clase7, p.22]]

![[clase7.pdf#page=23&rect=95,2,367,218&color=note|clase7, p.23]]

## En el caso de ser influyentes dichos puntos de deben tener en cuenta las siguientes medidas:

- [[distancia de Cook]]
- [[diagnostico DFFITS]]
- [[diagnostico DFBETAS]]
