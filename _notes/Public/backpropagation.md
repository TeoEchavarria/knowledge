El backpropagation calcula el [[gradiente descendente]] del error de la [[redes neuronales|RNA]] con respecto a cada parámetro del modelo. En otras palabras, puede hallar cómo se debe ajustar cada peso de conexión y cada término de bias para reducir el error.

En resumen, para cada instancia de entrenamiento, el algoritmo de backpropagation:
1. **Forward pass:** Hace una predicción y Mide el error
3. **Backward pass**: Pasa por cada capa en sentido inverso para medir la contribución de error de cada conexión
4. **Gradient Descent step:** Modifica los pesos de conexión para reducir el error