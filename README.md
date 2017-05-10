# IoT demo con RaspberryPi, Node-RED y Watson

## Hardware
* RaspberryPi (Zero, 2 o 3), OS recomendado Raspbian Jessie Lite
* Camara USB con microfono integrado
* Protoboard
* 2 Resistencias 100 Ohms, 1 resistencia 4.7 kOhms
* 2 LEDS
* Boton mecanico
* Sensor de temperatura DS18B20
* Cables tipo Jumpers


## Software y configuracion
* NodeRED instalado con los siguientes paquetes adicionales (instalar con npm install o desde node-red):
    * node-red-dashboard
    * node-red-contrib-ibm-watson-iot
    * node-red-node-watson
    * node-red-node-base64
    * node-red-contrib-ds18b20
* fswebcam (instalar con apt-get install)

## Coneccion de los componentes
Diagrama de coneccion:

## Ejecucion
Para que funcionen los flujos de Node-RED hay que tener una cuenta en IBM Bluemix y los servicios Speech2Text y VisualRecognition. Completar los flujos con sus respectivas credenciales.

