# Sistema Predictivo de Accidentes de Tránsito mediante IA

## Objetivo del Proyecto

Aplicar los conocimientos y habilidades adquiridos en el curso SIC para desarrollar un modelo predictivo de inteligencia artificial (IA), implementando algoritmos de Machine Learning como **Random Forest** y **KNN** para estimar la probabilidad de que en un accidente de tránsito haya personas heridas, a partir de datos históricos. Esto con el objetivo de mejorar la precisión en la identificación de patrones y factores de riesgo.

---

## Enlace al Repositorio de GitHub

[**https://github.com/Rogelio756/Equipo7-Grupo3-SIC-2024**](https://github.com/Rogelio756/Equipo7-Grupo3-SIC-2024)

---

## Instrucciones de Instalación y Uso



### 1. Requisitos Previos

Asegúrate de tener instalado lo siguiente:

- **Python 3.x**  
  [https://www.python.org/downloads/](https://www.python.org/downloads/)
- **pip** (gestor de paquetes de Python)
- **Git**  
  [https://git-scm.com/downloads](https://git-scm.com/downloads)

### 2. Clonar el Repositorio

Abre una terminal y ejecuta:

```bash
git clone https://github.com/Rogelio756/Equipo7-Grupo3-SIC-2024
cd Equipo7-Grupo3-SIC-2024
```

### 3. Crear un Entorno Virtual (Recomendado)

```bash
# En Windows
python -m venv venv
venv\Scripts\activate

# En macOS/Linux
python3 -m venv venv
source venv/bin/activate
```

### 4. Instalar las Dependencias

```bash
pip install numpy pandas seaborn matplotlib scikit-learn
```

Estas bibliotecas son necesarias para el análisis de datos, visualización y modelado de machine learning.

### 5. Obtener el Dataset

El proyecto espera un archivo llamado `traffic_accidents.csv` en el mismo directorio del script. Puedes descargarlo desde el siguiente enlace:

[https://www.kaggle.com/code/oktayrdeki/crash-type-prediction-eda-ml?select=traffic_accidents.csv](https://www.kaggle.com/code/oktayrdeki/crash-type-prediction-eda-ml?select=traffic_accidents.csv)

> **Nota:** Es posible que necesites una cuenta de Kaggle para acceder a la descarga.

### 6. Ejecutar el Código

#### Opción 1: Usando Jupyter Notebook

Instala Jupyter si no lo tienes:

```bash
pip install notebook
```

Ejecuta:

```bash
jupyter notebook
```

Esto abrirá el navegador. Carga el archivo `.ipynb` y ejecútalo celda por celda.

#### Opción 2: Convertir a Script de Python

Guarda el contenido del notebook en un archivo `main.py`, y luego ejecuta:

```bash
python main.py
```

Este script realiza:

- Carga y análisis del dataset
- Análisis descriptivo
- Preprocesamiento (codificación, normalización, limpieza)
- Entrenamiento de modelos (Random Forest, Decision Tree, KNN, MLP, SVC)
- Optimización con `GridSearchCV`
- Métricas de evaluación de modelos
- Agrupamiento con KMeans
- Visualización y evaluación de clusters

### 7. Interpretación de los Resultados

Después de la ejecución:

- Verás métricas como: `accuracy`, `classification_report`, `confusion_matrix`
- Resultados del agrupamiento con: `Silhouette Score`, `Calinski-Harabasz Score`, `Davies-Bouldin Score`
- Visualizaciones de los clusters detectados por KMeans

# Tecnologías Utilizadas

- **Python**: Lenguaje de programación principal.  
- **Pandas**: Para la manipulación y análisis de datos.  
- **NumPy**: Para operaciones numéricas.  
- **Seaborn**: Para la visualización de datos estadísticos.  
- **Matplotlib**: Para la creación de gráficos y visualizaciones.  
- **Scikit-learn (sklearn)**: Biblioteca de machine learning que incluye:
  - `preprocessing`: Para la codificación de etiquetas y la normalización de datos.
  - `tree`: Para el modelo de árbol de decisión.
  - `linear_model`: Para el modelo de regresión logística.
  - `neighbors`: Para el modelo KNN.
  - `model_selection`: Para la división de datos y la búsqueda de cuadrícula (`GridSearchCV`).
  - `ensemble`: Para el modelo de Random Forest.
  - `metrics`: Para la evaluación del rendimiento del modelo (`accuracy`, `classification_report`, `confusion_matrix`, `silhouette_score`, `calinski_harabasz_score`, `davies_bouldin_score`).
  - `neural_network`: Para el modelo de perceptrón multicapa (MLP).
  - `svm`: Para el modelo de máquina de vectores de soporte (SVC).
  - `cluster`: Para algoritmos de agrupamiento (`KMeans`, `DBSCAN`, `AgglomerativeClustering`).
  - `decomposition`: Para la reducción de dimensionalidad (`PCA`).
- **SciPy**: Para funciones de clustering jerárquico (`scipy.cluster.hierarchy`).

---

# Créditos o Autores

- **García Pérez Dariana Mildred**  
- **Maldonado González César Abdiel**  
- **Valerio Carera Ricardo**  
  *IPN*  
- **Méndez Macías Rogelio Leonardo**  
  *UAM Azcapotzalco*

