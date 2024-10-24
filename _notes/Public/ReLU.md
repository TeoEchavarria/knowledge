---
title: ReLU - RNN
feed: show
date: 07-10-2024
---

En [[keras]]: `"relu"`
$$R e L U(z)= max(z,0)$$
> Funcion de activacion mas utilizada en [[deep learning]]

![[Funciones de activación.pdf#page=7&rect=32,80,510,573&color=red|Funciones de activación, p.7|500]]


- **Mejor propagación del gradiente:** menos problemas de fuga de gradiente en comparación con las funciones de activación [[sigmoide]] y [[tangente hiperbólica|tahn]]. 

- En la región donde $x>0$, la derivada de ReLU es **1**, lo que significa que los gradientes pueden propagarse fácilmente sin volverse muy pequeños *(como ocurre con la sigmoide)*. Esto mejora la **eficacia del aprendizaje** en redes profundas, ya que el gradiente no se desvanece tan rápidamente como en las funciones sigmoide o tangente hiperbólica.

- Esto crea un comportamiento donde algunas neuronas no participan activamente en la propagación hacia adelante ni en la retropropagación, ya que el valor de salida es 0. Esto puede ser beneficioso porque **reduce la complejidad del modelo** al "apagar" neuronas que no contribuyen significativamente al resultado final.


- Si la entrada es positiva, la salida puede ser cualquier valor positivo sin límite superior. Esto es útil porque permite que el modelo **capture relaciones no lineales** mucho más fácilmente, especialmente cuando se trata de datos que necesitan representar valores grandes.