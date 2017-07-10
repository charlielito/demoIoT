# IoT demo con RaspberryPi, Node-RED y Watson

## Hardware
* RaspberryPi (Zero, 2 o 3), OS recomendado Raspbian Jessie Lite
* Camara USB con micrófono integrado
* Protoboard
* 2 Resistencias 100 Ohms, 1 resistencia 4.7 kOhms
* 2 LEDS
* Boton mecánico (o capacitivo touch, alguno de los dos)
* Sensor de temperatura DS18B20
* Cables tipo Jumpers


## Software y configuración
* NodeRED instalado con los siguientes paquetes adicionales (instalar con npm install o desde node-red):
    * node-red-dashboard
    * node-red-contrib-ibm-watson-iot
    * node-red-node-watson
    * node-red-node-base64
    * node-red-contrib-ds18b20
* fswebcam (instalar con apt-get install)

## Conexión de los componentes
Diagrama de conección:

![alt text][s1]

## Ejecución
Si no ha instalado los requisitos ir a la carpeta ~/.node-red y ejecutar:
```bash
sudo npm install node-red-dashboard node-red-contrib-ibm-watson-iot node-red-node-watson node-red-node-base64 node-red-contrib-ds18b20
```
```bash
sudo apt-get install fswebcam
```

Para el tutorial, simplemente ejectuar dentro de la carpeta del repo:
```bash
node-red -s settings.js tutorial.json 
```

Para que funcione el demo completo y los flujos de Node-RED hay que tener una cuenta en IBM Bluemix los servicios Speech2Text y VisualRecognition. Completar los flujos con sus respectivas credenciales. Ejecutar:
```bash
node-red -s settings.js demo.json 
```

Link Interfaz WEB en IBM Node-RED: [Link](https://demoiot-meetup.mybluemix.net/ui)


[s1]: https://raw.githubusercontent.com/charlielito/demoIoT/master/scheme.png "S"
