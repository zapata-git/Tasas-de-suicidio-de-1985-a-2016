<<<<<<< HEAD
¡Claro! Aquí tienes un README que detalla todo sobre el proyecto de tasas de suicidio utilizando el conjunto de datos "Suicide Rates Overview 1985 to 2016":

---

# Tasas-de-suicidio-de-1985-a-2016

Este proyecto analiza las tasas de suicidio a nivel mundial utilizando el conjunto de datos "Suicide Rates Overview 1985 to 2016". El análisis busca comprender las correlaciones y patrones asociados con tasas de suicidio más altas en diferentes cohortes a lo largo del tiempo.
=======
# Proyecto "Tasas-de-suicidio-de-1985-a-2016"
El siguiente README proporciona información detallada sobre el proyecto "Tasas-de-suicidio-de-1985-a-2016" que utiliza el conjunto de datos "Suicide Rates Overview 1985 to 2016". Este conjunto de datos recopila información sobre tasas de suicidio a nivel mundial con el propósito de analizar las correlaciones con tasas de suicidio más altas en diferentes cohortes a lo largo del tiempo.
>>>>>>> 49d3eab80cd5b18d20ed623401cc6e024597290d

### [Notebook 0: Análisis Exploratorio de Datos (EDA)](https://github.com/zapata-git/Tasas-de-suicidio-de-1985-a-2016/blob/main/0%20EDA.ipynb)
En este notebook, se encontrará visualizaciones y análisis descriptivos que proporcionarán información clave sobre las tendencias en las tasas de suicidio y las variables relevantes. El propósito principal es explorar y comprender la estructura y características del conjunto de datos "Suicide Rates Overview 1985 to 2016".

### [Notebook 1: Modelos de Regresión](https://github.com/zapata-git/Tasas-de-suicidio-de-1985-a-2016/blob/main/1%20Modelos%20de%20regresi%C3%B3n.ipynb)
Después de haber adquirido una comprensión inicial del conjunto de datos en el Notebook 0, se encuentra el Notebook de Modelos de Regresión. Aquí, se aplican diversos modelos para predecir tasas de suicidio, y se realiza un análisis comparativo para identificar cuál de ellos se ajusta mejor a los datos. Este notebook proporcionará información sobre la capacidad predictiva de diferentes modelos, permitiendo al usuario tomar decisiones informadas sobre su aplicabilidad en el contexto del proyecto.

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

<<<<<<< HEAD
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
=======
Estos pasos le permitirán obtener el conjunto de datos necesario para realizar análisis y modelado en este proyecto. Con estos datos, podrá explorar tendencias, correlaciones y patrones relacionados con las tasas de suicidio a lo largo de los años.

# Descripción de Notebooks en el Proyecto "Tasas-de-suicidio-de-1985-a-2016"

### [Notebook 0: Análisis Exploratorio de Datos (EDA)](https://github.com/zapata-git/Tasas-de-suicidio-de-1985-a-2016/blob/main/0%20EDA.ipynb)

El Notebook de Análisis Exploratorio de Datos (EDA) se centra en explorar y comprender la estructura y características del conjunto de datos "Suicide Rates Overview 1985 to 2016". Aquí, se realizan diversas visualizaciones y estadísticas descriptivas para identificar patrones, tendencias y posibles relaciones entre las variables. Los aspectos clave abordados incluyen la distribución de tasas de suicidio a lo largo del tiempo, análisis demográficos y económicos, y otras tendencias relevantes. Este notebook es el punto de partida para comprender el conjunto de datos antes de aplicar modelos de regresión.

### [Notebook 1: Modelos de Regresión](https://github.com/zapata-git/Tasas-de-suicidio-de-1985-a-2016/blob/main/1%20Modelos%20de%20regresi%C3%B3n.ipynb)

El Notebook de Modelos de Regresión se enfoca en la construcción y evaluación de modelos predictivos para las tasas de suicidio. Aquí se utilizan varios modelos de regresión, como Regresión Lineal, Ridge, Lasso, Support Vector Regression, Random Forest Regression, Gradient Boosting Regression y Multi-layer Perceptron Regression. El proceso incluye la carga del conjunto de datos procesado, la partición en conjuntos de entrenamiento y prueba, la búsqueda de hiperparámetros y la evaluación de modelos mediante métricas como el Error Cuadrático Medio (MSE), el coeficiente de determinación (R2) y el Error Absoluto Mediano (Median Absolute Error). Se proporciona un análisis detallado de cada modelo y sus resultados, ayudando al lector a entender la efectividad y limitaciones de cada enfoque.
>>>>>>> 49d3eab80cd5b18d20ed623401cc6e024597290d
