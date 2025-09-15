# Machine-Learning-Competicion-Pump-it-Up
Predicción del estado de bombas de agua 🚰

Este proyecto aplica técnicas de Machine Learning para predecir el estado de funcionamiento de bombas de agua en Tanzania. El objetivo es clasificar cada bomba como:

Funcionando

Funcionando pero necesita reparación

Estropeada

Contenido del repositorio

notebooks/ → desarrollo del EDA, feature engineering y entrenamiento.

transformar_x_test.py → función espejo para transformar el test con los mismos artefactos que en train.

artefactos/ → medianas, top categorías, label encoders, modelos serializados con joblib.

submission.csv → predicciones finales para Kaggle.

Metodología

EDA (Exploratory Data Analysis) → análisis descriptivo de variables, detección de nulos, outliers y patrones.

Feature Engineering

Imputación de variables numéricas con medianas por región y globales.

Creación de variables binarias y log-transformaciones.

Agrupación de categorías poco frecuentes.

Codificación LabelEncoder y One-Hot.

Clustering geográfico con KMeans (15 clusters).

Modelado

Modelos base: RandomForest, Gradient Boosting.

Ajuste de hiperparámetros.

Evaluación con precisión, recall y F1-score.

Predicción y envío

Transformación del test con los mismos artefactos.

Generación del archivo de submission
