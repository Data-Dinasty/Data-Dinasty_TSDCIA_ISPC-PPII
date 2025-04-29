# Project Charter - Entendimiento del Negocio

## Nombre del Proyecto

Predicción de Riesgo de Accidente Cerebrovascular con Equidad

## Objetivo del Proyecto

Desarrollar un modelo de machine learning capaz de predecir la probabilidad de que una persona sufra un accidente cerebrovascular (ACV) utilizando datos clínicos y socioeconómicos. Además de alcanzar un alto desempeño técnico, el proyecto busca evaluar y mitigar posibles sesgos, especialmente relacionados con género y condición laboral.

## Alcance del Proyecto

### Incluye:

- Uso del dataset "Stroke Prediction Dataset" disponible en Kaggle.
- Análisis exploratorio de datos clínicos, demográficos y socioeconómicos.
- Desarrollo de modelos de clasificación supervisada.
- Evaluación del rendimiento del modelo mediante métricas de desempeño técnico (Accuracy, Recall, Precision, F1-Score, AUC-ROC).
- Evaluación de equidad utilizando métricas de fairness (Demographic Parity y Equal Opportunity).
- Documentación del proceso en GitHub y seguimiento del trabajo en Jira o Trello.

### Excluye:

- Implementación clínica real en hospitales o centros de salud.
- Recolección de nuevos datos o conexión a bases de datos sanitarias externas.
- Diagnóstico médico o validación con datos en tiempo real.

## Metodología

Se seguirá el enfoque TDSP (Team Data Science Process), estructurado en las fases de entendimiento del negocio, exploración de datos, modelado, validación, despliegue y evaluación. Se emplearán herramientas como Python, Scikit-learn, MLflow y Fairlearn para el desarrollo técnico y análisis de equidad.

## Cronograma

| Etapa | Duración Estimada | Fechas |
|------|--------------------|--------|
| Entendimiento del negocio y carga de datos | 2 semanas | del 6 de abril al 28 de abril |
| Preprocesamiento, análisis exploratorio | 3 semanas | del 29 de abril al 16 de mayo |
| Modelamiento y extracción de características | 2 semanas | del 16 de mayo al 30 de mayo |
| Despliegue | 2 semanas | del 30 de mayo al 6 de junio |
| Evaluación y entrega final | 3 semanas | del 6 de junio al 27 de junio |

> Nota: Las fechas deben ajustarse si se modifica el calendario de trabajo.

## Equipo del Proyecto

- *Project Manager*: Julieta Battauz – Responsable de la coordinación general del proyecto.
- *Data Engineer*: Dante Javier Pagano, Laura Peralta – Responsable de la carga, limpieza y transformación de datos.
- *Data Scientist*: Marcelo Molina, Federico Gurrea – Encargado del desarrollo y evaluación de modelos.
- *Ethical Reviewer*: Eugenia Barozzi – Responsable de la evaluación de equidad y sesgos.

## Presupuesto

No aplica. Proyecto académico/simulativo sin presupuesto asignado.

## Stakeholders

- **Autoridades Sanitarias**: Usuarios finales interesados en políticas preventivas basadas en datos.
- **Profesionales de la Salud**: Usuarios que aplicarán predicciones para intervenciones tempranas.
- **Comunidad General**: Beneficiarios del proyecto a través de mejores diagnósticos y prevención.
- **Equipo de Ciencia de Datos**: Desarrollo y control de calidad técnica y ética del modelo.

Expectativas:
- Alta precisión en predicciones.
- Evaluación rigurosa de equidad.
- Entregables claros y documentados.

## Aprobaciones

- [Nombre del aprobador]: Carlos Ignacio CHARLETTI
- [Firma del aprobador]: ___________________
- [Fecha de aprobación]: ___________________
