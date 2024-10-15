---
title: "Metodos Numericos : Punto Fijo"
feed: show
date: 01-01-2021
---

Si $g(x)$ cumple con el ![[teorema existencia y unicidad del punto fijo]]

Entonces podemos tomar cualquier $p_0$ y ejecutar la siguiente formula $$p_{n+1} = g(p_n)$$
Donde $p_0 in [a,b]$ e iteramos 


>[!example]+ Ejemplo
>Sea $g(x) = \ln\left(\frac{5e^x}{x^2 - 1}\right)$
>
>![[ejercicio-puntoFijo.png|300]]

## Pregunta, cuantas veces tengo que iterar para tener un buen resultado?

Si queremos saber cuantas $n$ veces tenemos que iterar para obtener un error digamos que menor a un $e$ entonces usamos lo siguiente

>[!note]
>Para saber cual de las 3 usar decimos, la que nos de mejor con los datos que nos proporcionan


![[teorema convergencia punto fijo]]

Donde lo que queda luego de escoger alguna de las funciones seria despejar el $n$ y tomar una aproximacion hacia arriba del numero que te da



