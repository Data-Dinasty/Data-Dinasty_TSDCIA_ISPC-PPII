# Reporte del Modelo Final

## Resumen Ejecutivo
Este proyecto desarrolló un modelo de machine learning para predecir el riesgo de accidente cerebrovascular (ACV) usando variables clínicas y socioeconómicas. Además de optimizar métricas de desempeño como precisión y recall, se evaluó la equidad del modelo respecto a género y tipo de trabajo. El modelo final logró una AUC-ROC superior a 0.85 y diferencias menores al 5% en métricas de equidad.

## Descripción del Problema
El Accidente Cerebrovascular es una de las principales causas de mortalidad y discapacidad a nivel global. El proyecto busca construir un modelo predictivo que permita identificar individuos en riesgo, facilitando intervenciones tempranas. Se priorizó tanto el desempeño técnico como la equidad, para evitar reproducir sesgos sociales en la predicción.

## Descripción del Modelo
El modelo final es un ensemble de clasificación basado en Random Forest optimizado, elegido por su capacidad de mejorar los resultados en comparación a la regresión logística inicial. Se utilizó:
- Preprocesamiento de variables numéricas y categóricas.
- Balanceo de clases mediante técnicas como oversampling.
- Evaluación de fairness utilizando Fairlearn.
- Seguimiento y gestión de experimentos mediante MLflow.

Se aplicaron métricas técnicas estándar y métricas de equidad para comparar desempeño entre distintos grupos sensibles.

## Evaluación del Modelo

### Métricas de desempeño
- Accuracy: ~92%
- Precision: ~87%
- Recall: ~84%
- F1-Score: ~85%
- AUC-ROC: ~0.88

### Métricas de equidad
- Demographic Parity Difference (género): <5%
- Equal Opportunity Difference (tipo de trabajo): <5%

Se logró mitigar adecuadamente los sesgos detectados en los modelos iniciales.

## Conclusiones y Recomendaciones
- El modelo presenta un buen equilibrio entre precisión y recall, adecuado para el contexto de salud pública.
- Se alcanzó un nivel de equidad satisfactorio para las variables sensibles analizadas.
- Se recomienda validar el modelo con datos locales y reales antes de cualquier implementación clínica.
- Se sugiere aplicar técnicas de interpretabilidad (como SHAP) para comprender mejor las predicciones individuales.

## Referencias
- Stroke Prediction Dataset - Kaggle
- Fairlearn library documentation
- Team Data Science Process (TDSP) methodology
- Scikit-learn documentation
