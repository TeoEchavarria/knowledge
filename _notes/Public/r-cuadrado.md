---
title: $R^2$
feed: show
date: 17-11-2024
tags:
  - ai
  - ml
curso:
---
Es una medida del ajuste del [[modelo]] que provee un indicador de que tan bien la predictora $X$ predice a la respuesta Y . Se calcula como:

$$R^2 = text("SSR")/text("SST") = 1- text("SSE")/text("SST")$$
>[!note] Relacionada con [[SSE]] [[SSR]] [[SST]] [[r-cuadrado ajustado]]

> [!PDF|red] [[clase2.pdf#page=19&selection=0,0,33,21&color=red|clase2, p.19]]
> > Interpretaciones erróneas de $R^2$. 
> > - Un $R^2$ alto indica que el modelo puede hacer predicciones útiles. 
> > - Un $R^2$ alto indica que la recta de regresión tiene buen ajuste. 
> > - Un $R^2$ cercano a cero indica que X y Y no están relacionados
> 

> [!PDF|important] [[clase6.pdf#page=9&selection=0,69,23,40&color=important|clase6, p.9]]
> > Aunque es usado como una medida de bondad del ajuste de la función de regresión, es necesario tener presente que: 
> > - Valores grandes de $R^2$ no implican necesariamente que la superficie ajustada sea útil. Puede suceder que se hayan observado pocos niveles de las variables predictoras y por tanto la superficie ajustada no sería útil para hacer extrapolaciones por fuera de tales rangos. Incluso, si esta cantidad es muy cercana a 1, todavía el MSE podría ser muy grande y por tanto las inferencias tendrían poca precisión. 
> > - Cuando se agregan más variables predictoras al modelo, el $R^2$ tiende a no decrecer, aún cuando existan dentro del grupo de variables, un subconjunto de ellas que no aportan significativamente.
> 


