---
title: Regresión con Variables Indicadoras
feed: show
date: 03-02-2025
tags: ['regresión', 'variables indicadoras', 'multicolinealidad', 'estadística']
---

Las variables indicadoras se utilizan en regresión para representar predictores categóricos. Es crucial evitar la [[multicolinealidad]] perfecta eliminando el intercepto o una de las variables indicadoras.

- Las variables indicadoras permiten incluir variables categóricas en [[modelo|modelos]] de regresión.
- Cada categoría se representa mediante una variable indicadora binaria (0 o 1).
- Para evitar la multicolinealidad perfecta, se debe eliminar el intercepto o una de las variables indicadoras.
- La elección de la categoría de referencia afecta la interpretación de los coeficientes.

$$ y = beta_0 + beta_1 x_1 + beta_2 x_2 + epsilon $$

$$ y = beta_1 x_1 + beta_2 x_2 + epsilon quad "sin intercepto" $$

```
# Ejemplo en Python usando pandas y statsmodels
import pandas as pd
import statsmodels.api as sm

# Datos de ejemplo
data = {'Salario': [50000, 60000, 55000, 65000],
        'Genero': ['Masculino', 'Femenino', 'Femenino', 'Masculino']}
df = pd.DataFrame(data)

# Crear variables indicadoras
indicadores = pd.get_dummies(df['Genero'], drop_first=True)

# Concatenar con el DataFrame original
X = pd.concat([indicadores], axis=1)
X = sm.add_constant(X)  # Añadir intercepto

# Modelo de regresión
modelo = sm.OLS(df['Salario'], X).fit()
print(modelo.summary())
```

>[!example] Supongamos que tenemos una variable categórica 'Color' con categorías 'Rojo', 'Azul' y 'Verde'. Podemos crear dos variables indicadoras: 'Rojo' y 'Azul'. Si ambas son 0, implica que el color es 'Verde'.

>[!example] En un estudio de salarios, si 'Género' es una variable categórica con 'Masculino' y 'Femenino', podemos usar 'Femenino' como variable indicadora y eliminar el intercepto para evitar multicolinealidad.
