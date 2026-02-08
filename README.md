# Estudio Metodológico y Aplicación de Redes Neuronales Artificiales: Desde la Fundamentación Algorítmica hasta PINNs

Este repositorio contiene mi tesis y el código fuente desarrollado para mi trabajo de titulación.

## Estructura de la Investigación
El proyecto está dividido en 5 módulos que reflejan el avance metodológico de la tesis:

* **01. Clasificación Binaria:** Recreación de los resultados (Higham & Higham) y mejoras, así como evaluación del modelo.
* **02. Clasificación Multiclase:** Evolución del entrenamiento de clases binarias a multiclases.
* **03. Aproximación de Funciones:** Estudio de la RNA como interpolador y manejo de transformaciones lineales (Normalización).
* **04. Activos Financieros:** Aplicación a series de tiempo reales mediante ventanas deslizantes para interpolación y extrapolación.
* **05. PINNs (EDOs):** Resolución de ecuaciones diferenciales integrando leyes físicas en la función de costo.

## Implementación Técnica
Todos los problemas fueron desarrollados sin utilizar librerias especializadas en ambiente **Python** y ejecutados en el entorno de **Google Colab** para aprovechar el procesamiento por GPU, asegurando que los modelos de mayor complejidad (como las PINNs) converjan de manera eficiente, despues comparar los resultados con su contaparte utilizando librerias especializadas.

---
*Este repositorio es parte integral de la tesis presentada por López Pérez Olin Tonatiuh para obtener el título de Lic. en Ingeniería Matemática.*
