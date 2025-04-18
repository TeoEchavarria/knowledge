---
title: Optimizacion Multivariada
feed: show
date: 01-04-2025
tags: 
curso:
---
Es fundamental entender cómo encontrar puntos críticos y determinar su naturaleza (máximos, mínimos o puntos de silla).

Por ejemplo, una empresa que produce dos bienes diferentes necesita optimizar sus recursos. Si la función de beneficios es $π(x,y) = 100x + 80y - (x² + xy + y²)$, donde $x$ e $y$ son las cantidades producidas, necesitaríamos encontrar las [[derivada|derivadas]] parciales respecto a x e y, igualarlas a cero y resolver el sistema de [[ecuacion|ecuaciones]] para encontrar el nivel óptimo de producción que maximiza los beneficios.

# Pasos

Para resolver este problema de optimización, sigue estos pasos:

1. Calcula las derivadas parciales: $(∂π)/(∂x) = 100 - 2x - y$ &  $(∂π)/(∂y) = 80 - x - 2y$
2. Iguala ambas derivadas a cero: $100 - 2x - y = 0$  &  $80 - x - 2y = 0$
3. Resuelve el sistema de ecuaciones: De la primera ecuación: $y = 100 - 2x$ Sustituye en la segunda: $80 - x - 2(100 - 2x) = 0 80 - x - 200 + 4x = 0 3x = 120 x = 40$
4. Encuentra y sustituyendo el valor de x: $y = 100 - 2(40)$ por lo que  $y = 20$

Por lo tanto, el punto óptimo es (40,20), que maximiza los beneficios.