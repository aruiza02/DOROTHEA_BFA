######## EJECUTAR EL LABORATORIO #####################

Configuramos los laboratorios en el archivo conf.yaml. En él podemos cambiar las interfaces de red, si queremos que el tráfico se muestree y las credenciales para generar tráfico de correo electrónico.

Para ejecutar el laboratorio de ataque:

`sudo python3 run.py -t attack`

Para ejecutar el laboratorio de generar tráfico normal:

`sudo python3 run.py -t normal`

Cuando queremos detener la generación de tráfico normal, escribimos "save" y automáticamente el laboratorio guarda el tráfico capturado y los flujos y lo cierra.

Si queremos limpiar todo el entorno del laboratorio, ejecutamos:

`sudo python3 run.py -c`

En caso de que queramos realizar pruebas de precisión del modelo se puede ejecutar el cuaderno de Jupyter MPLS Classifier Jupyter Notebook.ipynb ubicado en la carpeta cuadernos de Jupyter.
Tener en cuenta que es necesario cambiar la ubicación de los archivos .csv de pruebas 