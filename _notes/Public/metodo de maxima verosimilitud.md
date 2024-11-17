---
title: Metodo de Maxima Verosimilitud
feed: show
date: 17-11-2024
tags:
  - ai
  - estadistica
  - ml
curso:
---
Es una técnica estadística fundamental utilizada para estimar los parámetros de un [[modelo]] estadístico. Basado en los datos observados, el método busca los valores de los parámetros del modelo que maximizan la probabilidad (verosimilitud) de obtener esos datos.

$$L(θ)=∏_(i=1)^n ​f(x_i​;θ)$$

# Proceso:
- **Especificación del Modelo**: Seleccionar el modelo estadístico apropiado y definir la función de probabilidad adecuada para los datos.
    
- **Función de Verosimilitud**: Construir la función de verosimilitud que representa la probabilidad de los datos dados ciertos parámetros del modelo.
    
- **Maximización**: Usar la log-verosimilitud, una transformación logarítmica de la verosimilitud, para transformar el producto de probabilidades en una suma, facilitando la maximización.
    
- **Solución Analítica**: Derivar la función de log-verosimilitud respecto a los parámetros, igualar a cero para encontrar los puntos críticos y resolver estas ecuaciones para obtener los estimadores de máxima verosimilitud.

>[!note] Contenido : 

