---
title: MSR
feed: show
date: 17-11-2024
tags:
  - estadistica
  - ai
  - ml
curso:
---
Es una medida de la variabilidad de los datos que se explica por el [[modelo]] de regresión completo (excluyendo el término del error). 

Se calcula dividiendo la suma de cuadrados de la regresión ([[SSR]]) entre los [[grados de libertad]] asociados a la regresión, que son típicamente el número de parámetros estimados menos uno (el número de variables independientes en el modelo).

>[!warning] Donde se usa?
>Se utiliza para evaluar la variabilidad en los datos que el modelo de regresión puede explicar. Es parte del cálculo del F-estadístico en [[anova|ANOVA]], donde se compara el MSR con el [[MSE]] (Media de los Cuadrados del Error): $$F = text("MSR")/text("MSE")$$
>​ Este valor F se utiliza para determinar si el modelo de regresión proporciona un ajuste significativamente mejor a los datos que un modelo que no incluye las variables independientes (modelo nulo).

