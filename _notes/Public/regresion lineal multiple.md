---
title: Regresion Lineal Multiple
feed: show
date: 03-12-2024
tags:
  - estadistica
  - ml
curso:
---
Es una funcion de relaciones lineales con dos o mas variables preductoras, formuladas simultaneamente en un unico modelo.
![[clase5.pdf#page=12&rect=76,37,381,67|clase5, p.12|450]]
Donde $$epsilon_i op(""tilde"", limits: #true)_text("iid") N(Omicron , σ^2), i = 1, . . . , n $$

$$underline(y) = X underline(beta) + underline(epsilon)$$
Llegandose a ver de la forma: $$mat(y_1;y_2;dots.v;y_n) =
mat(
  1, x_11, ..., x_(1 k);
  1, X_21, ..., x_(2 k);
  dots.v, dots.v, dots.down, dots.v;
  1, x_(n 1), ..., x_(n k);
) 
mat(beta_0;beta_1;dots.v;beta_k) +
mat(epsilon_1;epsilon_2;dots.v;epsilon_3)
$$
Donde:
 - $underline(y)=$  Es el vector $n times 1$ de observaciones.![[SST#^2ec09a]]
 - $X=$ Es una matriz $n times p$ con los valores de predictoras.
 - $underline(beta)=$  Es el vector de $p times 1$ parámetros.![[SSR#^f2ba51]]
 - $underline(epsilon)=$  Es el vector $n times 1$ de errores aleatorios ![[SSE#^9ffca9]]

## Ecuacion de regresion ajustada

![[clase5.pdf#page=30&rect=114,49,342,82|clase5, p.30|400]]
Donde la estimacion de los parametros de modelo matriz beta gorro se calcula de la forma:
![[clase5.pdf#page=30&rect=177,151,266,171&color=important|clase5, p.30|180]]

### Estimación de la Varianza
![[varianza#^e8743d]]

## Validar la significancia del modelo
![[anova#^85d964]] En este caso lo que usamos es el $F$ calculado 

## Inferencia sobre los parametros del modelo de regresion
![[intervalos de confianza para regresiones lineales multiples#^e1eda5]]
Con lo que podemos contruir un [[intervalos de confianza]] de la forma ![[intervalos de confianza para regresiones lineales multiples#^847a73]]

Claro antes de eso hay que validar los supuestos, esto se hace por medio de pruebas ![[prueba de normalidad para los errores]]
Y de igual forma por medio de la grafica de los resuduos por medio de ![[validacion modelo analisis residuales#^5c2dc1]]
## Pruebas de significancia
- [[prueba lineal general]]
- [[prueba de significancia para parametros individuales]] => Para este ya la funcion `sumary` en la ultima fila que es el [[p-valor]] nos indica que tan significante es esa variable para el modelo
- [[prueba de significancia subconjunto parametros]]

>[!note] Relacionado con: 
>- [[intervalos de confianza para regresiones lineales multiples]]
>- [[IC para la respuesta media]]
>- [[IP para un valor futuro]]
>- [[puntos de balanceo]]

