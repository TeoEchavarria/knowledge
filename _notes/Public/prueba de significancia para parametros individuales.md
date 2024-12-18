---
title: Prueba de Significancia para parametros individuales
feed: show
date: 17-12-2024
tags:
  - estadistica
  - ml
curso:
---
En este caso realizamos una [[pruebas de hipotesis]] en donde $$H_0: beta_j = 0$$ $$H_1 : beta_j != 0$$
Donde nuestro [[estadistico de prueba]] sera: $$T_(j,0) = overline(beta_j)/("se" overline(beta_j)) op(""tilde"", limits: #true)^text("bajo" H_0) t_(n-p)$$
Donde $s e$ es el `error estandar` que se ve en la segunda fila del sumary del modelo: 
```yaml
Coefficients:
            Estimate Std. Error t value Pr(>|t|)
(Intercept)  5.032    0.220      22.873  < 2e-16 ***
X1           0.044    0.010      4.400   0.000134 ***
X2          -0.198    0.030     -6.600   2.53e-10 ***
X3           0.001    0.005      0.200   0.841
---
Signif. codes:  0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1
``` 

