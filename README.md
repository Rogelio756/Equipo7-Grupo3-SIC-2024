# Predicción de Accidentes

## Descripción

Este proyecto tiene como objetivo analizar datos de accidentes y construir modelos de aprendizaje automático para predecir la cantidad de accidentes en función del tiempo (año y mes). 

## Datos

Los datos utilizados en este proyecto se encuentran en la carpeta `fixed_csv` y consisten en varios archivos CSV que contienen información sobre accidentes. 

## Metodología

1. **Carga y preparación de datos:** Se cargan y combinan los datos de los archivos CSV. Se crea una columna "time" que representa el tiempo en años y se agregan características adicionales "month_sin" y "month_cos" para capturar la periodicidad mensual.
2. **Análisis exploratorio:** Se realiza un análisis exploratorio de los datos para comprender la relación entre el tiempo y la cantidad de accidentes.
3. **Modelado:** Se entrenan cuatro modelos de regresión: Regresión lineal, Bosque aleatorio, XGBoost y Red neuronal (MLP Regressor).
4. **Evaluación del modelo:** Se evalúa el rendimiento de cada modelo utilizando métricas como MSE, MAE y R².
5. **Visualización de resultados:** Se visualizan las predicciones de cada modelo en comparación con los valores reales.

## Resultados

Los resultados del análisis y la evaluación del modelo se presentan en el notebook. Se puede observar el rendimiento de cada modelo y comparar sus predicciones.

## Conclusiones

Este proyecto demuestra la viabilidad de utilizar modelos de aprendizaje automático para predecir la cantidad de accidentes en función del tiempo. Los resultados obtenidos pueden ser útiles para la toma de decisiones en la prevención de accidentes.

## Instrucciones de uso

1. Descarga los archivos del proyecto.
2. Asegúrate de tener las bibliotecas necesarias instaladas (pandas, scikit-learn, xgboost, etc.).
