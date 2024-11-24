---
title: Simulaciones de Monte Carlo
feed: show
date: 24-11-2024
tags:
  - ai
  - ml
  - finanzas
curso:
---
Es una técnica matemática que se utiliza para estimar los posibles resultados de un [[evento]] incierto.

Construye un [[modelo]] de posibles resultados aprovechando una distribución de probabilidad, como una distribución uniforme o [[distribucion normal|normal]], para cualquier variable que tenga incertidumbre inherente. Luego, vuelve a calcular los resultados una y otra vez, cada vez utilizando un conjunto diferente de números aleatorios entre los valores mínimo y máximo. En un experimento típico de Monte Carlo, este ejercicio se puede repetir miles de veces para producir una gran cantidad de resultados probables

## Ventajas
- **Flexibilidad:** No requieren supuestos de normalidad o formulaciones matematicas espacificas, y pueden aplicarse a cualquier distribución de datos.
- **Aplicabilidad en Modelos Complejos**: Pueden generar intervalos de confianza para sistemas muy complejos o para aquellos donde las distribuciones de las variables no son conocidas o son difíciles de modelar analíticamente.
- **Incorporación de Múltiples Variables Aleatorias**: Pueden manejar fácilmente múltiples variables aleatorias con diferentes distribuciones, algo que puede ser complicado en métodos analíticos convencionales.
- **Capacidad de Exploración**: Permiten explorar el efecto de cambiar parámetros del modelo sobre los intervalos de confianza, proporcionando una comprensión más profunda del sistema modelado.



