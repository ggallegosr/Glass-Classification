# Glass Dataset Classification – EDA & Machine Learning

Este proyecto aborda la tarea de clasificación utilizando múltiples algoritmos de aprendizaje supervisado sobre el dataset "Glass". Se implementan y comparan diversas técnicas de preprocesamiento y clasificación con el fin de analizar cómo afectan al rendimiento del modelo y a su vez evidenciar la importancia del preprocesamiento y análisis del conjunto de datos para obtener modelos óptimos para la clasificación.

##  Técnicas Utilizadas

### 📊 Preprocesamiento de Datos

- **Normalización**: Se normalizan las características numéricas para mejorar el rendimiento de ciertos clasificadores sensibles a la escala.
- **Oversampling con SMOTE (Synthetic Minority Oversampling Technique)**: Se aplica para equilibrar las clases del dataset, especialmente útil al trabajar con datos desbalanceados.
- **Conjunto de datos sin procesar**: También se evalúan modelos sin ningún preprocesamiento, como referencia comparativa.

### 🤖 Algoritmos de Clasificación (Supervisados)

- **Árbol de decisión simple**
- **Random Forest**
- **Red neuronal (MLPClassifier de Scikit-Learn)**
- **XGBoost – Random Forest (RandomForestClassifier como base estimator de XGBClassifier)**
- **XGBoost – Classifier**
- **K-Nearest Neighbors (KNN)**
- **CatBoost**

Cada clasificador fue evaluado en tres escenarios distintos:
1. Con datos crudos
2. Con datos normalizados
3. Con datos normalizados y balanceados mediante oversampling (SMOTE)

### 📈 Evaluación de Modelos

Se utilizó la matriz de confusión para evaluar los modelos y en el repositorio también se encuentra un documento donde se realiza el informe de cada etapa junto con las observaciones y conclusiones de la experimentación con cada modelo.

---

## 📂 Descarga del Dataset

El conjunto de datos utilizado en este proyecto se puede descargar desde Kaggle en el siguiente enlace:

🔗 [Glass Identification Dataset - Kaggle](https://www.kaggle.com/datasets/uciml/glass/data)

Para utilizar el dataset en tu entorno local, puedes descargarlo directamente desde la página, o utilizar la API de Kaggle ejecutando:

```bash
kaggle datasets download -d uciml/glass
