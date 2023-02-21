Implementación del protocolo de seguridad
Este es un proyecto de implementación de un protocolo de seguridad en Python. Este protocolo utiliza los algoritmos de cifrado AES y RSA para proporcionar confidencialidad e integridad en la comunicación entre dos procesos, llamados p-a y p-b, a través de un tercer proceso de confianza llamado p-t.

Estructura del proyecto
funciones_aes.py: este archivo contiene las funciones necesarias para cifrar y descifrar los mensajes utilizando el algoritmo AES.
funciones_rsa.py: este archivo contiene las funciones necesarias para cifrar y descifrar los mensajes utilizando el algoritmo RSA.
p-a.py: este archivo implementa el proceso p-a.
p-b.py: este archivo implementa el proceso p-b.
p-t.py: este archivo implementa el proceso p-t.
socket_class.py: este archivo contiene las clases necesarias para la comunicación entre procesos utilizando sockets.
Uso
Para utilizar el protocolo de seguridad, es necesario ejecutar los archivos p-t.py, p-a.py y p-b.py en tres terminales distintas, en este orden:
python p-t.py
python p-a.py
python p-b.py
El proceso p-t se encargará de la generación y distribución de las claves necesarias para el cifrado y descifrado de los mensajes entre p-a y p-b. Los procesos p-a y p-b se encargan de cifrar y descifrar los mensajes utilizando los algoritmos AES y RSA.

Es importante asegurarse de que las dependencias necesarias estén instaladas antes de ejecutar los archivos. Puedes revisar el archivo requirements.txt para verificar las dependencias.