# Sistema Predictivo de Accidentes de Tránsito mediante IA

## Introducción

Este proyecto desarrolla un sistema predictivo de accidentes de tránsito integrando técnicas de aprendizaje automático. La seguridad vial es un desafío global con importantes implicaciones sociales. [cite: 1, 2] El sistema aborda tres problemas fundamentales en IA: clasificación (predictor binario de accidentes), regresión (estimación de severidad de accidentes) y agrupamiento (identificación de patrones de riesgo). [cite: 2]

## Metodología

### Datos y Preprocesamiento

Se utilizó un dataset de 15,000 registros con las siguientes variables:

* Características numéricas: Límite de velocidad, densidad vehicular. [cite: 5, 6]
* Variables categóricas: Condiciones climáticas, tipo de vía. [cite: 5, 6]
* Variables objetivo: Ocurrencia de accidente (binaria), severidad (numérica). [cite: 6]

El flujo de preprocesamiento de datos se detalla en la Figura 1 del documento (flujo\_preprocessing.png). [cite: 6, 7]

### Arquitectura del Modelo

El sistema implementa tres enfoques principales:

1.  Clasificación: Random Forest y KNN para predicción binaria. [cite: 7, 8]
2.  Regresión: Modelo lineal para estimar severidad. [cite: 8]
3.  Agrupamiento: K-means para identificar patrones de riesgo. [cite: 8]

La arquitectura general del modelo se puede observar en la Figura 3 del documento (model\_architecture.png). [cite: 16]

## Resultados

### Desempeño de los Modelos

Los resultados de clasificación se muestran en la siguiente tabla:

| Modelo        | Precisión (Test) | F1-Score |
| ------------- | ---------------- | -------- |
| Random Forest | 0.76             | 0.79     |
| KNN           | 0.73             | 0.72     |

Figura 2 en el documento (features\_importancia.png) muestra la importancia de las características para el modelo de Random Forest. [cite: 10, 11]

### Análisis de Agrupamiento

Se identificaron tres clusters principales:

* Cluster 1: Accidentes nocturnos en condiciones lluviosas. [cite: 12]
* Cluster 2: Colisiones múltiples en horas pico. [cite: 12]
* Cluster 3: Incidentes leves en zonas escolares. [cite: 12]

## Discusión y Conclusiones

El modelo demostró una efectividad del F1 = 0.79 identificando situaciones de riesgo. [cite: 13] La integración de múltiples técnicas permite:

* Predecir probabilidad de accidentes (clasificación). [cite: 13]
* Estimar severidad potencial (regresión). [cite: 13]
* Identificar patrones de riesgo (clustering). [cite: 13]

Los principales retos identificados son el desbalance en las clases de severidad y la variabilidad en las condiciones climáticas. [cite: 13]

## Implementación Técnica

El código del proyecto está disponible en [https://github.com/amg-abdiel](https://github.com/amg-abdiel) e incluye: [cite: 16]

* Jupyter Notebook completo. [cite: 16]
* Conjunto de datos procesado. [cite: 16]
* Modelos pre-entrenados. [cite: 16]

## Referencias

1.  Almanza, M. et al. (2021). Traffic Accident Prediction Using Machine Learning. IEEE Transactions on ITS. [cite: 14]
2.  Chen, L. (2022). Ensemble Methods for Road Safety Analytics. Journal of Transportation Engineering. [cite: 14, 15]
3.  Kumar, P. (2020). Spatial-Temporal Patterns in Traffic Data. Accident Analysis & Prevention. [cite: 15]
