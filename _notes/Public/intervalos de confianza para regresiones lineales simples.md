---
title: Intervalos de Confianza para Regresiones Lineales Simples
feed: show
date: 17-11-2024
tags:
  - ai
  - estadistica
  - ml
curso:
---
Para una [[regresion]] la expresion:
$$beta_0 plus.minus t_(alpha/2, n-2) times sqrt((sigma^2 sum_(i=1)^n x_i^2)/(n S_(x x)))$$

Donde el valor de la t-Student es el valor critico de la distribucion, correspondiente al nivel de confianza que se desea. Y el termino dentro de la raiz cuadrada corresponde al error estandar 

[[R]] `confint(modelo)`
![[confint.png|350]]

### Como lo interpreto?
Con un incremento unitario, el valor esperado de $y$ esta entre $[20.489, 21.902]$
