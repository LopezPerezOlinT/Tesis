# Bitácora de Evolución del Código: Rutinas Propias

En esta sección evoluciona el algoritmo a clasificación multiclase, la diferencia radica en aumentar n-nodos o neuronas
en la capa de salida para n-clases, así como la definición de los vectores auxiliares canonicos de dimención n.

## Historial de Versiones

### Versión 1: Implementación Base (Higham & Higham).
- **Objetivo:** Implementar el aprendizaje a multiclase.
- **Origen:** Partimos del problema de clasificación binaria ya resuelto.
- **Funcionalidad:** Generar puntos aleatorios para cada clase de tal manera que el modelo pueda clasificarlos.
* **Acceso:** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1HXPtn1SAu_JlhEkne5QVNz-s2pzIIlsV?usp=sharing)

### Versión 2: Rutina final Optimizada.
- **Objetivo:** Mejorar los tiempos al reducir las operaciones.
- **Funcionalidad:** Implementar algoritmos para aumentar la eficiencia, utilizando el optimizador Adam, inicialización
de pesos y sesgos adecuada, para reducir la variabilidad, segunda condición de paro y cálculo del error cada 1000 iteraciones.
* **Acceso:** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1liw4mEiKvGcq6EbQTXMGLbDWzscmGiqp?usp=sharing)
---

> **Nota para el lector:** Además de los enlaces a los notebooks de Colab, el código fuente original en `.py` para cada versión también se encuentra disponible en esta carpeta para una consulta técnica más detallada.
