# DOROTHEA_BFA
Laboratorio de ataques de fuerza bruta basados en Hydra con modelo de predicción.

######## EJECUTAR EL LABORATORIO #####################

Configuramos los laboratorios en el archivo conf.yaml ubicado en la carpeta Labs. 
En él podemos cambiar las interfaces de red y otros atributos.

Para ejecutar el laboratorio de ataque:
sudo python3 run.py -t attack

Por defecto se generará una ataque con el archivo rockyou.txt el cual habrá que descargar y poner en la ubicación Labs\lab_attacks\attacker
En nuestro caso, en dicha ubicación, está el archivo rockyoufinal.txt que es una versión reducida del rockyou.txt (que no se permite subir aquí por exceder el tamaño máximo)
Si se desea utilizar ese archivo, hay que modificar el archivo run_task_hydra.py y poner el nombre del archivo rockyoufinal.txt donde pone rockyou.txt
cmd = ["hydra", "-l", "root", "-P", "rockyou.txt", str(randomize_ip()), "ssh"]

Para ejecutar el laboratorio de generar tráfico normal:
sudo python3 run.py -t normal

Cuando queremos detener la generación de tráfico normal, escribimos "save" y automáticamente el laboratorio guarda el tráfico capturado y los flujos y lo cierra.
Si queremos limpiar todo el entorno del laboratorio, ejecutamos:

sudo python3 run.py -c

En caso de que queramos realizar pruebas de precisión del modelo se puede ejecutar el cuaderno de Jupyter MPLS Classifier Jupyter Notebook.ipynb ubicado en la carpeta cuadernos de Jupyter. Tener en cuenta que es necesario cambiar la ubicación de los archivos .csv de pruebas
