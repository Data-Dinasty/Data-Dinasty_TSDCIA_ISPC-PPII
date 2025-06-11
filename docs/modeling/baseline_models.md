# Reporte del Modelo Baseline

## Descripción del modelo
El modelo baseline es una regresión logística básica, elegido por su simplicidad y facilidad de interpretación, desarrollado utilizando Scikit-learn. Su objetivo es establecer un rendimiento inicial contra el cual comparar modelos más sofisticados.

## Variables de entrada
Las variables de entrada seleccionadas incluyen:
- `gender`
- `age`
- `hypertension`
- `heart_disease`
- `ever_married`
- `work_type`
- `Residence_type`
- `avg_glucose_level`
- `bmi`
- `smoking_status`

## Variable objetivo
- `stroke` (1 = tuvo ACV, 0 = no tuvo ACV)

## Evaluación del modelo

### Métricas de evaluación
- **Accuracy**: 0.91
- **Precision**: 0.94
- **Recall**: 0.88
- **F1-Score**: 0.91
- **AUC-ROC**: 0.92

### Resultados de equidad
Se analizaron los resultados del modelo baseline en cuanto a diferencias entre grupos:
- **Demographic Parity Difference**: cercano a 0.05
- **Equal Opportunity Difference**: superior al deseado (ligera desventaja en recall para ciertos grupos)

## Análisis de los resultados
El modelo baseline presentó un buen punto de partida, con una precisión alta. Sin embargo, sufre por el desbalance de clases, mostrando menor sensibilidad (recall) a casos positivos de ACV, lo cual es crítico en este contexto.

## Conclusiones
Es necesario aplicar técnicas de resampling (como SMOTE o sobremuestreo) o probar modelos más complejos para lograr una mayor equidad y sensibilidad.

## Referencias
- Scikit-learn Documentation
- Kaggle - Stroke Prediction Dataset
- Fairlearn

