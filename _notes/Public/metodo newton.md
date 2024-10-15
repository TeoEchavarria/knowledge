---
title: "Metodos Numericos : Newton"
feed: show
date: 01-01-2021
---

Sea $f(x)$ una funcion, y $[a,b]$ el intervalo donde queremos probar que existe un punto que pasa por 0

1. Comprobar que $f(x)$ existe en $[a,b]$
2. Que $f(a)dot f(b) < 0$
3. Es [[monotona]] lo que quiere decir que es creciente o decreciente en $[a,b]$ 
	 > Lo que quiere decir que $f^`(x)$ es menor o mayor a cero $forall x in [a,b]$
	 > **POR LO CUAL CUMPLIENDO CON LO ANTERIOR DECIMOS QUE ES UNICA**
1. $f, f^`$ y $f^(``)$ existan en el intervalo $[a,b]$
2.  Construir $p_{n+1}$
 ![[teorema convergencia para cualquier punto inicial iteraciones newton]]
>[!danger]+ Example
>![[ejercicio-metodoNewton.png]]

