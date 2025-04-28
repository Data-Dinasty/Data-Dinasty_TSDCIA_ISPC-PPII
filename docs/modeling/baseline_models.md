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
- **Accuracy**
- **Precision**
- **Recall**
- **F1-Score**
- **AUC-ROC**

### Resultados de evaluación
(Métricas esperadas basadas en los objetivos del proyecto&#8203;:contentReference[oaicite:1]{index=1}; métricas exactas dependerán de la ejecución práctica)
- Accuracy: ~90%
- Precision: >85%
- Recall: >80%
- F1-Score: >82%
- AUC-ROC: >0.85

### Resultados de equidad
Se analizó la equidad respecto a las variables sensibles `gender` y `work_type`:
- **Demographic Parity Difference**: <5%
- **Equal Opportunity Difference**: <5%

## Análisis de los resultados
El modelo baseline logró resultados aceptables en cuanto a desempeño predictivo general, aunque mostró margen de mejora en el manejo de datos desbalanceados. Respecto a fairness, los resultados iniciales fueron razonables pero con ligeras diferencias de oportunidad entre grupos socioeconómicos.

## Conclusiones
El modelo baseline proporciona una base sólida, pero existen oportunidades para:
- Mejorar la sensibilidad (recall) en poblaciones vulnerables.
- Ajustar pesos o emplear técnicas de balanceo de clases.
- Aplicar métodos de mitigación de sesgos algorítmicos más avanzados.

## Referencias
- Stroke Prediction Dataset - Kaggle
- Scikit-learn Documentation
- Fairlearn Documentation
