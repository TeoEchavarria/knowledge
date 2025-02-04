---
title: Método de Eliminación hacia Atrás en Modelos Estadísticos
feed: show
date: 03-02-2025
tags: ['estadística', 'modelos estadísticos', 'regresión', 'selección de variables']
---

El método de eliminación hacia atrás es una técnica utilizada en la selección de variables en [[modelo|modelos]] estadísticos. Comienza con un modelo completo que incluye todas las variables posibles y elimina iterativamente aquellas que no son significativas, basándose en el estadístico F parcial más bajo. Este proceso se repite hasta que no se puedan eliminar más variables sin afectar significativamente el modelo.

- Comienza con un modelo completo que incluye todas las variables.
- Se eliminan las variables con el [[estadistico de prueba|estadistico]] F parcial más bajo si no son significativas.
- El proceso se repite hasta que todas las variables restantes sean significativas.
- Ayuda a simplificar el modelo sin perder precisión significativa.
- Es útil en regresiones lineales y otros modelos estadísticos.

$$ F = ("SSR"_("reducido") - "SSR"_("completo"))/(p_("completo") - p_("reducido")) dot "SSR"_("completo")/(n - p_("completo")) $$


![[backward.png]]

```
# Ejemplo en Python usando statsmodels
import statsmodels.api as sm

# Supongamos que tenemos un DataFrame df con las variables independientes X y la dependiente y
X = df.drop('y', axis=1)
y = df['y']

# Agregar constante para el intercepto
X = sm.add_constant(X)

# Ajustar modelo completo
modelo_completo = sm.OLS(y, X).fit()

# Iterar eliminando variables no significativas
while True:
    # Obtener p-valores
    p_values = modelo_completo.pvalues
    # Encontrar la variable con el p-valor más alto
    max_p_value = p_values.max()
    if max_p_value > 0.05:  # Umbral de significancia
        # Eliminar la variable con el p-valor más alto
        X = X.drop(p_values.idxmax(), axis=1)
        # Reajustar el modelo
        modelo_completo = sm.OLS(y, X).fit()
    else:
        break

print(modelo_completo.summary())
```

>[!example] En un estudio de mercado, se comienza con todas las variables demográficas y de comportamiento del consumidor para predecir las ventas. Se eliminan las variables que no contribuyen significativamente al modelo, como la edad o el género, si su estadístico F parcial es bajo.

>[!example] En un análisis de salud, se incluyen inicialmente todas las variables de estilo de vida y antecedentes médicos para predecir el riesgo de enfermedad. Las variables con menor impacto, como el consumo ocasional de alcohol, se eliminan si no son significativas.

>[!danger] Relacionado con [[método de selección paso a paso - stepwise]] , [[metodo de seleccion hacia adelante en regresion - backward]] [[métodos automáticos de selección de variables en regresión]]