# Sistema Predictivo de Accidentes de Tránsito mediante IA

## Introducción

Este proyecto desarrolla un sistema predictivo de accidentes de tránsito integrando técnicas de aprendizaje automático. La seguridad vial es un desafío global con importantes implicaciones sociales.  El sistema aborda tres problemas fundamentales en IA: clasificación (predictor binario de accidentes), regresión (estimación de severidad de accidentes) y agrupamiento (identificación de patrones de riesgo).

## Metodología

### Datos y Preprocesamiento

Se utilizó un dataset de 15,000 registros con las siguientes variables:

* Características numéricas: Límite de velocidad, densidad vehicular. 
* Variables categóricas: Condiciones climáticas, tipo de vía. 
* Variables objetivo: Ocurrencia de accidente (binaria), severidad (numérica).

El flujo de preprocesamiento de datos se detalla en la Figura 1 del documento (flujo\_preprocessing.png).

### Arquitectura del Modelo

El sistema implementa tres enfoques principales:

1.  Clasificación: Random Forest y KNN para predicción binaria.
2.  Regresión: Modelo lineal para estimar severidad. 
3.  Agrupamiento: K-means para identificar patrones de riesgo. 

La arquitectura general del modelo se puede observar en la Figura 3 del documento (model\_architecture.png).

## Resultados

### Desempeño de los Modelos

Los resultados de clasificación se muestran en la siguiente tabla:

| Modelo        | Precisión (Test) | F1-Score |
| ------------- | ---------------- | -------- |
| Random Forest | 0.76             | 0.79     |
| KNN           | 0.73             | 0.72     |

Figura 2 en el documento (features\_importancia.png) muestra la importancia de las características para el modelo de Random Forest. 

### Análisis de Agrupamiento

Se identificaron tres clusters principales:

* Cluster 1: Accidentes nocturnos en condiciones lluviosas.
* Cluster 2: Colisiones múltiples en horas pico. 
* Cluster 3: Incidentes leves en zonas escolares.

## Discusión y Conclusiones

El modelo demostró una efectividad del F1 = 0.79 identificando situaciones de riesgo. La integración de múltiples técnicas permite:

* Predecir probabilidad de accidentes (clasificación). 
* Estimar severidad potencial (regresión). 
* Identificar patrones de riesgo (clustering). 

Los principales retos identificados son el desbalance en las clases de severidad y la variabilidad en las condiciones climáticas.

## Implementación Técnica

El código del proyecto está disponible en [https://github.com/amg-abdiel](https://github.com/amg-abdiel) e incluye:

* Jupyter Notebook completo.
* Conjunto de datos procesado. 
* Modelos pre-entrenados. 

## Referencias

1.  Almanza, M. et al. (2021). Traffic Accident Prediction Using Machine Learning. IEEE Transactions on ITS.
2.  Chen, L. (2022). Ensemble Methods for Road Safety Analytics. Journal of Transportation Engineering.
3.  Kumar, P. (2020). Spatial-Temporal Patterns in Traffic Data. Accident Analysis & Prevention.
