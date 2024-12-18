---
title: Prueba de significancia para subconjunto de parametros
feed: show
date: 05-12-2024
tags:
  - estadistica
  - R
  - ml
curso:
---
Como saber que aporte tienen variables nuevas en un [[modelo]] de [[regresion lineal multiple]] 

> [!PDF|note] [[clase6.pdf#page=15&selection=28,0,32,1&color=note|clase6, p.15]]
> > Una forma de medir la importancia de un subconjunto de coeficientes en un modelo de RLM es a través de las denominadas [[sumas extra de cuadrados]].
> 

# Explicacion Teorica
![[clase6.pdf#page=17&rect=11,4,425,214&color=note|clase6, p.17]]
![[clase6.pdf#page=18&rect=18,27,428,236&color=note|clase6, p.18]]
# Explicacion Practiva - Ejemplo

Planteemos un ejemplo practico donde ![[clase6.pdf#page=33&rect=14,165,439,214&color=important|clase6, p.33]]
Vemos que esto podemos escribirlo como:
![[clase6.pdf#page=33&rect=141,110,318,137&color=important|clase6, p.33|400]]
Y luego esto verlo como una matriz de la forma:
![[clase6.pdf#page=33&rect=98,12,360,89&color=important|clase6, p.33]]
Vemos que la matriz $L$ tiene $r=3$ filas linealmente independientes

Para esta prueba tendremos que crear un modelo alterno en [[R]] que encapsule esta prueba de significancia. De la forma 
```
modelo = lm(Y~X1 + X2 + X3 + X4)

X34 = X3+X4
modelo2 = lm(Y~X34)
```

Dado que $X_1$ y $X_2$ son iguales a cero. Entonces calculamos el [[estadistico de prueba]] que es: 
$$F_0="SSH"/r/"MSE" tilde F_(r,n-p)$$
Donde el $"SSH"$ va a ser *"suma de cuadrados de la hipotesis"*, el $r$ se definio arriba y el *"MSE"* es el del modelo completo, usaremos entones el [[anova]]\_table_lm para ver esos valores, llegando a algo asi:
![[anova_f0_test_reducido.png]]

$$F_0 = 6000557/3/293 tilde F_(3, 996)$$
  >[!note] Relacionado con : [[SSE]] [[SSR]] 


