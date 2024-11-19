---
title: Predicciones de modelos lineales en R
feed: show
date: 17-11-2024
tags:
  - estadistica
  - ai
  - ml
curso:
---
```r
predict.lm(modelo, newdata = data.frame(X= $valor))
```

# Intervalo
En el caso de querer un intervalo de confianza
```r
predict.lm(modelo, newdata = data.frame(X= $valor), interval = "confidence" or "predict")
```

>[!note] Diferencias entre confidence y predict
>

