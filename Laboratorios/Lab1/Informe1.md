<p align="left">
  <img src="https://seeklogo.com/images/U/u-cayetano-heredia-logo-CA435ADF8C-seeklogo.com.png" width="200">
  <h1 align="center">Informe I</h1>
</p>
 
<strong>Docentes:</strong>
- Mg. Umbert Lewis De La Cruz Rodriguez 
- Mg. Marcos Retamozo Ramos
- Mg. Moises Stevend Meza Rodriguez
- Mg. Carol Ordoñez Aquino
- Dr. Harry Anderson Rivera Tito  
- Dr. Pierre Ramos Apestegui 
- Ing. Renzo José Chan Ríos

<strong>Integrantes:</strong>
- Gavidia Crovetto, Bruno Paolo
- Silva Cuzqui, Camilo Sebastián
- Cueva Ramos, José Nilson
- Toribio Alvarado, Stephany Marilyn
- Herrera Valeriano, Jhunior Fernando 

## Introducción

En las últimas décadas, el estudio de las concentraciones de los contaminantes ha revolucionado diversos campos debido a su asociación con problemas de salud [1] y su importancia se rige en cuidar la salud pública, prevenir los efectos a largo y corto plazo y poblaciones vulnerables. Estas investigaciones han demostrado que algunas personas son susceptibles que otras a contaminantes atmosféricos, donde estos grupos incluyen niños, mujeres embarazadas, adultos mayores y personas con enfermedades cardíacas y pulmonares preexistentes [2]. Es así como el presente informe tiene como objetivo analizar el índice de calidad del aire (AQI) en la ciudad de Nueva York, Estados Unidos, durante los años 2022 y 2023, mediante regresión lineal utilizando los datos obtenidos de la United States Environmental Protection Agency (EPA). En consecuencia, este informe abordará la importancia del estudio de la contaminación ambiental y su relación con los problemas de salud, el desarrollo de técnicas de predicción de los contaminantes en los próximos meses y permitirá comprender cómo el monitoreo de la salud ambiental es necesaria para tomar conciencia de la repercusión de los gases.
 
## Metodología

Para llevar a cabo el análisis de la regresión lineal sobre el índice de calidad del aire (AQI) en la ciudad de Nueva York durante los años 2022 y 2023, se siguieron los siguientes pasos:

**Importar las librerías**

```python
#importar librerias para machine learning y regresion lineal
import pandas as pd
import numpy as np
from sklearn.linear_model import LinearRegression
```

**1- Obtención de datos:**

Los datos del AQI fueron recolectados de la base de datos pública de la United States Environmental Protection Agency (EPA). Se descargaron los datos correspondientes a los años 2022 y 2023, asegurando que incluían todos los registros necesarios para el análisis.

[Base de datos](https://github.com/stephany-toribio/IdentificadorDeMicroplasticos/tree/main/Laboratorios/Lab1/Base_de_Datos)


**2- Preprocesamiento de datos:**

Antes de realizar el análisis, se llevó a cabo una limpieza de los datos. Esto incluyó la eliminación de valores nulos o duplicados, la conversión de formatos de fecha, eliminacion de columnas con datos repetidos a los largo de esta. Además, se realizó una exploración inicial de los datos para identificar posibles patrones o anomalías.

Se eliminaron columnas en los cuales en su mayoria eran codigos por tanto no eran necesarios
```python
df.drop('POC', axis=1, inplace=True)
df.drop('AQS Parameter Code', axis=1, inplace=True)
df.drop('CBSA Code', axis=1, inplace=True)
df.drop('State FIPS Code', axis=1, inplace=True)
df.drop('County FIPS Code', axis=1, inplace=True)
df.drop('Method Code', axis=1, inplace=True)
```

Asu ves tambien se eliminaron todos los datos tipo object, los cuales no aportan a la predicción
```python
df.drop(['Source','Units','Local Site Name','AQS Parameter Description','CBSA Name','State','County'], axis=1, inplace=True)
```


**3- Análisis exploratorio de datos (EDA):**

Se realizó un análisis exploratorio de datos para entender mejor la distribución del AQI en los diferentes meses del año  y su relacon con las otras caracteristicas . Esto incluyó la generación de gráficos y estadísticas descriptivas para identificar tendencias y variaciones en la calidad del aire .

Para el uso de las series temporales, establecimos una fecha y luego a la columna "Date" lo convertimos en tipo datetime para luego segun la fecha establecida solo se filtraran en el csv los datos anteriores a esa fecha:
```python
fecha_fin = '2022-12-10'
df['Date'] = pd.to_datetime(df['Date'])
df = df[df['Date'] < fecha_fin]
```

**4- Construcción del modelo de regresión lineal:**

Se utilizó la técnica de regresión lineal para modelar la relación entre las variables independientes seleccionadas (como el tiempo, condiciones meteorológicas, etc.) y el AQI como variable dependiente.

```python
from sklearn.linear_model import LinearRegression
lr.fit(X_train, y_train)

y_pred = lr.predict(X_test)
```

**5- Evaluación del modelo:**

La precisión del modelo de regresión lineal se evaluó utilizando métricas como el coeficiente de determinación (R²) , el error cuadrático medio (MSE)y Error Absoluto Medio (MAE) . Además, se realizaron pruebas de validación cruzada para asegurar la robustez del modelo, en este caso usamos el kfold para evitar el sobreajuste del modelo.

## Resultados
[Colab del laboratorio](https://colab.research.google.com/drive/1NUe_PaJCw6_VrwuNAMcw2oVl9_nWhxDZ?usp=sharing)

<p>En los resultados finales obtuvimos métricas esenciales para evaluar la precisión y la capacidad de generalización de un modelo predictivo. En este caso: </p>

- Media del RMSE de 0.267323... esta indicando que en promedio en las predicciones del modelo se desvian de los valores reales aproximadamente 0.267323... unidades. Esto nos hace referencia a un alto grado de precisión en la predicción, ya que la desviación es pequeña.
```python
RMSE values: [0.26200398 0.27103676 0.26204986 0.26436505 0.27715953]
Mean RMSE: 0.26732303522968265
```


- Media del MAE de 0.205424... esta indicando que en promedio en las predicciones difieren de los valores reales aproximadamente 0.205424... unidades. Esto nos refuerza los resultados obtenidos del RMSE, mostrando una buen rendimiento en terminos de precisión general.
```python
MAE values: [0.20510978 0.21028109 0.19736777 0.20286455 0.21149823]
Mean MAE: 0.20542428594276996

```
- Un R^2 (alto) sugiere que el modelo explica casi toda la variabilidad de los datos.

```python
R² values: [0.98297587 0.98056087 0.98112245 0.98264799 0.98085014]
Mean R²: 0.9816314653381951
```
- Las métricas de entrenamiento son similares al de prueba indicándonos que no esta sobreajustado y es capaz de predecir futuros datos.
```python
Test RMSE: 0.27715952723656134
Test MAE: 0.2114982346273682
Test R²: 0.9808501408409329
```


## Discusión


## Referencias
- [1] D. S. Suárez-Moreno and J. G. Piñeros-Jiménez, "Systematization of experiences on air quality and health surveillance systems in different cities of Latin America and the Caribbean," 2019 Congreso Colombiano y Conferencia Internacional de Calidad de Aire y Salud Pública (CASP), Barranquilla, Colombia, 2019, pp. 1-7, doi: 10.1109/CASAP48673.2019.9364054.
  
- [2] US EPA, O. (2020, octubre 28). Research on Health Effects from Air Pollution. https://www.epa.gov/air-research/research-health-effects-air-pollution

- 
