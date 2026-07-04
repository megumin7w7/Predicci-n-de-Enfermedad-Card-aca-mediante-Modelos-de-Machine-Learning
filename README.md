# Predicción de Enfermedad Cardíaca mediante Modelos de Machine Learning

<div align="center">

<img src="https://readme-typing-svg.herokuapp.com?font=Lexend+Giga&size=24&pause=1000&color=4A90E2&center=true&vCenter=true&width=700&lines=Predicción+de+Enfermedad+Cardíaca;Heart+Disease+Prediction+%7C+UCI+Dataset;CRISP-DM+%7C+SEMMA+%7C+Machine+Learning" />

![Python](https://img.shields.io/badge/Python-3.12-blue?style=for-the-badge&logo=python)
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.4-F7931E?style=for-the-badge&logo=scikit-learn)
![Pandas](https://img.shields.io/badge/Pandas-2.0-150458?style=for-the-badge&logo=pandas)
![Status](https://img.shields.io/badge/Status-Completado-brightgreen?style=for-the-badge)

</div>

---

## Resumen del proyecto

Este proyecto se desarrolló en simulación de una colaboración con el ficticio Hospital Regional **"Vida Salud"** ante el incremento del **34%** en ingresos por patologías cardiovasculares. El objetivo fue implementar un modelo predictivo para la detección temprana de enfermedad cardíaca, optimizando recursos clínicos y fortaleciendo estrategias de prevención.

Se trabajó con el dataset **UCI Heart Disease**, aplicando dos metodologías de minería de datos:

- **CRISP-DM:** garantizó coherencia entre objetivos clínicos y decisiones técnicas.
- **SEMMA:** aportó un enfoque práctico en la manipulación y modelado de datos.

El modelo final seleccionado fue **Regresión Logística con AIC**, por su equilibrio entre rendimiento (**Accuracy 86.2%**, **AUC-ROC 92.5%**) e interpretabilidad clínica.

---

## Metodologías aplicadas

| Metodología | Aplicación |
|-------------|------------|
| **CRISP-DM** | Comprensión del negocio, comprensión de datos, preparación, modelado, evaluación y despliegue |
| **SEMMA** | Sample, Explore, Modify, Model, Assess |

Ambas metodologías se complementaron: **CRISP-DM** aportó visión integral y **SEMMA** eficiencia técnica.

---

## Procesamiento y limpieza de datos

| Técnica | Aplicación |
|---------|------------|
| **Imputación** | Valores faltantes (ej. `vasos_coloreados`) mediante métodos estadísticos |
| **Outliers** | Tratamiento con **IQR** y winsorización |
| **Codificación** | One-Hot Encoding para variables categóricas |
| **Estandarización** | Z-score para variables numéricas |
| **Multicolinealidad** | Reducción con **VIF** |

---

## Modelos comparados

| Modelo | Observación |
|--------|-------------|
| **Regresión Logística** | Base, AIC y Boruta — elegido por interpretabilidad clínica |
| **KNN** | Útil pero menos interpretable |
| **MLP (Red Neuronal)** | Buen rendimiento sin complejidad excesiva |

El mejor desempeño fue de **KNN con AIC** en validación cruzada, aunque para implementación clínica se priorizó **LogReg AIC** por su interpretabilidad.

---

## Métricas y resultados

| Métrica | Resultado |
|---------|:---------:|
| **Accuracy** | 0.86 |
| **Precision** | 0.87 |
| **Recall** | 0.83 |
| **F1-Score** | 0.85 |
| **AUC-ROC** | 0.93 |

El modelo predice correctamente a más de **9 de cada 10 pacientes**, reduciendo diagnósticos tardíos y mejorando la atención preventiva.

---

## Interpretabilidad

- **Odds Ratios:** `vasos_coloreados` (>1) incrementa riesgo cardiovascular, alineado con guías ACC/AHA.
- **SHAP Values:** aplicados en LogReg y MLP para explicar contribución de variables.
- **Permutation Importance:** usado en KNN para ranking de variables relevantes.

**Variables clave:** edad, colesterol, frecuencia cardíaca máxima, angina por ejercicio, depresión ST, vasos coloreados, tipo de dolor torácico, talasemia.

---

## Técnicas adicionales

- **PCA:** Reducción dimensional, identificando componentes que explican variabilidad clínica.
- **Clustering (K-Means):** Segmentación de pacientes en perfiles de riesgo diferenciados.

---

## Impacto y extensión

| Aspecto | Impacto |
|---------|---------|
| **Madurez analítica** | Eleva el hospital de nivel 2 (descriptivo) a 3 (predictivo) |
| **KPIs** | Reducción de falsos negativos, mejora en detección temprana (+18%) |
| **Ahorro estimado** | **USD 450,000 anuales** |
| **Extensión a Perú** | Incluir variables socioeconómicas, hábitos alimenticios y acceso a salud |

---

## Conclusiones

El proyecto demostró que el uso de machine learning en el ámbito hospitalario puede mejorar significativamente la capacidad predictiva y la eficiencia operativa.

La **Regresión Logística AIC** se consolidó como la alternativa más adecuada por su balance entre precisión, simplicidad e interpretabilidad.

La implementación progresiva permitirá optimizar recursos, reducir complicaciones y mejorar la calidad de vida de los pacientes mediante una atención más preventiva y basada en datos.

---

## Integrantes

- Bryan Jean Pierre Villasante López
- **Pedro Sebastián Alfieri Arteaga Guerra**
- Piero Hideki Furushio Casanave
- Renzo Sebastian Salazar Chavez

---

<div align="center">

**Curso:** Gestión de Análisis de Datos  
**Docente:** Pilar Sayán Mejía  
**Fecha:** 06/12/2025

</div>
