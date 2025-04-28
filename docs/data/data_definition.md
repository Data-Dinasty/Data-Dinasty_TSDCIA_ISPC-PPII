# Definición de los datos

## Origen de los datos
El conjunto de datos utilizado es el **Stroke Prediction Dataset**, disponible en [Kaggle](https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset).

Este dataset contiene variables clínicas, demográficas y socioeconómicas relevantes para predecir la ocurrencia de un Accidente Cerebrovascular (ACV), incluyendo género, edad, hipertensión, enfermedades cardíacas, tipo de trabajo, residencia (urbana/rural), índice de masa corporal (IMC), y nivel de glucosa.

## Especificación de los scripts para la carga de datos
Los datos se cargan mediante scripts en Python utilizando librerías como `pandas`. Las etapas principales del script incluyen:
- Descarga del dataset desde Kaggle o carga local.
- Limpieza de datos: tratamiento de valores nulos, codificación de variables categóricas.
- Separación en conjunto de entrenamiento y prueba.

## Referencias a rutas o bases de datos origen y destino

### Rutas de origen de datos
- Archivo original: `stroke_data.csv` descargado desde Kaggle.

### Base de datos de destino
- Datos procesados almacenados en estructuras locales (`DataFrame` de pandas) o archivos `.csv` intermedios en el repositorio.
