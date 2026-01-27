# WRFmodel_over_Windows
Sistema generado en Streamlit en Python, para procesar el modelo atmosférico regional WRF compilado en Windows por CMAKE

Ademas se ha generado 2 ejecutables para el uso en cualquier computador con sistema operativo Windows:
1) Descarga_WRF.exe : Que realiza la descarga de las carpetas WPS y WRF de, projecto CMAKE
                   https://github.com/WRF-CMake/wrf
                   Y ademas la carpeta de datos geograficos de baja resolucion.

2) run.exe: Que es el App web del modelo WRF. Esta App esta dividida en 4 partes:
            - Selección del dominio espacial y fechas para la modelizacion.
            - Descarga de datos del modelo GFS a 0.25° y preprocesamiento.
            - Preparación de las condiciones iniciales y de contorno y la modelización.
            - Generación de graficas para evaluación

# Uso del App WRFmodel_over_Windows
Lo primero es descargar el archivo comprimido WRF_Windows.zip, el cual contiene los 2 ejecutables y un archivo namelist.wps 

Luego dentro de tu carpeta de trabajo ejecutar Descarga_WRF.exe para descargar el modelo WRF y datos geograficos.
Y listo ahora ejecutamos el script run.exe y a empezar (👍 ✅)

Entonces se abrira una pagina web o un terminal con la ruta de la pagina web: http://172.25.201.8:8501

<img width="632" height="112" alt="image" src="https://github.com/user-attachments/assets/a533a32c-8b48-4b5f-8f33-6733a5405932" />

Teniendo finalmente el entorno web para el uso del modelo WRF.

<img width="1797" height="943" alt="image" src="https://github.com/user-attachments/assets/0a535e35-93d8-4f67-b51e-bcd36eeafa87" />

El cual esta compuesta pou una barra vertical a la derecha para limpiar archivos temporales y finalizar un proceso.
Y cuatro ventanas, siendo la primera para la selección del dominio espacial y seleccion de fecha de odleizacion y descarga de datos.

La segunda ventana

