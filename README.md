# Dominio-Grupo-4-Finanzas

Analisis de la Dinamica de Precios del indice NASDAQ-100 (Octubre 2019 - Octubre 2024)

## Descripcion Del Proyecto
Este proyecto aplica metodos numericos para analizar, modelar y entender el comportamiento y la volatilidad del indice financiero NASDAQ-100 durante un periodo de 5 a;os. A traves del modelado matematico, se busca identificar tendencias a largo plazo, suavizar el ruido del mercado diario y determinar numericamente los puntos de inflexion criticos provocados por eventos macroeconomicos.


## Metodos Numericos Propuestos
Para el análisis de los activos, se implementarán los siguientes enfoques numéricos en Python:
1. **Regresion por Minimos Cuadrados:**Para modelar la tendencia general de los precios a largo plazo y reducir el ruido diario del mercado.
2. **Interpolación por Splines Cúbicos:** Para realizar un análisis detallado y curvas suavizadas en subperiodos de alta volatilidad (por ejemplo, la caída por COVID-19 en 2020).
3. **Métodos de Búsqueda de Raíces (Newton-Raphson):** Aplicado a la derivada de las funciones de tendencia obtenidas, con el fin de hallar numéricamente las fechas exactas de los máximos y mínimos locales (techos y suelos de mercado).


