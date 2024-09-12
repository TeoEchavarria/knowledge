---
title: "Corolario : Convergencia de solucion unica de un Sistema Lineal"
feed: show
date: 01-01-2021
---

**Corolario.** Si $\|T\| < 1$ para alguna [[norma matricial]] natural o inducida y $c$ es un [[vector]] cualquiera, la [[sucesión]] $\{x^{(k)}\}_{k=0}^{\infty}$ definida por la iteración $x^{(k+1)} = T x^{(k)} + c$ para $k = 0, \ldots$ [[convergente|converge]] a la solución única del sistema $x = T x + c$ para toda aproximación inicial $x^{(0)} \in \mathbb{R}^n$ y además se cumple

$$
\|x^{(k)} - x\| \leq \|T\|^k \|x^{(0)} - x\|, \quad k = 0,1,\ldots
$$

$$
\|x^{(k)} - x\| \leq \frac{\|T\|^k}{1 - \|T\|} \|x^{(1)} - x^{(0)}\|, \quad k = 0,1,\ldots.
$$
