# Tasas-de-suicidio-de-1985-a-2016

Este proyecto analiza las tasas de suicidio a nivel mundial utilizando el conjunto de datos "Suicide Rates Overview 1985 to 2016". El análisis busca comprender las correlaciones y patrones asociados con tasas de suicidio más altas en diferentes cohortes a lo largo del tiempo.

## Integrantes del Proyecto Ingeniería de Sistemas

- **Juan Fernando Cardona Ruiz**
- **Carlos Osvaldo Zapata Arango**

## Fuente de Datos

Los datos se obtuvieron de la competencia en Kaggle llamada "Resumen de las tasas de suicidio de 1985 a 2016". Puede acceder a la fuente de datos [aquí](https://www.kaggle.com/datasets/russellyates88/suicide-rates-overview-1985-to-2016).

## Requerimientos

Asegúrese de contar con las siguientes herramientas y bibliotecas instaladas en su entorno para ejecutar este proyecto:

- Python 3.7 o superior
- pandas 1.2.4 o superior
- numpy 1.20.2 o superior
- scikit-learn 0.24.2 o superior
- matplotlib 3.4.2 o superior

## Obtención de los Datos

### 1. Descargar el JSON Web Token (Kaggle API Token)

Para descargar los datos del conjunto de datos desde Kaggle, debe contar con un archivo JSON Web Token (API Token) que identifica su cuenta. Puede obtener su propio token desde la página de configuración de su cuenta de Kaggle [aquí](https://www.kaggle.com/settings/account). Este token es único y personal para cada cuenta.

### 2. Cargar el JSON Web Token

Una vez descargado el JSON Web Token, cárguelo en el entorno donde ejecutará el proyecto utilizando el código proporcionado.

### 3. Extracción de los Archivos del Conjunto de Datos

Luego de cargar el JSON Web Token, proceda a extraer los archivos del conjunto de datos desde Kaggle. Asegúrese de almacenarlos en el entorno de ejecución. Los comandos necesarios están detallados en el README del proyecto.

## Notebook.

### [Notebook 0: Análisis Exploratorio de Datos (EDA)](https://github.com/zapata-git/Tasas-de-suicidio-de-1985-a-2016/blob/main/0%20EDA.ipynb)
En este notebook, se encontrará visualizaciones y análisis descriptivos que proporcionarán información clave sobre las tendencias en las tasas de suicidio y las variables relevantes. El propósito principal es explorar y comprender la estructura y características del conjunto de datos "Suicide Rates Overview 1985 to 2016".

### [Notebook 1: Modelos de Regresión](https://github.com/zapata-git/Tasas-de-suicidio-de-1985-a-2016/blob/main/1%20Modelos%20de%20regresi%C3%B3n.ipynb)
Después de haber adquirido una comprensión inicial del conjunto de datos en el Notebook 0, el usuario puede dirigirse al Notebook de Modelos de Regresión. Aquí, se aplican diversos modelos para predecir tasas de suicidio, y se realiza un análisis comparativo para identificar cuál de ellos se ajusta mejor a los datos. Este notebook proporcionará información sobre la capacidad predictiva de diferentes modelos, permitiendo al usuario tomar decisiones informadas sobre su aplicabilidad en el contexto del proyecto.

### [Notebook 2: Modelos de Clasificación](https://github.com/zapata-git/Tasas-de-suicidio-de-1985-a-2016/blob/main/2%20Modelos%20de%20clasificaci%C3%B3n.ipynb)
Después de explorar y comprender el conjunto de datos en el Notebook 1: Modelos de Regresión, se puede avanzar al Notebook de Modelos de Clasificación para profundizar aún más en el análisis. En este notebook, nos sumergimos en la aplicación de diversos modelos de clasificación con el objetivo de predecir y clasificar las tasas de suicidio en diferentes cohortes y regiones.

## Conclusiones del Análisis Exploratorio

El análisis exploratorio revela información clave sobre las tasas de suicidio a nivel global:

- **Visión de Suicidios:** El conjunto de datos ofrece información detallada sobre suicidios en múltiples países a lo largo de varios años.
- **Información Relevante:** Proporciona datos demográficos, cifras de suicidios, población, tasas de suicidio y datos económicos, permitiendo un análisis detallado.
- **Valores Faltantes Tratados:** Se imputaron valores faltantes en la columna "HDI for year" utilizando la mediana de los valores disponibles.
- **Diversidad de Formatos:** Presenta una diversidad de formatos de datos que permiten un análisis exhaustivo.

## Análisis y Modelado

Se aplicaron varios modelos de regresión para predecir las tasas de suicidio:

- **Regresión Lineal, Ridge y Lasso:** Mostraron un rendimiento limitado con errores cuadráticos medios similares.
- **SVR:** Mejoró el rendimiento con una capacidad moderada para explicar la variabilidad en los datos.
- **Random Forest y Gradient Boosting:** Destacaron con un buen rendimiento y mayor capacidad para explicar la variabilidad en los datos.
- **MLP:** Aunque aceptable, no superó a los modelos basados en árboles en este contexto.

## Resultados del Análisis de Modelos de Regresión

El modelo Random Forest Regression destacó con un buen desempeño, presentando un MSE de aproximadamente 4.04 en el conjunto de entrenamiento y 60.80 en el conjunto de prueba, y un coeficiente de determinación (R2) de aproximadamente 0.8260. Mientras que Gradient Boosting Regression tuvo un rendimiento similar con un MSE de aproximadamente 2.64 en el conjunto de entrenamiento y 60.27 en el conjunto de prueba, y un R2 de aproximadamente 0.8275.

## Resultados del Análisis de Clustering K-Means

Se aplicaron modelos de clustering K-Means para identificar patrones en los datos:

- **Mejor Modelo:** El modelo con mejor desempeño fue el que utilizó 2 clusters, inicialización aleatoria, algoritmo de fuerza bruta y tolerancia de 1e-05.
    - Tiempo de evaluación: 0.3037 segundos en promedio.
    - Puntaje de prueba: -59425.564754.
    - Desviación estándar del puntaje de prueba: 11732.176734.
