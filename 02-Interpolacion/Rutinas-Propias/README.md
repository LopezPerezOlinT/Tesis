# Bitácora de Evolución del Código: Rutinas Propias

Este documento detalla el progreso en el desarrollo de mi rutina de aprendizaje profundo.

## Historial de Versiones

### Versión 1: Interpolación de funciones
- **Objetivo:** Partimos de una función conocida, tomamos puntos de entrenamiento del dominio e interpolamos puntos desconocidos para el aprendizaje y comparamos gráficamente si el modelo aprendió de manera adecuada.
- **Origen:** Partimos de los problemas de clasificación.
- **Funcionalidad:**  Modificando la arquitectura para que tenga un solo nodo en la capa de entrada y de salida, tambien hay un cambio en el vector auxiliar, se presenta un problema cuando el modelo intenta aprender ya sea puntos del dominio negativos o imágenes negativas, así que se realiza una transformación lineal llamada normalización para el correcto aprendizaje del modelo.
* **Acceso:** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]()

### Versión 2: Optimización de rutina.
- **Objetivo:** Mejorar los tiempos al reducir las operaciones.
- **Funcionalidad:** Implementar optimzador Adam, inicialización de pesos y sesgos adecuado para reducir variabilidad, cálculo del error cada 1000 iteraciones en lugar de cada una de ellas, y segunda condición de paro si el error es lo suficientemente pequeño.
* **Acceso:** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]()

### Versión 3: Rutina final optimizada e implementación del módelo de ventanas deslizantes.
- **Objetivo:** Implementación de ventanas deslizantes para perfilarse a la extrapolación.
- **Funcionalidad:** Dividir los puntos de entrenamiento en conjuntos tamaño 10 consecutivos para pronosticar el punto 11, recorrer hacia la derecha la ventana para entrenar con los puntos del 2 al 11 para pronosticar el punto 12 y así sucesivamente hasta que el modelo aprenda y pueda trabajar con nuevos puntos dentro del mismo dominio.
* **Acceso:** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]()
---

> **Nota para el lector:** Además de los enlaces a los notebooks de Colab, el código fuente original en `.py` para cada versión también se encuentra disponible en esta carpeta para una consulta técnica más detallada.
