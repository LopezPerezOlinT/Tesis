### Comparativa con Librerías Especializadas de Machine Learning & Deep Learning

En esta sección se utiliza el poder de frameworks comerciales para validar y contrastar los resultados obtenidos con las **Rutinas Propias**.
# Comparativa con Librerías Especializadas de Machine Learning & Deep Learning

En esta sección se utiliza el poder de frameworks comerciales para validar y contrastar los resultados obtenidos con las **Rutinas Propias**.

## Objetivo de la Comparación
El objetivo principal es establecer un punto de referencia (benchmark) confiable. Al comparar nuestros desarrollos personalizados con herramientas estandarizadas y ampliamente validadas, podemos:
- **Validar la precisión y el comportamiento** de nuestras rutinas.
- **Identificar diferencias clave** en aspectos como la convergencia, la inicialización de pesos o la velocidad de entrenamiento.
- **Cuantificar el rendimiento** relativo de nuestra implementación.

## Bitácora de Pruebas y Versiones

- **Versión 1:** Interpolación y primer intento de extrapolación
- **Librería usada:** tensorFlow/keras/sklearn
- **Descripción:** Interpolación de funciones y extrapolación sin uso de ventanas deslizantes, solamente con el modelo entrenado pedirle que clasifique puntos fuera del dominio a la derecha.
- **Acceso:** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1ek_rtLBXVoiZOgzaKBbUXZE0imvipwf6?usp=sharing)


