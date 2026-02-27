# 🚀 Predicción de Churn - Telecom X

¡Misión cumplida! 🎉 Tras mi promoción al equipo de **Machine Learning**, he desarrollado este pipeline predictivo para anticipar la cancelación de clientes y transformar datos en decisiones estratégicas.

## 🎯 Misión del Proyecto
Desarrollar modelos capaces de prever qué clientes tienen mayor probabilidad de cancelar sus servicios, permitiendo a Telecom X actuar de forma proactiva antes de perder al usuario.

## 🧠 Metodología y Modelado
Se evaluaron diversos algoritmos para encontrar el equilibrio perfecto entre detección y precisión:
* **Modelos probados**: Regresión Logística y Random Forest.
* **Desafío técnico**: Los datos presentaban un fuerte desbalance: 1,035 casos 'No' vs. 374 'Yes'.
* **Solución estratégica**: Se seleccionó la **Regresión Logística Balanceada** (`class_weight="balanced"`).

## 📊 ¿Por qué este modelo?
Aunque los modelos tradicionales tenían un mayor *accuracy* general, fallaban en la misión principal: detectar el Churn.

| Métrica para clase "Yes" | Regresión Logística (Normal) | Regresión Logística (Balanceada) |
| :--- | :---: | :---: |
| **Recall (Detección)** | 0.52 | **0.79** |
| **F1-Score** | 0.58 | **0.62** |
| **Accuracy General** | 0.80 | 0.74 |

> **Decisión Ejecutiva**: Para Telecom X, es preferible identificar a un cliente que podría irse (aunque no lo haga) que perder a uno por no haberlo detectado a tiempo. El modelo balanceado aumentó nuestra capacidad de detección en un **27%**.

## 📈 Análisis de Resultados
La **Matriz de Confusión** final respalda esta decisión estratégica:

* **Verdaderos Positivos (294)**: Clientes en riesgo detectados con éxito.
* **Falsos Negativos (80)**: Casos de fuga que el modelo no detectó; reducidos drásticamente gracias al balanceo.
* **Verdaderos Negativos (753)**: Clientes leales correctamente identificados.



## 🧰 Herramientas Utilizadas
* **Python**: Procesamiento y limpieza de datos.
* **Scikit-learn**: Entrenamiento y evaluación de modelos (`LogisticRegression`, `RandomForestClassifier`, `classification_report`).
* **Matplotlib/Seaborn**: Visualización de métricas y análisis de matriz de confusión.

---
**Analista Junior de Machine Learning** *Telecom X confía en esta entrega para dar los próximos pasos hacia una solución de inteligencia predictiva eficaz.*
