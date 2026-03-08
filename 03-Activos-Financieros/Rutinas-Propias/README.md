# Bitácora de Evolución del Código: Rutinas Propias

Este documento detalla el progreso en el desarrollo de mi rutina de aprendizaje profundo.

## Historial de Versiones

### Versión 1: Activos financieros.
- **Objetivo:** Partimos del problema de interpolación de funciones, ahora tenemos una base de datos que es el precio de los activos, pero desconocemos completamente la función que represanta en el mercado, así que utilizamos las redes neuronales profundas para poder interpolar cualquer día del costo del activo dentro del rango de tiempo establecido como nuestro dominio.
- **Origen:** Partimos del problema de interpolación de funciones ya resuelto.
- **Funcionalidad:** Tomamos la base de activos desde Yahoo Finance y utilizando ventanas deslizantes de tamaño 60, realizamos la interpolación.
* **Acceso:** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/11D9S774JkvJ6IzIVmgMFRuYqopc8G9EE?usp=sharing)

### Versión 2: Optimización de rutina.
- **Objetivo:** Mejorar los tiempos al reducir las operaciones.
- **Funcionalidad:** Implementar algoritmos para aumentar la eficiencia, utilizando el optimizador Adam, inicialización
de pesos y sesgos adecuada, para reducir la variabilidad, cálculo del error cada 1000 iteraciones en lugar de cada
una de ellas, y segunda condición de paro si el error es lo suficientemente pequeño.
* **Acceso:** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1gwEAn1vVeRC6If57rZQ7UILagJiDNCTh?usp=sharing)

### Versión 3: Interpolación y extrapolación.
- **Objetivo:** Pronosticar 10 días del activo financiero de interes.
- **Funcionalidad:** Utilizando ventanas deslizantes y Recurcive Forecast para pronosticar valor de activos 10 días en el futuro, es decir, en la última ventana con datos reales pronosticamos el día de mañana, para la siguiente ventana usamos 59 datos reales y el pronostico como datos de entrenamiento para pronosticar pasado mañana y así sucesivamente hasta acabar con los 10 días, se imprime el pronostico y se puede guardar en formato .CSV para documentación, así como para ayudar a comparar en el futuro el pronostico vs. datos reales.
* **Acceso:** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/12e7xaYk-6AQA_ISEgNudxzeNTA_z019n?usp=sharing)

### Comparar real Vs pronósticos.
- **Objetivo:** Una vez teniendo los pronosticos podemos realizar la comparación con los datos reales ya sea subiendo el archivo .CSV anteriormente generado o escribiendo directamente los datos de manera manual.
- **Funcionalidad:** El modelo trabaja con ventanas deslizantes y pronostica tomando en cuenta datos que estan equidistantes uno de otro, no tiene distinción en el calendario de los mercados, entonces el pronostico del día 1 puede ser un día festivo o un fin de semana, el modelo se comporta de manera congruente, si tomamos la fecha del día que se hace el pronostico como la fecha ancla y empezamos a contar los días laborales de la bolsa.
* **Acceso:** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1Sdlu1Wcxc9AjMZDuQNOphuiJH22ddWW-?usp=sharing)

---

> **Nota para el lector:** Además de los enlaces a los notebooks de Colab, el código fuente original en `.py` para cada versión también se encuentra disponible en esta carpeta para una consulta técnica más detallada.
