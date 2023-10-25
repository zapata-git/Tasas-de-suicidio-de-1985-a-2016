# Tasas-de-suicidio-de-1985-a-2016
El conjunto de datos "Suicide Rates Overview 1985 to 2016" recopila información sobre tasas de suicidio a nivel mundial, 
con el objetivo de encontrar correlaciones con tasas de suicidio más altas en diferentes cohortes a lo largo del tiempo.

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
#PARA EJECUTAR ESTA LÍNEA, EN EL COMPUTADOR QUE SE EJECUTE DEBE HABER UNA COPIA DEL JSON WEB TOKEN
#DESCARGABLE DESDE LA PÁGINA DE UNA CUENTA DE KAGGLE EN https://www.kaggle.com/settings/account?...
#ESTE JSON WEB TOKEN ES PERSONAL DE CADA CUENTA Y SIRVE COMO IDENTIFICADOR DE ACCESO.
#CARGUE EL JSON QUE USTED DESCARGÓ DE SU CUENTA DE KAGGLE
files.upload()

#Extracción de los archivos del conjunto de datos descargados desde Kaggle
* El conjunto de datos descargado

* Los archivos quedan almacenados en el entorno de ejecución de Google Colab siempre y cuando se haya autorizado el acceso de la cuenta de Google a este.
* Esto se debió realizar en bloques de código anteriores.

!rm -r ~/.kaggle
!mkdir ~/.kaggle
!cp kaggle.json ~/.kaggle/
!mv ./kaggle.json ~/.kaggle/
!chmod 600 ~/.kaggle/kaggle.json
#!kaggle datasets list

#Para descargar el conjunto de datos desde Kaggle al drive local de Google

!kaggle datasets download 'russellyates88/suicide-rates-overview-1985-to-2016'


         
  
