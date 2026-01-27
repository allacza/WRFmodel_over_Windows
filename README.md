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
