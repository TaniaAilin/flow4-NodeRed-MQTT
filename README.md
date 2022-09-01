# flow4-NodeRed-MQTT
Este repositorio contiene el flow 4 del curso de NodeRed, visto en en los contenidos de Internet de las cosas de Codigo IoT en edu.codigoiot.com
# Introducción
Este flow consiste en un tablero que presente la información de temperatura y humedad locales. Este flow recibe la información por MQTT con un broker local.

# Material Necesario
Para realizar este flow necesitas lo siguiente

Ubuntu 20.04
NodeJS
NPM
NodeRed
Nodos Dashboard
Mosquitto
Material de referencia
En los siguientes enlaces puedes encontrar cursos en la plataforma de edu.codigoiot.com que te permitirán realiar las configuraciones necesarias

Instalación de Virutal Box y Ubuntu 20.04
Instalación de NodeRed
Introducción a NodeRed
Introducción a Mosquitto
# Instrucciones
  Requisitos previos
Para que este flow funcione, debes cumplir con los siguientes requisitos previos

Instalación de NodeJS. Se recomienda tener instalado NodeJS en alguna versión LTS. Al momento de creación de este documento, se usó la versión 16.17.0LTS. Esta instalación debe incluir las Build-Tools para hacer uso de NPM
Instalación de NodeRed. La instalación se realiza por NPM. Al momento de la creación de este contenido, se usó la versión 3.0.2
Instalar los nodos node-red-dashboard. Para ello, dirigete a la opcion "Manage Palet" de NodeRed y en la pestaña Install busca node-red-dashboard. Finalmente haz clic en instalar.
Instalación de Broker local Mosquitto MQTT.
  Instrucciones de preparación del entorno
Para ejecutar este flow, es necesario lo siguiente

Arrancar NodeRed con el comando node-red
Importar el flow del repositorio
Hacer clic en el boton Deploy
Instrucciones de operación
Para observar el resutlado de este flow, abre un navegador y dirígete a localhost:1880/ui
Enviar por MQTT un mensaje que contenga un JSON con las variables ID, temp y hum
  Notas
Este Flow se suscribe al tema codigoIoT/Mor/mqtt/flow4
El mensaje mqtt usado para probar este flow es mosquitto_pub -h localhost -t codigoIoT/Mor/mqtt/flow4 -m '{"ID":"Tania Ailin","temp":20,"hum":100}'
Para que la gráfica historica muestre información, deben enviarse al menos 2 puntos
Resultados
A continuación puedes ver los nodos del flow. 

![Captura de pantalla de 2022-09-01 07-34-56](https://user-images.githubusercontent.com/111372187/187925539-d091175c-4980-4318-84c8-052f7ab88693.png)

A continuación puede ver el tablero resultante.

![Captura de pantalla de 2022-09-01 08-26-00](https://user-images.githubusercontent.com/111372187/187925634-5b1ed61f-5a51-478d-a6d3-4261b9868ad3.png)


# Evidencias
https://youtu.be/01liZiYrYq4
# Créditos
Desarrollado por Tania Ailin

https://www.facebook.com/tania.ailin.1
https://github.com/TaniaAilin
