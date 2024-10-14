Las capas más cercanas a la entrada de la red no reciben suficiente señal de error para ajustarse, haciendo que el aprendizaje sea extremadamente lento o, en algunos casos, imposible.

En otras palabras, los **pesos en las capas inferiores apenas cambian** porque el gradiente es prácticamente **cero**.

### Resumen del problema:

- Cuando las entradas a la función sigmoide son grandes o pequeñas, la función tiende a 0 o 1.
- En estos rangos, la derivada de la sigmoide se acerca a 0.
- Si la derivada es casi 0, el gradiente que se retropropaga a través de la red es muy pequeño.
- Esto afecta el aprendizaje de las capas más profundas (inferiores), ya que no hay suficiente gradiente para ajustar los pesos en esas capas.

