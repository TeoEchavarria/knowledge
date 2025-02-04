---
title: Método de Selección Paso a Paso
feed: show
date: 03-02-2025
tags: ['Estadística', 'Regresión', 'Modelado', 'Selección de Variables']
---

El método de selección paso a paso es una técnica estadística que combina los [[metodo de seleccion hacia adelante en regresion - backward]] y [[metodo de eliminacion hacia atras en modelos estadisticos -  forward]] para construir un [[modelo]] de regresión. Este método agrega variables una a una y evalúa la significancia de las variables existentes, permitiendo tanto la adición como la eliminación de variables en pasos sucesivos.

- Combina los métodos de selección hacia adelante y hacia atrás.
- Permite la adición y eliminación de variables en cada paso.
- Evalúa la significancia estadística de las variables en el modelo.
- Optimiza el modelo de regresión para incluir solo variables significativas.
- Ayuda a evitar el sobreajuste al incluir solo variables relevantes.

$$ "Modelo inicial": Y = beta_0 + epsilon $$

$$ "Agregar variable: " Y = beta_0 + beta_1X_1 + epsilon $$

$$ "Evaluar significancia: " H_0: beta_i = 0 "vs" H_1: beta_i != 0 $$

$$ "Eliminar variable si " "-valor" > alpha $$

![[stepwise.png]]

```
# Ejemplo en Python usando statsmodels
import statsmodels.api as sm
import pandas as pd

# Datos de ejemplo
data = pd.DataFrame({
    'X1': [1, 2, 3, 4, 5],
    'X2': [2, 1, 4, 3, 5],
    'Y': [5, 7, 9, 11, 13]
})

# Modelo inicial
X = data[['X1']]
X = sm.add_constant(X)
model = sm.OLS(data['Y'], X).fit()
print(model.summary())

# Agregar variable
X['X2'] = data['X2']
model = sm.OLS(data['Y'], X).fit()
print(model.summary())
```

>[!example] En un estudio de mercado, se utiliza el método de selección paso a paso para identificar las variables demográficas más significativas que afectan las decisiones de compra.

>[!example] En un análisis de salud, se aplica este método para determinar qué factores de estilo de vida están más relacionados con el riesgo de enfermedades cardíacas.
