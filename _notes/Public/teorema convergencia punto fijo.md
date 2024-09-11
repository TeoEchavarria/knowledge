---
title: "Teorema : Convergencia de punto fijo"
feed: show
date: 01-01-2021
---

Si se satisface el [[teorema existencia y unicidad del punto fijo]]  en $[a, b]$, para cualquier $p_0 \in [a, b]$ la sucesión generada por la iteración $p_n = g(p_{n-1}), \forall n \geq 1$, converge a $p$ y se cumple

- $$|p_n - p| \leq k^n |p_0 - p|, \forall n \geq 1$$
- $$|p_n - p| \leq k^n \max\{b - p_0, p_0 - a\}, \forall n \geq 1$$
- $$|p_n - p| \leq \frac{k^n}{1 - k} |p_1 - p_0|, \forall n \geq 1$$

Sea este usado cuando tenemos un [[criterio de parada]] estipulado, y deseamos saber cuantas iteraciones nos va a tomar lograr llegar a ese criterio de parada el cual comunmente es que el [[error]] sea muy pequeño en cuanto al real, o que el cambio entre un $p_{n+1}$ y un $p_n$ ya sea demasiado pequeño

