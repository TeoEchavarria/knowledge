---
title: Método de Selección Hacia Adelante en Regresión
feed: show
date: 03-02-2025
tags: ['Regresión', 'Selección de Variables', 'Estadística', 'Modelado Predictivo']
---

El método de selección hacia adelante es una técnica de regresión que comienza con modelos simples y agrega variables basándose en el criterio de menor error cuadrático medio ([[MSE]]) y significancia estadística. Se continúa añadiendo variables utilizando estadísticas F parciales hasta que no queden variables significativas.

- Comienza con un modelo de [[regresion lineal simple]].
- Selecciona el [[modelo]] con el menor error cuadrático medio (MSE).
- Añade variables basándose en la significancia estadística y el criterio de F parcial.
- El proceso continúa hasta que no se puedan añadir más variables significativas.
- Es útil para identificar el mejor subconjunto de variables predictoras.

$$ "MSE" = (1)/(n) sum_(i=1)^(n) (y_i - "hat" y_i)^2 $$

$$ F = (("SSR"_("new") - "SSR"_("old")) / p)("SSE"_("new") / (n - k - 1)) $$

![[backward.png]]
```
# Ejemplo de Forward Selection en Python usando statsmodels
import statsmodels.api as sm
import pandas as pd

# Datos de ejemplo
data = pd.DataFrame((
    'X1': [1, 2, 3, 4, 5],
    'X2': [2, 3, 4, 5, 6],
    'X3': [5, 4, 3, 2, 1],
    'Y': [1, 3, 2, 5, 4]
))

# Función para selección hacia adelante
def forward_selection(data, response):
    remaining = set(data.columns)
    remaining.remove(response)
    selected = []
    current_score, best_new_score = float('inf'), float('inf')
    while remaining and current_score == best_new_score:
        scores_with_candidates = []
        for candidate in remaining:
            formula = "() ~ ()".format(response, ' + '.join(selected + [candidate]))
            score = sm.OLS.from_formula(formula, data).fit().aic
            scores_with_candidates.append((score, candidate))
        scores_with_candidates.sort()
        best_new_score, best_candidate = scores_with_candidates.pop(0)
        if current_score > best_new_score:
            remaining.remove(best_candidate)
            selected.append(best_candidate)
            current_score = best_new_score
    formula = "() ~ ()".format(response, ' + '.join(selected))
    model = sm.OLS.from_formula(formula, data).fit()
    return model

# Aplicar selección hacia adelante
model = forward_selection(data, 'Y')
print(model.summary())
```

>[!example] Supongamos que estamos construyendo un modelo para predecir el precio de las casas. Comenzamos con una sola variable, como el tamaño de la casa, y calculamos el MSE. Luego, añadimos variables como el número de habitaciones o la ubicación, evaluando cada vez el MSE y la significancia de las variables añadidas.

>[!example] En un estudio de mercado, se podría comenzar con una variable como el precio del producto y luego añadir variables como la publicidad o la calidad del servicio, evaluando el impacto de cada una en las ventas.
