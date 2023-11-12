# Proyecto "Tasas-de-suicidio-de-1985-a-2016"
El siguiente README proporciona información detallada sobre el proyecto "Tasas-de-suicidio-de-1985-a-2016" que utiliza el conjunto de datos "Suicide Rates Overview 1985 to 2016". Este conjunto de datos recopila información sobre tasas de suicidio a nivel mundial con el propósito de analizar las correlaciones con tasas de suicidio más altas en diferentes cohortes a lo largo del tiempo.

## Notebook 0: Análisis Exploratorio de Datos (EDA)
En este notebook, se encontrará visualizaciones y análisis descriptivos que proporcionarán información clave sobre las tendencias en las tasas de suicidio y las variables relevantes. El propósito principal es explorar y comprender la estructura y características del conjunto de datos "Suicide Rates Overview 1985 to 2016".

## Notebook 1: Modelos de Regresión
Después de haber adquirido una comprensión inicial del conjunto de datos en el Notebook 0, se encuentra el Notebook de Modelos de Regresión. Aquí, se aplican diversos modelos para predecir tasas de suicidio, y se realiza un análisis comparativo para identificar cuál de ellos se ajusta mejor a los datos. Este notebook proporcionará información sobre la capacidad predictiva de diferentes modelos, permitiendo al usuario tomar decisiones informadas sobre su aplicabilidad en el contexto del proyecto.

## Integrantes del Proyecto

- **Juan Fernando Cardona Ruiz**, CC 1044508271, Ingeniería de Sistemas.
- **Carlos Osvaldo Zapata Arango**, CC 1044504411, Ingeniería de Sistemas.

## Fuente de Datos

Los datos utilizados en este proyecto provienen de una competencia en Kaggle titulada "Resumen de las tasas de suicidio de 1985 a 2016". Puede acceder a la fuente de datos a través del siguiente enlace: [Suicide Rates Overview 1985 to 2016](https://www.kaggle.com/datasets/russellyates88/suicide-rates-overview-1985-to-2016).

## Requerimientos

Asegúrese de contar con las siguientes herramientas y bibliotecas instaladas en su entorno para ejecutar este proyecto:

- Python 3.7 o superior
- pandas 1.2.4 o superior
- numpy 1.20.2 o superior
- scikit-learn 0.24.2 o superior
- matplotlib 3.4.2 o superior

## Obtención de los Datos

### 1. Descargar el JSON Web Token (Kaggle API Token)

Para descargar los datos del conjunto de datos desde Kaggle, debe contar con un archivo JSON Web Token (API Token) que identifica su cuenta. Puede obtener su propio token desde la página de configuración de su cuenta de Kaggle en el enlace [https://www.kaggle.com/settings/account](https://www.kaggle.com/settings/account). Este token es único y personal para cada cuenta.

### 2. Cargar el JSON Web Token

Una vez descargado el JSON Web Token, cárguelo en el entorno donde ejecutará el proyecto. Puede realizar esta carga a través del código siguiente:

```python
from google.colab import files
files.upload()
```

### 3. Extracción de los Archivos del Conjunto de Datos

Luego de cargar el JSON Web Token, proceda a extraer los archivos del conjunto de datos desde Kaggle. Asegúrese de que los archivos queden almacenados en el entorno de ejecución de Google Colab. Este proceso debe realizarse en bloques de código previos:

```python
!rm -r ~/.kaggle
!mkdir ~/.kaggle
!cp kaggle.json ~/.kaggle/
!mv ./kaggle.json ~/.kaggle/
!chmod 600 ~/.kaggle/kaggle.json
```

### 4. Descargar el Conjunto de Datos desde Kaggle

Una vez configurado el JSON Web Token y el entorno de ejecución, puede descargar el conjunto de datos desde Kaggle utilizando el siguiente comando:

```python
!kaggle datasets download 'russellyates88/suicide-rates-overview-1985-to-2016'
```

Estos pasos le permitirán obtener el conjunto de datos necesario para realizar análisis y modelado en este proyecto. Con estos datos, podrá explorar tendencias, correlaciones y patrones relacionados con las tasas de suicidio a lo largo de los años.

# Descripción de Notebooks en el Proyecto "Tasas-de-suicidio-de-1985-a-2016"

**[Notebook 0: Análisis Exploratorio de Datos (EDA)]([0 EDA.ipynb](https://github.com/zapata-git/Tasas-de-suicidio-de-1985-a-2016/blob/main/0%20EDA.ipynb))**

El Notebook de Análisis Exploratorio de Datos (EDA) se centra en explorar y comprender la estructura y características del conjunto de datos "Suicide Rates Overview 1985 to 2016". Aquí, se realizan diversas visualizaciones y estadísticas descriptivas para identificar patrones, tendencias y posibles relaciones entre las variables. Los aspectos clave abordados incluyen la distribución de tasas de suicidio a lo largo del tiempo, análisis demográficos y económicos, y otras tendencias relevantes. Este notebook es el punto de partida para comprender el conjunto de datos antes de aplicar modelos de regresión.

**[Notebook 1: Modelos de Regresión]([1 Modelos de regresión.ipynb](https://github.com/zapata-git/Tasas-de-suicidio-de-1985-a-2016/blob/main/1%20Modelos%20de%20regresi%C3%B3n.ipynb))**  

El Notebook de Modelos de Regresión se enfoca en la construcción y evaluación de modelos predictivos para las tasas de suicidio. Aquí se utilizan varios modelos de regresión, como Regresión Lineal, Ridge, Lasso, Support Vector Regression, Random Forest Regression, Gradient Boosting Regression y Multi-layer Perceptron Regression. El proceso incluye la carga del conjunto de datos procesado, la partición en conjuntos de entrenamiento y prueba, la búsqueda de hiperparámetros y la evaluación de modelos mediante métricas como el Error Cuadrático Medio (MSE), el coeficiente de determinación (R2) y el Error Absoluto Mediano (Median Absolute Error). Se proporciona un análisis detallado de cada modelo y sus resultados, ayudando al lector a entender la efectividad y limitaciones de cada enfoque.
