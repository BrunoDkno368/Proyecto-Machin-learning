# Proyecto-Machin-learning
Predicción de Churn de Clientes — Machine Learning Básico
🧠 Proyecto: Predicción de Churn de Clientes — Machine Learning Básico
📋 Descripción general

Este proyecto tiene como objetivo desarrollar un modelo de Machine Learning supervisado capaz de predecir si un cliente dejará o no un servicio (churn).
El proyecto incluye todo el flujo de trabajo completo de un analista de datos:

ETL (Extracción, Transformación y Carga) del dataset.

EDA (Análisis Exploratorio de Datos) con visualizaciones y detección de patrones.

Modelado predictivo con técnicas de clasificación.

Evaluación de resultados y visualización de métricas.

Dashboard en Power BI con KPIs y visualizaciones ejecutivas.

📊 Dataset

Fuente: Kaggle - Telco Customer Churn Dataset

Registros: ~7.000 clientes

Columnas principales:

gender, SeniorCitizen, Partner, Dependents,

tenure, PhoneService, InternetService,

MonthlyCharges, TotalCharges, Churn

⚙️ Flujo del proyecto
🔹 1. ETL — Limpieza y preparación

Carga del dataset (.csv) usando pandas.

Revisión de valores nulos y duplicados.

Conversión de tipos de datos (TotalCharges → numérico).

Eliminación e imputación de valores faltantes con SimpleImputer.

Codificación de variables categóricas con get_dummies().

🔹 2. EDA — Análisis exploratorio

Estadísticas descriptivas (promedios, desviaciones, outliers).

Distribución de variables con matplotlib y seaborn.

Matriz de correlación numérica.

Análisis de churn por características clave: género, servicio de internet, tipo de contrato.

🔹 3. Modelado (Machine Learning)

División de los datos en X_train, X_test, y_train, y_test (70/30).

Entrenamiento con Regresión Logística (LogisticRegression).

Alternativa: modelos que aceptan NaN como HistGradientBoostingClassifier.

Normalización opcional de variables numéricas.

🔹 4. Evaluación del modelo

Precisión: accuracy_score(y_test, y_pred)

Reporte de métricas: classification_report()

Matriz de confusión con seaborn.heatmap()

Curva ROC y AUC (si corresponde).

Ejemplo de resultados:

Métrica	Valor
Accuracy	0.80
Precision	0.78
Recall	0.75
F1-score	0.76
📈 5. Dashboard en Power BI

Se creó un dashboard interactivo que complementa el análisis con:

Churn total y tasa de abandono.

Comparativa por tipo de contrato, servicio y género.

Segmentación dinámica (slicers) por antigüedad y método de pago.

Visualizaciones: barras, KPI cards, treemap, donut chart.

(Captura sugerida del dashboard)
📊 “Tasa de Churn por tipo de contrato y método de pago”

🧩 Tecnologías utilizadas
Categoría	Herramientas
Lenguaje principal	Python 3.12
Librerías	pandas, numpy, matplotlib, seaborn, scikit-learn
Visualización	Power BI
Entorno	Jupyter Notebook / Google Colab
Control de versiones	Git & GitHub

✨ Autor

👤 Bruno Roberto Argañaraz

📧 bruno.r.arganaraz@gmail.com

🔗 LinkedIn https://www.linkedin.com/in/bruno-argañaraz-726a4a199/

💻 GitHub https://github.com/BrunoDkno368
