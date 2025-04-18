# 🫀 Predicción de Enfermedad Cardíaca con Machine Learning

Este proyecto implementa un modelo de clasificación binaria utilizando técnicas de Machine Learning para predecir el riesgo de enfermedad cardíaca en pacientes, basado en variables clínicas.

---

## 📁 Contenido

- `heart_disease_uci.csv`: Dataset utilizado
- `ProyectoClasificacionHeartDisease.ipynb`: Notebook con todo el desarrollo del modelo
- `README.md`: Documentación del proyecto
- `requirements.text`: librerias a instalar

---

## 🎯 Objetivo

El objetivo principal es construir un modelo de clasificación que permita **predecir si un paciente tiene riesgo de enfermedad cardíaca** utilizando variables clínicas como edad, presión arterial, colesterol, resultados de ECG, entre otras.

---

## 🧠 Modelo Utilizado

- **Balanceo de clases**: Se utilizó `class_weight='balanced'` para mejorar el rendimiento frente a clases desbalanceadas.
- **Feature Engineering aplicado**: Se crearon nuevas variables como `chol_log`, `chol_per_age` y `stress_risk_score` para mejorar la representación de los datos clínicos.
- **Algoritmo**: Random Forest Classifier
- **Tipo de predicción**: Binaria (Enfermo / Sano)


---

## ⚙️ Flujo del Proyecto

1. **Carga y limpieza de datos**
2. **Tratamiento de outliers**
3. **Imputación de valores faltantes**
4. **Codificación de variables categóricas**
5. **Transformaciones (log, escalado)**
6. **Feature Engineering**
7. **Entrenamiento del modelo**
8. **Evaluación con métricas y visualizaciones**
9. **Predicción sobre pacientes simulados**

---

## 📊 Evaluación del Modelo

El modelo mostró un excelente rendimiento, especialmente en la detección de pacientes con riesgo (recall = 0.82), lo cual es clave en contextos clínicos.

**Métricas destacadas:**
- Accuracy: 82%
- Precision (enfermo): 87%
- Recall (enfermo): 82%
- F1-score: 84%
- AUC-ROC: 0.92

---

## 📈 Visualizaciones

- Matriz de Confusión
- Curva ROC
- Importancia de características
- Scatter plots y análisis exploratorio

---

## 🧪 Predicción en nuevos pacientes

Se generaron **valores simulados** de pacientes para probar el modelo. El modelo predice correctamente el riesgo de enfermedad con alta confianza.

---

## 🚀 Requisitos

- Python 3.8+
- scikit-learn
- pandas
- seaborn
- matplotlib
- numpy

Instalar dependencias:

```bash
pip install -r requirements.txt

## 📌 Conclusión

El modelo Random Forest implementado demuestra un rendimiento sólido para predecir el riesgo de enfermedad cardíaca. Las variables `oldpeak`, `cp`, `thal` y `ca` fueron las más influyentes en la predicción.

Este sistema puede servir como herramienta complementaria en sistemas de salud preventivos. Futuras mejoras podrían incluir validación cruzada, tuning de hiperparámetros (GridSearchCV), y evaluación con modelos avanzados como XGBoost.

---

## 🧾 Autor

**Marco Adrian**  
*Proyecto académico de Machine Learning – Abril 2025*
