---
title: Métodos Automáticos de Selección de Variables en Regresión
feed: show
date: 03-02-2025
tags: ['Regresión', 'Selección de Variables', 'Estadística', 'Modelado Predictivo']
---

Exploramos tres métodos computacionalmente eficientes para la selección de variables en regresión:  [[metodo de seleccion hacia adelante en regresion - backward]], [[metodo de eliminacion hacia atras en modelos estadisticos -  forward]] y [[método de selección paso a paso - stepwise]]. Cada método opera secuencialmente para identificar variables significativas.

- La Selección Hacia Adelante comienza con un modelo vacío y agrega variables una por una basándose en un criterio de ajuste, como el [[AIC]] o el [[BIC]].
- La Eliminación Hacia Atrás inicia con todas las variables y elimina aquellas que no contribuyen significativamente al modelo.
- La Selección por Pasos combina ambos enfoques, añadiendo y eliminando variables para optimizar el [[modelo]].
- Estos métodos son útiles cuando se trabaja con grandes conjuntos de datos y se busca reducir la dimensionalidad.
- Cada método tiene sus ventajas y desventajas en términos de precisión y eficiencia computacional.

$$ "AIC" = 2k - 2 ln( "hat" L) $$

$$ "BIC" = k ln(n) - 2 ln( "hat" L) $$


```
# Ejemplo de Selección Hacia Adelante en Python usando statsmodels
import statsmodels.api as sm
import pandas as pd

def forward_selection(data, response):
    remaining = set(data.columns)
    remaining.remove(response)
    selected = []
    current_score, best_new_score = float('inf'), float('inf')
    while remaining and current_score == best_new_score:
        scores_with_candidates = []
        for candidate in remaining:
            formula = "{} ~ {}".format(response, ' + '.join(selected + [candidate]))
            score = sm.OLS.from_formula(formula, data).fit().aic
            scores_with_candidates.append((score, candidate))
        scores_with_candidates.sort()
        best_new_score, best_candidate = scores_with_candidates.pop(0)
        if current_score > best_new_score:
            remaining.remove(best_candidate)
            selected.append(best_candidate)
            current_score = best_new_score
    formula = "{} ~ {}".format(response, ' + '.join(selected))
    model = sm.OLS.from_formula(formula, data).fit()
    return model
```

>[!example] En un estudio de mercado, se utiliza la Selección Hacia Adelante para identificar las características del producto que más influyen en las ventas.

>[!example] En un análisis de datos médicos, la Eliminación Hacia Atrás ayuda a determinar qué factores de riesgo son más relevantes para una enfermedad.

>[!example] La Selección por Pasos se aplica en la ingeniería para optimizar modelos predictivos de fallos en maquinaria.
