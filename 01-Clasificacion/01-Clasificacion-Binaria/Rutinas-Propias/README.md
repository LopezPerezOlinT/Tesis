# Bitácora de Evolución del Código: Rutinas Propias

Este documento detalla el progreso en el desarrollo de mi rutina de aprendizaje profundo.

El objetivo es mantener una documentación en apoyo a la tesis.

## Historial de Versiones

### Versión 1: Implementación Base (Higham & Higham).
- **Objetivo:** Reproducción fiel del seudocódigo.
- **Origen:** Basado en el artículo Deep Learning: An Introduction
for Applied Mathematicians de Higham & Higham.
- **Funcionalidad:** Implementación inicial diseñada para validar los resultados teóricos y validar el algoritmo.
* **Acceso:** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1X0aZkqoxq00aunCFmL9gRAuNDU9LM2wF?usp=sharing)


### Versión 2: Flexibilidad en su Arquitectura e hiperparámetros.
- **Objetivo:** Variantes del resultado con dependencia en la estructura del aprendizaje.
- **Funcionalidad:** Toda una gama de resultados dependiendo de la arquitectura y parámetros.
* **Acceso:** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1Wu0Omp1VcbaF-UacLr98ULt465XTlutl?usp=sharing)


### Versión 3: Evaluación de modelos.
- **Objetivo:** Tener muchos resultados nos lleva a la pregunta ¿Cuál es el correcto?.
- **Funcionalidad:** Realizamos validaciones cruzadas para evaluar el modelo, pero se puede escalar fácilmente buscando
combinaciones de arquitecturas e hiperparámetros por mallado o por búsqueda aleatoria, incluso si encuentras un buen modelo
puedes volver a buscar más combinaciones que se encuentren al rededor de ese modelo. Eso conlleva un costo alto 
computacionalmente hablando y esta fuera del alcance de este trabajo.
* **Acceso:** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1xdM2SH58y_D_YJqXZ_K3NKGhUkVL9G64?usp=sharing)

### Versión 4: Optimización de rutina.
- **Objetivo:** Mejorar los tiempos al reducir las operaciones.
- **Funcionalidad:** Cálculo del error cada 1000 iteraciones en lugar de cada
una de ellas, y segunda condición de paro si el error es lo suficientemente pequeño.
* **Acceso:** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/17yStvhF4M76DHXlFM8cdyeMH1UkUcUnW?usp=sharing)

### Versión 4: Rutina final Optimizada.
- **Objetivo:** Mejorar los tiempos al reducir las operaciones.
- **Funcionalidad:** Implementar algoritmos para aumentar la eficiencia, utilizando el optimizador Adam, inicialización
de pesos y sesgos adecuada, para reducir la variabilidad.
* **Acceso:** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1rJrNSYzvhGpU4ZYLAhx13TOy_GIt9Xaa?usp=sharing)
---

> **Nota para el lector:** Además de los enlaces a los notebooks de Colab, el código fuente original en `.py` para cada versión también se encuentra disponible en esta carpeta para una consulta técnica más detallada.
