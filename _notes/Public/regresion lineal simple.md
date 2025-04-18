---
title: Regresion Lineal Simple
feed: show
date: 01-01-2025
tags: 
curso:
---
Permite establecer asociaciones, en este caso lineales, entre las variables de interes.

$$Y_i = beta_0+beta_i X + Epsilon_i$$

Expresado en otros terminos: [[SST]] = [[SSR]] + [[SSE]] ^2e68f3

Donde $Epsilon_i$ es una variable de error iid con distribucion $N tilde (0,sigma^2)$ 

# Pasos 
- Denifir $X$ y $Y$ 
- [[pruebas de hipotesis relacionado con determinar la relevancia variables sobre Y]]
- [[validacion modelo analisis residuales]]
- [[prueba de normalidad para los errores]]
- [[prediccion de modelos lineales]]
# Enfoques 

-  [[Enfoque probabililistico - metodo de maxima verosimilitud]]
- [[Enfoque no probabilistico - metodo de minimos cuadrados]]


>[!warning] 
>Como $Y_i$ es una funcion de [[variable aleatoria]] [[distribucion normal|normal]], entonces $Y_i$ tambien es normal


> $beta_0$ = Solo tiene interpretacion cuando $x_i$ puede tomar valor de $0$
> $beta_i$ = El cambio esperado de $y_i$ por un incremento unitario en la variable predictoria $x_i$

## Subtemas
- [[intervalos de confianza para regresiones lineales simples]]
- [[regresiones lineales en R]]



