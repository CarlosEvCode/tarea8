# Clasificador de Formas Geométricas

Proyecto de aprendizaje automático para clasificar formas básicas (círculos, cuadrados y triángulos) en tiempo real.

## Flujo de Trabajo

* **Generación de datos:** Se usó Processing en la carpeta `GeneradorFormas` para generar 100 imágenes PNG de 64x64 píxeles para cada figura geométrica.
* **Entrenamiento:** En `entrenamiento.html` se cargaron las 300 imágenes etiquetadas, se normalizaron los datos y se entrenó la red neuronal (`ml5.neuralNetwork`) con 50 épocas. El modelo resultante se guardó en la carpeta `model/`.
* **Prueba:** En `index.html` se cargó el modelo entrenado y se habilitó un lienzo interactivo de 400x400 para dibujar con el ratón y predecir las formas en tiempo real, mostrando su etiqueta y porcentaje de confianza.
