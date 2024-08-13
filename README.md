# Agua-Tierra App Web

Esta herramienta permite hacer una distinción clara entre el entorno marino-fluvial y terrestre a partir de seleccionar un área de interés.

El algoritmo fue consruido en el entorno de Google Earth Engine, a partir de imágenes SENTINEL-2A/B MSI Nivel 1C para el primer trimestre del 2023, el Índice de Diferencia Normalizada de Agua (NDWI), un DEM, puntos de muestreo y el algoritmo de distancia mínima.

&nbsp;


                                             --- Instalación ---

El **primer paso** es crear una cuenta en Google Earth Engine, en caso de no tener una. Link a Google Earth Engine: https://earthengine.google.com/

Una vez hecho esto, será necesario guardar el nombre del proyecto personal que se encuentra en el borde superior derecho de la pagina, como indica la flecha roja.

![image](https://github.com/user-attachments/assets/0d42ec22-373b-4142-9dcb-4ef9a1746928)

&nbsp;
-----------------------------------------------------------------------------------------------------

El **segundo paso** es descargar la carpeta AguaTierraAppWeb desde GitHub en **Code ----> Download ZIP**

![image](https://github.com/user-attachments/assets/922c421c-6628-466d-979c-cd2e1a3c7686)

&nbsp;

A continuación, guardar la descarga en una carpeta en nuestra pc y accedar hasta ver los archivos (flecha azul). Vamos a necesitar hacer dos cosas para poder hacer uso de la aplicación Agua-Tierra App Web. 

![image](https://github.com/user-attachments/assets/290640a8-ea48-4895-8818-b301825f28e4)

&nbsp;

Por un lado, **ABRIR** el archivo AguaTierra.ipynb y **MODIFICAR** la linea **"ee.Initialize(project='...')"** con el nombre de tu proyecto. Se encuentra dentro de las primeras líneas del archivo (flecha roja). 

![image](https://github.com/user-attachments/assets/dc1ca3e7-e16f-43ab-8c3d-ff13986e7366)


Por otro lado, vamos a necesitar **COPIAR** la ruta donde se encuentran los archivos (flecha verde) para un paso más adelante.

&nbsp;
-----------------------------------------------------------------------------------------------------

El **tercer paso** es la **intsalación de los componentes** de la aplicación en nuestra PC. Será necesario ejecutar los siguientes pasos en orden (texto en negrita).


  1- Abrir la consola de Anaconda o Minianaconda. 

  2- Pararse en la carpeta contenedora del proyecto: **cd ruta\donde\estan\los\archivos** (acá va la ruta mencionada mas arriba con la flecha verde)
  
  3- Crear el entorno virtual con todas las dependecias utilizadas: **conda env create --file ENV.yml**

  4- Activar el entorno virtual: **conda activate env_time**

  5- Otorgar permisos: **earthengine authenticate**
  
  6- Cerrar la consola.

  
&nbsp;

                       --- Ejecutar la aplicación ---

Una vez instalado, cada vez que se quiera ejecutar la aplicación, se deberán ejecutar los siguientes pasos:

  1- Abrir la consola de Anaconda o Minianaconda. 

  2- Acceder a la carpeta contenedora del proyecto:  **cd ruta\donde\estan\los\archivos** (acá va la ruta mencionada mas arriba con la flecha verde)

  3- Activar el entorno virtual: **conda activate env_time**

  4- Ejecutar la aplicación: **voila AguaTierra.ipynb**

Listo!

&nbsp;
----------------------------------------------------------------------------------------------------------------  

© 2024 Autor. Licensed under the Apache License 2.0.



