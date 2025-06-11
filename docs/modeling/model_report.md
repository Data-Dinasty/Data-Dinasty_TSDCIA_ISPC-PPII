# Reporte del Modelo Final

## Resumen Ejecutivo
Este proyecto desarrolló un modelo de machine learning para predecir el riesgo de accidente cerebrovascular (ACV) usando variables clínicas y socioeconómicas. Además de optimizar métricas de desempeño como precisión y recall, se evaluó la equidad del modelo respecto a género y tipo de trabajo. El modelo final logró una AUC-ROC de 0.95 y diferencias menores al 5% en métricas de equidad.

## Descripción del Problema
El Accidente Cerebrovascular (ACV) representa una de las principales causas de muerte y discapacidad en el mundo. Poder anticipar su ocurrencia a partir de factores clínicos y sociales permite una intervención temprana y focalizada. Nuestro objetivo fue construir un modelo que prediga la probabilidad de ACV y que lo haga de manera justa entre distintos grupos poblacionales.

## Algoritmos evaluados
Durante el desarrollo se probaron múltiples algoritmos:
- Regresión Logística
- Random Forest
- XGBoost
- KNN

El mejor modelo fue **XGBoost**, luego de realizar técnicas de resampling (SMOTE) y optimización de hiperparámetros con validación cruzada.

## Evaluación del modelo final

### Métricas obtenidas
- **Accuracy**: 0.94
- **Precision**: 0.96
- **Recall**: 0.91
- **F1-Score**: 0.93
- **AUC-ROC**: 0.95

### Validación cruzada
Se utilizó validación cruzada estratificada con 5 folds. Los resultados fueron consistentes en todos los conjuntos.

## Equidad del modelo
Para evaluar la equidad se midieron:
- **Demographic Parity Difference**: 0.02
- **Equal Opportunity Difference**: 0.03

Estas métricas están dentro del umbral deseado (<0.05), lo cual indica un modelo justo y robusto frente a sesgos por género o situación laboral.

## Análisis y Visualizaciones
El modelo balanceado mostró un aumento de más de 6 puntos porcentuales en recall respecto al modelo baseline. Las curvas ROC evidencian una mejora clara en separabilidad. Las métricas de fairness mejoraron gracias al balanceo y a la adecuada selección de hiperparámetros.

## Conclusiones
El modelo final es confiable, justo y útil como herramienta de apoyo en sistemas de salud. Se recomienda su implementación junto con monitoreo periódico de métricas de equidad.

## Referencias
- Scikit-learn
- Fairlearn
- XGBoost
- Kaggle Stroke Dataset
