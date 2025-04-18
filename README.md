
# 🫀 Predicción de Enfermedad Cardíaca con Machine Learning

Este proyecto implementa un modelo de clasificación binaria utilizando técnicas de Machine Learning para predecir el riesgo de enfermedad cardíaca en pacientes, basado en variables clínicas.

---

## 📁 Contenido del Repositorio

- `heart_disease_uci.csv`: Dataset original utilizado (UCI Heart Disease)
- `ProyectoClasificacionHeartDisease.ipynb`: Notebook con todo el desarrollo del modelo
- `Presentacion_HeartDisease_MarcoAdrian_TECH.pptx`: Presentación profesional en PowerPoint con enfoque técnico
- `README.md`: Documentación del proyecto
- `requirements.txt`: Librerías necesarias para ejecutar el proyecto

---

## 🎯 Objetivo

Construir un modelo predictivo que clasifique si un paciente tiene o no riesgo de enfermedad cardíaca, utilizando variables clínicas como edad, colesterol, presión arterial, resultados de ECG, entre otros.

---

## 🧠 Modelo Utilizado

- **Algoritmo**: Random Forest Classifier
- **Predicción**: Binaria (Sano / Enfermo)
- **Balanceo de clases**: `class_weight='balanced'`
- **Feature Engineering**: Nuevas variables como `chol_log`, `chol_per_age`, `stress_risk_score`, entre otras.

---

## ⚙️ Flujo del Proyecto

1. Exploración inicial del dataset (EDA)
2. Tratamiento de nulos y outliers
3. Codificación de variables categóricas
4. Escalado y transformaciones (logarítmica)
5. Ingeniería de características
6. Entrenamiento y evaluación del modelo
7. Simulación de pacientes con datos aleatorios

---

## 📊 Evaluación del Modelo

El modelo mostró un excelente rendimiento, especialmente en la detección de pacientes en riesgo (recall alto):

- **Accuracy**: 82%
- **Precision (enfermo)**: 87%
- **Recall (enfermo)**: 82%
- **F1-score**: 84%
- **AUC-ROC**: 0.92

---

## 📈 Visualizaciones Incluidas

- Matriz de Confusión
- Curva ROC
- Importancia de características
- Scatter plots
- Simulación de pacientes nuevos

---

## 🧪 Predicción con Datos Simulados

Se generaron registros aleatorios con distribuciones similares al dataset original para simular pacientes nuevos.  
El modelo demostró ser capaz de generalizar y predecir el riesgo de forma confiable utilizando `predict_proba()`.

---

## 🖥️ Presentación Técnica

📎 Archivo: `Presentacion_HeartDisease_MarcoAdrian_TECH.pptx`

La presentación contiene:

- Introducción y objetivos del proyecto
- Visualizaciones del análisis exploratorio (EDA)
- Detalles del preprocesamiento aplicado
- Métricas clave de evaluación
- Aplicación del modelo en pacientes simulados
- Conclusiones técnicas y sugerencias de mejora futura

> 👉 Está diseñada para comunicar los resultados de forma clara, visual y profesional en un entorno académico o clínico.

---

## 🚀 Requisitos

- Python 3.8+
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- plotly *(opcional para visualizaciones interactivas)*

Instalar dependencias con:

```bash
pip install -r requirements.txt
```

---

## 📌 Conclusión

El modelo Random Forest implementado demostró ser robusto, preciso y clínicamente relevante.  
Destacó por su capacidad de detección, simplicidad y aplicabilidad como herramienta de apoyo en decisiones médicas.

✅ Variables clave: `oldpeak`, `cp`, `thal`, `ca`

🚀 Futuras mejoras:
- Validación cruzada
- Tuning con GridSearchCV
- Comparación con modelos avanzados como XGBoost

---

## 🧾 Autor

**Marco Adrian**  
Proyecto académico de Machine Learning – Abril 2025
