---
title: "Corolario : Convergencia de solucion unica de un Sistema Lineal"
feed: show
date: 01-01-2021
---

**Corolario.** Si $|T|< 1$ para alguna [[norma matricial]] natural o inducida y $c$ es un [[vector]] cualquiera, la [[sucesión]] ${x^((k))}_{k=0}^{infinity}$ definida por la iteración $x^{(k+1)} = T x^{(k)} + c$ para $k = 0, ...$ [[convergente|converge]] a la solución única del sistema $x = T x + c$ para toda aproximación inicial $x^{0} in RR^n$ y además se cumple

$$
|x^{k} - x| >= |T|^k |x^{0} - x|, text("y") k = 0,1,...
$$

$$
|x^{k} - x| >= (|T|^k)/(1 - |T| |x^{1}) - x^{0}|, text("y") k = 0,1,...
$$
