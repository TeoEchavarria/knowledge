---
title: Prueba de Linealidad General
feed: show
date: 17-12-2024
tags:
  - estadistica
  - ml
  - R
curso:
---
$$H_0 : L underline(beta) = Omicron$$

$$H_1 : L underline(beta) != Omicron$$

Donde: 
- $L$ es una matriz $m times p$
- $underline(beta)$ una matriz $p times 1$ 
- $Omicron$ una matriz $m times 1$
y $m$ es el numero de hipotesis que se desean probar de manera simultanes

## Ejemplo:
$$H_o : beta_2=0; beta_1=beta_3$$
$$H_1 : beta_2!=0 or beta_1!=beta_3$$
Escribiendo ahora el modelo reducido, tenemos que $beta_1 - beta_3 = 0$; por lo que $X_(13) = X_1+X_3$
Llegando a un modelo reducido de la forma:
$$y=beta_0 + beta_1 X_13 + epsilon$$
$$$$
Escrito de forma matricial:
$$mat(0,0,1,0;0,1,0,-1) mat(beta_0;beta_1;beta_2;beta_3)=mat(0;0)$$

$$F_("par") = ("SSH"/r)/"MSE del Modelo Completo" tilde F_(r, n-p)$$
$$"SSH" = "SSR"(F M) - "SSR"(R M)$$
$$="SSE"(R M) - "SSE"(F M)$$
> $r$ numero de filas linealmente independientes en la matriz $L$ 

> Veamos que para el ejemplo $r=2$ para el ejemplo

