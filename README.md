# Dominio-Grupo-4-Finanzas

Analisis de la Dinamica de Precios del indice NASDAQ-100 (Octubre 2019 - Octubre 2024)

## Descripcion Del Proyecto
Este proyecto aplica metodos numericos para analizar, modelar y entender el comportamiento y la volatilidad del indice financiero NASDAQ-100 durante un periodo de 5 a;os. A traves del modelado matematico, se busca identificar tendencias a largo plazo, suavizar el ruido del mercado diario y determinar numericamente los puntos de inflexion criticos provocados por eventos macroeconomicos.


## Metodos Numericos Propuestos
Para el análisis de los activos, se implementarán los siguientes enfoques numéricos en Python:
1. **Regresion por Minimos Cuadrados:** Para modelar la tendencia general de los precios a largo plazo y reducir el ruido diario del mercado.
2. **Interpolación por Splines Cúbicos:** Para realizar un análisis detallado y curvas suavizadas en subperiodos de alta volatilidad (por ejemplo, la caída por COVID-19 en 2020).
3. **Métodos de Búsqueda de Raíces (Newton-Raphson):** Aplicado a la derivada de las funciones de tendencia obtenidas, con el fin de hallar numéricamente las fechas exactas de los máximos y mínimos locales (techos y suelos de mercado).


## Prerrequisitos y Tecnologías
Para ejecutar este proyecto adecuadamente, se requiere el siguiente entorno:
* **Lenguaje:** Python 3.x
* **Entorno:** Jupyter Notebook, VSCode o Google Colab
* **Librerías principales:** 
  * `numpy` (operaciones matriciales y vectorización matemática)
  * `pandas` (importación, manejo y limpieza del dataset)
  * `matplotlib` (renderizado de gráficos y visualización de resultados)
  * `scipy` (implementación del algoritmo de splines cúbicos)


## Estructura del Proyecto
El desarrollo numérico y algorítmico está dividido en las siguientes fases secuenciales dentro del cuaderno:
* **Fase 1: Preprocesamiento y Linealización Temporal:** Carga de los datos bursátiles, estandarización de decimales y conversión de las fechas calendario a una variable independiente numérica (tiempo continuo).
* **Fase 2: División del Dataset (Train/Test):** Segmentación de los datos históricos en subconjuntos de entrenamiento (80%) y prueba (20%) para validar el modelo y evitar el sobreajuste temporal.
* **Fase 3: Interpolación y Suavizado:** Aplicación de Splines Cúbicos Naturales para mitigar la volatilidad diaria y construir una curva fluida de los precios de cierre.
* **Fase 4: Determinación de Tendencia y Búsqueda de Raíces:** Construcción de la regresión polinomial optimizada (evitando el overfitting) y ejecución del método iterativo de Newton-Raphson para el cálculo exacto de puntos de cruce sobre la tendencia.
* **Fase 5: Visualización de Proyecciones:** Generación de gráficas comparativas y renderizado final del modelo sobre el segmento de prueba para evaluar la predicción.

## Uso y Ejecución
1. Clona este repositorio en tu entorno local.
2. Asegúrate de tener instaladas las dependencias necesarias ejecutando: `pip install numpy pandas matplotlib scipy`.
3. Abre el archivo principal `.ipynb` en tu entorno de desarrollo preferido.
4. Asegúrate de que el dataset original (`.csv`) se encuentre en la misma ruta o ajusta el path de lectura en la primera celda.
5. Ejecuta las celdas de manera secuencial desde la importación de librerías hasta la etapa de visualización.
