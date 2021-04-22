## Script COVID-19[BASH]

Requisitos:

-Docker

Primero haremos un pull a la imagen siguiente:

`$ docker pull carlosve97/script_covid_mx`

Despues correremos la imagen que descargamos:\
`$ docker run -it carlosve97/script_covid_mx:latest`

Despues de que se corra aparecerá algo asi, indicando que lo hemos podido correr correctamente:\
`root@<CARACTERES>:` 
***
### script_salud.sh

Ahora accederemos al directorio scripts_covid y ejecutaremos el script 'script_salud.sh'\
`$ bash scripts_covid/script_salud`

Esto descargará los datos mas actuales de COVID en méxico y generará un directorio con tres archivos:

* 'factores_de_riesgo.csv' -> archivo que contiene las columnas de edad,fecha,sexo,fecha de defuncion, factores de riesgo y resultado final
* 'confirmados_factores_de_riesgo.csv' -> archivo que contiene las columnas de edad,fecha,sexo,fecha de defuncion, factores de riesgo para todos los casos confirmados en México
* 'negativos_factores_de_riesgo.csv' -> archivo que contiene las columnas de edad,fecha,sexo,fecha de defuncion, factores de riesgo  para todos los casos negativos en México
* 'fallecidos_factores_de_riesgo.csv' archivo que contiene las columnas de edad,fecha,sexo,fecha de defuncion, factores de riesgo  para todos los casos fallecidos en México 
***
### filtro_por_estado.sh

POsteriormente accederemos al directorio scripts_covid y ejecutaremos el script 'filtro_por_estado.sh'\
`$ bash scripts_covid/filtro_por_estado.sh`

Esto dará un menu de los estados disponibles para filtrar los datos y nosotros seleccionamos el estado de nuestra elección (en este caso es Sonora por lo que elegiremos el 26\
`26`

Se crearán dos archivos dentro del directorio 'carpeta_covid':\
*NOTA: $NUM es el numero que elegimos*

* 'casos_totales_estado_$NUM.csv' -> casos totales para el estado de nuestra elección
* 'confirmados_estado_$NUM.csv' -> casos confirmados para el estado de nuestra elección

Listo, ya tenemos todos los archivos para empezar a analizar los datos!
<!-- terminar de poner todo lo que genera -->

