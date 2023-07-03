# DOROTHEA_BFA
Laboratorio de ataques de fuerza bruta basados en Hydra con modelo de predicción.

######## EJECUTAR EL LABORATORIO #####################

Configuramos los laboratorios en el archivo conf.yaml ubicado en la carpeta Labs. 
En él podemos cambiar las interfaces de red y otros atributos.

Para ejecutar el laboratorio de ataque:
sudo python3 run.py -t attack

Por defecto se generará una ataque con el archivo rockyoufinal.txt que es una versión reducida del rockyou.txt (que no se permite subir aquí por exceder el tamaño máximo)

Para ejecutar el laboratorio de generar tráfico normal:
sudo python3 run.py -t normal

Cuando queremos detener la generación de tráfico normal, escribimos "save" y automáticamente el laboratorio guarda el tráfico capturado y los flujos y lo cierra.
Si queremos limpiar todo el entorno del laboratorio, ejecutamos:

sudo python3 run.py -c

En caso de que queramos realizar pruebas de precisión del modelo se puede ejecutar el cuaderno de Jupyter MPLS Classifier Jupyter Notebook.ipynb ubicado en la carpeta cuadernos de Jupyter. Tener en cuenta que es necesario cambiar la ubicación de los archivos .csv de pruebas

En la carpeta Labs se localizan los dos datsets principales utilizados para las pruebas de aprendizaje y resultados:
   - csv_normalizado.csv
   - dataset_text.csv
