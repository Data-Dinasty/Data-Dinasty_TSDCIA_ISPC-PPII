# Reporte de Datos

## Resumen general de los datos
El dataset contiene información clínica y demográfica de 5110 personas con el objetivo de predecir la ocurrencia de un accidente cerebrovascular. Incluye variables como edad, nivel de glucosa en sangre, índice de masa corporal, antecedentes de hipertensión, enfermedades cardíacas, tipo de trabajo, estado civil, entre otras. La variable objetivo es binaria (stroke: 0 o 1) y el conjunto de datos presenta un desbalance significativo entre clases.

## Resumen de calidad de los datos
Los datos presentan buena calidad general. Solo la variable bmi contiene valores faltantes, con un 4.9% de registros incompletos. No se detectan valores faltantes en el resto de las variables. Algunas variables categóricas requieren codificación para su uso en modelos predictivos. También se observan posibles outliers en variables numéricas como glucosa y BMI.

## Variable objetivo
La variable objetivo es stroke, que indica si una persona ha sufrido un accidente cerebrovascular (1) o no (0). Esta variable está fuertemente desbalanceada, con solo un 4.9% de casos positivos en el conjunto de datos. Esto sugiere la necesidad de aplicar técnicas de balanceo como sobremuestreo (SMOTE) o penalización en modelos.

## Variables individuales
- Gender: Género del paciente (Male, Female, Other).
- age: Edad del paciente (0–100).
- hypertension: 1 si el paciente tiene hipertensión, 0 si no.
- heart_disease: 1 si tiene enfermedad cardíaca, 0 si no.
- ever_married: Estado civil (Yes o No).
- work_type: Tipo de trabajo (Private, Self-employed, Govt_job, Children, Never_worked).
- Residence_type: Zona de residencia (Urban o Rural).
- avg_glucose_level: Nivel promedio de glucosa en sangre.
- bmi: Índice de masa corporal (puede contener nulos).
- smoking_status: Estado de fumador (formerly smoked, never smoked, smokes, unknown).
- stroke: Variable objetivo, indica si tuvo un ACV.

## Ranking de variables
1 age
2 avg_glucose_level
3 bmi
4 hypertension
5 heart_disease
6 ever_married
7 smoking_status
8 work_type
9 Residence_type
10 gender

## Relación entre variables explicativas y variable objetivo
Se observa una fuerte asociación entre la edad, nivel de glucosa y antecedentes de hipertensión/enfermedades cardíacas con la presencia de ACV. A mayor edad y mayor glucosa, aumenta el riesgo de sufrir un ACV. También existe una mayor proporción de ACV en personas casadas y con ciertos tipos de empleo (como quienes nunca trabajaron). Las variables como gender y Residence_type muestran baja correlación con la variable objetivo.
