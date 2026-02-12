# WRF en Windows
Es una Interfaz web generado con Streamlit en Python, para procesar el modelo atmosférico regional WRF compilado en Windows por CMAKE

Ademas se ha generado 2 ejecutables para el uso en cualquier computador con sistema operativo Windows:
1) Descarga_WRF.exe : Que realiza la descarga de las carpetas WPS y WRF de, projecto CMAKE
                   https://github.com/WRF-CMake/wrf
                   Y ademas la carpeta de datos geograficos de baja resolucion.

2) run.exe: Que es el App web del modelo WRF. Esta App esta dividida en 4 partes:
            - Selección del dominio espacial y fechas para la modelizacion.
            - Descarga de datos del modelo GFS a 0.25° y preprocesamiento.
            - Preparación de las condiciones iniciales y de contorno y la modelización.
            - Generación de graficas para evaluación

# Uso WRF en Windows
Lo primero es descargar el archivo comprimido WRF_Windows.zip, el cual contiene los 2 ejecutables y un archivo namelist.wps 

Luego dentro de tu carpeta de trabajo ejecutar Descarga_WRF.exe para descargar el modelo WRF y datos geograficos.
Y listo ahora ejecutamos el script run.exe y a empezar (👍 ✅)

Entonces se abrira una pagina web o un terminal con la ruta de la pagina web: http://172.25.201.8:8501

Teniendo finalmente el entorno web para el uso del modelo WRF.

<img width="1800" height="926" alt="image" src="https://github.com/user-attachments/assets/f175a6bf-0799-4773-b8a1-b150a2982ec5" />

El cual esta compuesta pou una barra vertical a la derecha para limpiar archivos temporales y finalizar un proceso.
Y cuatro ventanas, siendo la primera para la selección del dominio espacial y seleccion de fecha de odleizacion y descarga de datos.

La segunda ventana

<img width="1351" height="780" alt="image" src="https://github.com/user-attachments/assets/da75b860-050b-4632-bc8b-48400a9e8d84" />

La tercera ventana
<img width="1370" height="926" alt="image" src="https://github.com/user-attachments/assets/b90ac9b4-0ae3-4645-a5ae-cdf387cc8762" />

<img width="1362" height="898" alt="image" src="https://github.com/user-attachments/assets/28f6b47e-216a-4c4c-8bbc-86effe8fdc95" />

La ultima ventana presenta graficas de revisión de variables modelizadas

<img width="1373" height="908" alt="image" src="https://github.com/user-attachments/assets/7aecd85e-252a-4449-b008-ee15cd36af03" />



# Monitoreo del proceso
Adicionalmente puedes monitorear si se utiliza la misma cantida de procesadores con el comando en la terminal de Windows:

Get-Process | Where-Object { $_.ProcessName -match "wrf" }


