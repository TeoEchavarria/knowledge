---
title: "Metodos Numericos : Biyeccion"
feed: show
date: 01-01-2021
---

En si el metodo de biyeccion es una serie de pasos:

1. Garanticemos que existe cero entre $[a,b]$ para la funcion $f(x)$
Eso lo hacemos por medio del ![[teorema_valor_intermedio#^f06dfb]]
Que en otras palabras es si existe un valor $k$ entre $[a,b]$ entonces existe almenos un $f(c)=k$

2. Ver que $f(a)\cdot f(b) < 0$ 
>[!note] Lo que significa
>Que una punta es positiva y la otra negativa, por lo que tiene que cortar a el eje $X$

3. Calculamos $$p_0=\frac{b-a}{2}$$
4. Reemplazamos ese $p_0$ por $a$ o $b$ manteniendo siempre el hecho de que $f(a)\cdot f(b)<0$ 
5. Repetimos hasta encontrar a $0$ o hasta un determinado parametro de parada

>[!image] Grafica
![[biyeccion-grafic.png]]
![[biyeccion-grafic-lineal.png]]

>[!process] Procedimiento
>![[biyeccion-grafic-process.png]]

