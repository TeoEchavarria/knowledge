---
title: Arima
feed: show
date: 01-01-2021
---

Significa "Autoregressive Integrated Moving Average", es un modelo estadístico utilizado para analizar y prever [[serie de tiempo]]. Es especialmente útil para datos que muestran patrones claros de tendencia o [[estacionalidad]].

1. **Autoregressive (AR)**: Esta parte del modelo captura la correlación entre observaciones pasadas y actuales. En términos simples, intenta explicar el valor actual de una serie como una combinación de sus valores anteriores. El componente AR utiliza parámetros conocidos como "lags", que son simplemente valores anteriores en la serie de tiempo.

2. **Integrated (I)**: Esta sección del modelo se encarga de hacer la serie de tiempo estacionaria. Esto implica diferenciar la serie, es decir, calcular las diferencias entre observaciones consecutivas. 

>Esto se hace para eliminar tendencias o ciclos que pueden variar en el tiempo. La integración sugiere cuántas veces se debe diferenciar la serie para alcanzar la estacionariedad.

3. **Moving Average (MA)**: Este componente modela el error de la predicción como una combinación lineal de errores de observaciones pasadas. Ayuda a incorporar "shocks" o innovaciones en la serie de tiempo, que son cambios repentinos que no se pueden explicar por el modelo autoregresivo solo.

>[!code] Mira [aqui](https://www.youtube.com/watch?v=GBy8TJF9vLU) un ejemplo de implementacion
