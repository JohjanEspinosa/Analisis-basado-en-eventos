# Análisis del Embudo de Ventas y Test A/A/B para App de E-commerce

## Descripción del Proyecto
Este proyecto fue desarrollado para una empresa emergente del sector de alimentos, con el objetivo de analizar el comportamiento de los usuarios en su aplicación móvil. La investigación se dividió en dos partes principales: el **análisis del embudo de ventas** para identificar las etapas de mayor abandono, y la **evaluación de un test A/A/B** para determinar si un nuevo diseño de fuentes afectaba la conversión de los usuarios.

## Objetivo
* **Evaluar el embudo de ventas:** Comprender el recorrido del usuario desde su primer evento hasta la compra, identificando las tasas de conversión y las etapas con mayor pérdida de usuarios.
* **Analizar un test A/A/B:** Determinar si un cambio en las fuentes de la aplicación tiene un impacto estadísticamente significativo en la interacción y conversión de los usuarios.

## Herramientas Utilizadas
-   **Lenguaje:** Python
-   **Librerías de Python:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `scipy`
-   **Entorno de Desarrollo:** Jupyter Notebook
-   **Análisis Estadístico:** Pruebas de hipótesis (Prueba Z)

## Fases del Análisis

### 1. Preparación y Exploración de Datos
* Se realizó la carga del archivo `logs_exp_us.csv`.
* Se renombraron las columnas para facilitar el análisis y se verificaron los tipos de datos y valores ausentes.
* Se filtraron los datos para asegurar la consistencia, excluyendo eventos de períodos con información incompleta.
* Se realizó un análisis de la cantidad de eventos y usuarios, así como la distribución de los datos a lo largo del tiempo.

### 2. Análisis del Embudo de Eventos
* Se identificaron los eventos más frecuentes y se ordenaron para construir el embudo de ventas.
* Se calculó la cantidad de usuarios únicos para cada evento.
* Se determinaron las tasas de conversión entre cada etapa del embudo, desde el primer contacto hasta el pago.
* Se identificó la etapa con la mayor pérdida de usuarios, proporcionando un punto de enfoque para futuras mejoras de la UX.

### 3. Evaluación del Test A/A/B
* Se verificó la distribución de usuarios en los grupos de control (246 y 247) y el grupo de prueba (248).
* Se realizó un **test A/A** entre los grupos de control (246 vs. 247) para validar la integridad del experimento y asegurar que no existían diferencias significativas entre ellos antes de probar el cambio.
* Se compararon los resultados del grupo de prueba (248) con los grupos de control, tanto de forma individual como combinada.
* Se realizaron pruebas de hipótesis estadísticas (usando la prueba Z) para determinar si las diferencias en la tasa de conversión para cada evento eran significativas.
* Se ajustó el nivel de significancia para mitigar el riesgo de falsos positivos debido a las múltiples pruebas realizadas.

## Conclusiones Clave

* **Punto de Abandono:** La mayor pérdida de usuarios ocurre entre la visualización de la página principal y la adición de productos al carrito.
* **Tasa de Conversión:** Solo el X% de los usuarios que inician el embudo completan el pago.
* **Resultados del Test A/A/B:** El análisis demostró que no existe una diferencia estadísticamente significativa en el comportamiento de los usuarios entre el grupo de prueba y los grupos de control. Por lo tanto, el nuevo diseño de fuentes **no afectó negativamente la conversión** y puede ser implementado sin riesgo.

## Cómo Ejecutar el Proyecto
Para ejecutar este proyecto en tu entorno local, sigue estos pasos:

1.  Clona el repositorio: `git clone https://github.com/johjan-espinosa/analisis-basado-en-eventos.git`
2.  Instala las librerías necesarias: `pip install pandas numpy matplotlib seaborn scipy`
3.  Abre el notebook en Jupyter: `jupyter notebook`
4.  Selecciona y ejecuta el archivo `analisis basado en eventos.ipynb`.

---
**Desarrollado por:** Johjan Danilo Mendivelso Espinosa
**Perfil de LinkedIn:** https://www.linkedin.com/in/johjan-espinosa/
