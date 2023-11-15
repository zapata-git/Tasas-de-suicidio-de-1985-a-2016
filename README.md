# Tasas-de-suicidio-de-1985-a-2016

Este proyecto analiza las tasas de suicidio a nivel mundial utilizando el conjunto de datos "Suicide Rates Overview 1985 to 2016". El análisis busca comprender las correlaciones y patrones asociados con tasas de suicidio más altas en diferentes cohortes a lo largo del tiempo.

## Integrantes del Proyecto

- **Juan Fernando Cardona Ruiz**, CC 1044508271, Ingeniería de Sistemas.
- **Carlos Osvaldo Zapata Arango**, CC 1044504411, Ingeniería de Sistemas.

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

## Resultados Actualizados del Análisis de Modelos

El modelo Random Forest Regression destacó con un buen desempeño, presentando un MSE de aproximadamente 4.04 en el conjunto de entrenamiento y 60.80 en el conjunto de prueba, y un coeficiente de determinación (R2) de aproximadamente 0.8260. Mientras que Gradient Boosting Regression tuvo un rendimiento similar con un MSE de aproximadamente 2.64 en el conjunto de entrenamiento y 60.27 en el conjunto de prueba, y un R2 de aproximadamente 0.8275.

## Análisis de Clustering

Se implementó un modelo de clustering con los siguientes resultados:

- **Mejores Hiperparámetros:** Algoritmo 'Elkan', inicialización 'K-means++', 11 clusters, tolerancia 0.001.
- **Puntuación de Validación:** Puntuación media de alrededor de 6905, superior a otros modelos, indicando su eficiencia en la segmentación y definición de clusters.

En resumen, este proyecto ofrece una comprensión detallada de las tasas de suicidio a nivel mundial, analizando correlaciones, patrones y aplicando modelos predictivos para predecir estas tasas con diferentes enfoques y herramientas de aprendizaje automático.
