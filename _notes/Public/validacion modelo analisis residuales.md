---
title: Validacion de un modelo por medio de analizar sus resudiales
feed: show
date: 17-11-2024
tags:
  - ai
  - estadistica
  - ml
curso:
---
Recuerde que los supuestos sobre los errores asumidos en el modelo de [[regresion lineal simple|RLS]] se pueden resumir como:$$ε_i op(""tilde"", limits: #true)_text("iid") N(0 , σ^2), i = 1, . . . , n $$donde, iid. es la abreviación de independiente e idénticamente distribuido.
![[clase3.pdf#page=7&rect=20,-2,440,254|clase3, p.7]]


[[R]] `plot(modelo, 1)` en el caso de [[regresion lineal simple]]

`plot(modelo,2)` en el caso de [[regresion lineal multiple]] ^5c2dc1

![[residuals.png|350]]
