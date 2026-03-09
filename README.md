# Challenge-Alura-Telecom-X-parte-2

📊 Predicción de Cancelación de Clientes (Churn Prediction)
📌 Descripción del Proyecto

Este proyecto tiene como objetivo analizar los factores que influyen en la cancelación de clientes (churn) y desarrollar modelos de Machine Learning capaces de predecir si un cliente abandonará el servicio.

A través de un proceso completo de análisis exploratorio de datos (EDA), preprocesamiento, entrenamiento de modelos y evaluación, se identifican patrones relevantes en el comportamiento de los clientes.

Este tipo de análisis es fundamental para que las empresas puedan anticipar la pérdida de clientes y aplicar estrategias de retención más efectivas.

🧠 Objetivos

Analizar los factores asociados con la cancelación de clientes.

Explorar relaciones entre variables mediante visualización de datos.

Preparar los datos para modelos de Machine Learning.

Implementar modelos de clasificación para predecir churn.

Evaluar el desempeño de los modelos mediante métricas de clasificación.

🔎 Análisis Exploratorio de Datos (EDA)

Durante el análisis inicial se realizaron las siguientes tareas:

Limpieza y preparación del dataset

Conversión de variables categóricas a formato numérico

Identificación de variables irrelevantes

Análisis de correlación entre variables

Visualización de patrones mediante gráficos

Hallazgos principales

Existe un desbalance en la variable Churn, con aproximadamente:

73% clientes activos

27% clientes que cancelaron

Variables con mayor relación con churn:

InternetService_Fiber optic

PaymentMethod_Electronic check

Charges.Monthly

Charges.Daily

PaperlessBilling

SeniorCitizen

Los análisis sugieren que los costos del servicio y ciertos métodos de pago están asociados con una mayor probabilidad de cancelación.

⚙️ Preparación de Datos

Para entrenar los modelos se realizaron los siguientes pasos:

Separación de variables predictoras y variable objetivo (Churn)

División del dataset en:

Conjunto de entrenamiento

Conjunto de prueba

Normalización de variables mediante StandardScaler

La normalización es importante para modelos que dependen de distancias, como KNN y SVM.

🤖 Modelos Implementados

Se entrenaron dos modelos de clasificación:

Support Vector Machine (SVM)

Este modelo construye una frontera de decisión óptima que separa las clases maximizando el margen entre ellas.

K-Nearest Neighbors (KNN)

Este algoritmo clasifica un cliente según la proximidad con los vecinos más cercanos en el espacio de características.

📈 Evaluación de Modelos

Los modelos fueron evaluados utilizando las siguientes métricas:

Accuracy

Precision

Recall

F1-score

Matriz de confusión

Resultados
Modelo	Accuracy	Precision	Recall	F1-score
SVM	0.80	0.66	0.53	0.59
KNN	0.76	0.54	0.54	0.54

El modelo SVM obtuvo el mejor desempeño general, especialmente en accuracy y F1-score, mostrando un mejor equilibrio entre precisión y detección de churn.

📊 Interpretación de Variables

KNN: las variables influyen según su contribución a la distancia entre clientes.

SVM: las variables influyen en la posición de la frontera de decisión entre clases.

Entre los factores más influyentes se encuentran:

Tipo de servicio de internet

Método de pago

Cargos del servicio

Facturación electrónica

💻 Tecnologías Utilizadas

Python

Pandas

NumPy

Matplotlib

Seaborn

Scikit-learn

Jupyter Notebook

📌 Conclusión

El análisis permitió identificar factores importantes asociados con la cancelación de clientes. Los modelos de Machine Learning demostraron ser herramientas útiles para predecir el churn y detectar patrones en el comportamiento de los clientes, lo cual puede ayudar a las empresas a desarrollar estrategias de retención más efectivas.
