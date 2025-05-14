# Time Series Forecasting with Deep Learning

## 🎯 Objetivo del Proyecto
Realizar un pronóstico de series de tiempo (temperaturas diarias) utilizando redes neuronales recurrentes (LSTM), evaluando el rendimiento mediante métricas de regresión.

## 📂 Descripción del Dataset
Se utiliza el dataset de temperaturas diarias de la ciudad de Melbourne, Australia. El conjunto de datos contiene registros históricos diarios de temperatura máxima, mínima, precipitación, etc.

## ⚖️ Decisiones Tomadas en el Modelado
- Se transformaron los datos en secuencias para predecir la temperatura del día siguiente.
- Se diseñó una red LSTM simple con una capa densa de salida para realizar la predicción.
- Se utilizó normalización de datos y división secuencial en conjuntos de entrenamiento y prueba.
- Registro y seguimiento de experimentos mediante MLflow.

## 📈 Resultados y Métricas Principales
- MSE: 2.01
- MAE: 1.12

## ⚙️ Instrucciones para Ejecutar el Proyecto

1. Clona este repositorio:
```bash
git clone https://github.com/tu_usuario/time_series_dl_regression_project.git
cd time_series_dl_regression_project
```

2. Instala las dependencias:
```bash
pip install -r requirements.txt
```

3. Ejecuta los notebooks en orden:
   - `1_EDA.ipynb`
   - `2_preprocessing.ipynb`
   - `3_train_validate_model.ipynb`
   - `4_evaluation_export.ipynb`

4. Opcional: iniciar MLflow
```bash
mlflow ui
```
Accede a `http://localhost:5000` en tu navegador.
