## Script COVID-19[BASH]

Requisitos:

-Docker

Primero haremos un pull a la imagen siguiente:

`$ docker pull carlosve97/script_covid_mx`

Despues correremos la imagen que descargamos:\
`$ docker run -it carlosve97/script_covid_mx:latest`\

Despues de que se corra aparecerá algo asi, indicando que lo hemos podido correr correctamente:\
`root@<CARACTERES>:` 

Ahora accederemos al directorio scripts_covid y ejecutaremos el script 'script_salud.sh'\
`$ bash scripts_covid/script_salud`

Esto descargará los datos mas actuales de COVID en méxico y generará 3 archivos

<!-- terminar de poner todo lo que genera -->

