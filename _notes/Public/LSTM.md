---
title: Long Shot-Term Memory
feed: show
date: 15-03-2025
tags:
  - ai
  - ml
curso:
---
Es un tipo de [[redes neuronales|red neuronal]] recurrente (RNN) diseñada para procesar y aprender de secuencias de datos, superando algunas limitaciones de las RNN tradicionales.

### Características Clave

- **Memoria a largo plazo:**  
    La estructura de un LSTM incluye una "célula de memoria" que permite mantener información durante períodos prolongados, lo que es crucial para aprender dependencias a largo plazo en secuencias.
    
- **Puertas de control:**  
    Los LSTM utilizan mecanismos llamados "puertas" para gestionar el flujo de información:
    
    - **Puerta de entrada:** Decide qué información nueva se añade a la célula.
    - **Puerta de olvido:** Determina qué información antigua se descarta.
    - **Puerta de salida:** Controla qué información se extrae de la célula para ser utilizada en la salida.

![[LSTM.png]]

>[!note] Explicacion
>**Sigmoide** : ![[sigmoide#^2c33e5]]
>**Tanh** :![[tanh#^09a50d]]

>[!warning] Gates
>- **Forget** - Usa una [[sigmoide|sig]] dado que dice que se olvida y que no
>- **Input** - Usa [[sigmoide|sig]] para decir *CUANTA* informacion entra y [[tanh]] para decir si es informacion valiosa
>##### Actualización del Estado de la Célula 
>Combina lo que has “olvidado” con lo que vas a “agregar”.
$$c_{t} = (c_{t-1} \times \text{Forget Gate}) + (\text{Candidate} \times \text{Input Gate})$$
>- **Output** - Usa [[sigmoide|sig]] por decir que parte de $c_t$ muestra y [[tanh]] se usa para escalar el resultado de $c_t$


