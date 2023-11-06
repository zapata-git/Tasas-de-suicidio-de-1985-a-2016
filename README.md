El siguiente README proporciona información detallada sobre el proyecto "Tasas-de-suicidio-de-1985-a-2016" que utiliza el conjunto de datos "Suicide Rates Overview 1985 to 2016". Este conjunto de datos recopila información sobre tasas de suicidio a nivel mundial con el propósito de analizar las correlaciones con tasas de suicidio más altas en diferentes cohortes a lo largo del tiempo.

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