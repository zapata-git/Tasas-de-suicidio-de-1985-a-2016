# Tasas-de-suicidio-de-1985-a-2016
El conjunto de datos "Suicide Rates Overview 1985 to 2016"** recopila información sobre tasas de suicidio a nivel mundial, con el objetivo de encontrar correlaciones con tasas de suicidio más altas en diferentes cohortes a lo largo del tiempo

## Integrantes del proyecto

- JUAN FERNANDO CARDONA RUIZ, CC , Ingeniería de Sistemas.
- CARLOS OSVALDO ZAPATA ARANGO, CC 1044504411, Ingeniería de Sistemas.

## Fuente de datos

Los datos utilizados en este proyecto provienen de una competencia en Kaggle llamada "Resumen de las tasas de suicidio de 1985 a 2016". 
El enlace a la fuente de datos es el siguiente: https://www.kaggle.com/datasets/russellyates88/suicide-rates-overview-1985-to-2016.

## Requerimientos

- Python 3.7 o superior
- pandas 1.2.4 o superior
- numpy 1.20.2 o superior
- scikit-learn 0.24.2 o superior
- matplotlib 3.4.2 o superior

## Obtención de los datos

Para obtener los datos y hacerlos disponibles en los notebooks cuando se ejecutan en Colab, siga los siguientes pasos:

1. Descargue los archivos de datos de la fuente mencionada anteriormente.
2. Guarde los archivos de datos en una carpeta llamada "data" en el directorio principal del proyecto.
3. En los notebooks de Colab, asegúrese de que la carpeta "data" esté montada en el entorno ejecutando el siguiente código:

      ```python
          from google.colab import drive
          drive.mount('/content/drive')

          import os
          os.chdir('/content/drive/MyDrive/path/to/project').
  
