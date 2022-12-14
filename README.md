# Flow5--NodeRed--ClimaApi
 Este repositorio contiene el flow5 realizado en NodeRed en donde se obtiene la informacion climatica por API desde openweathermap.org
 
## Introducción

En este flow se muestra un conjunto de gráficas en Dasboard, las cuales tienen como proposito reportar la información climática recibida por MQTT, la información recibida automáticamente por API.

## Material Necesario

Para realizar este flow necesitas lo siguiente

- [Ubuntu 20.04](https://releases.ubuntu.com/20.04/)
- [NodeJS](https://nodejs.org/es/)
    - [NPM](https://www.npmjs.com/)
    - [NodeRed](https://nodered.org/docs/getting-started/local)
    - [Nodos Dashboard](https://flows.nodered.org/node/node-red-dashboard)
- [Mosquitto](https://mosquitto.org/)

## Material de referencia

En los siguientes enlaces puedes encontrar cursos en la plataforma de edu.codigoiot.com que te permitirán realiar las configuraciones necesarias

- [Instalación de Virutal Box y Ubuntu 20.04](https://edu.codigoiot.com/course/view.php?id=812)
- [Instalación de NodeRed](https://edu.codigoiot.com/course/view.php?id=817)
- [Introducción a NodeRed](https://edu.codigoiot.com/course/view.php?id=278)
- [Introducción a Mosquitto](https://edu.codigoiot.com/course/view.php?id=851)

### Servicios

Para que este ejercicio funcione, necesitas los siguientes servicios
- [HiveMQ](http://www.mqtt-dashboard.com/). Es un broker publico y no se necesita cuenta
- [OpenWeatherMap](https://openweathermap.org). Servicio meteorológico gratuito. Se requiere cuenta, pero no se requiere ningun pago.
## Instrucciones
1. Obtener una cuenta de OpenWeatherMap.org
2. Clonar el Flow4 para realizar el flow5
3. Crear una nueva pestaña para el nuevo flow y reorganizar los elementos gráficos
### Requisitos previos

Para que este flow funcione, debes cumplir con los siguientes requisitos previos
1. Instalación de NodeJS. Se recomienda tener instalado NodeJS en alguna versión LTS. Al momento de creación de este documento, se usó la versión 16.17.0LTS. Esta instalación debe incluir las Build-Tools para hacer uso de NPM
2. Instalación de NodeRed. La instalación se realiza por NPM. Al momento de la creación de este contenido, se usó la versión 3.0.2
3. Instalar los nodos node-red-dashboard. Para ello, dirigete a la opcion "Manage Palet" de NodeRed y en la pestaña Install busca node-red-dashboard. Finalmente haz clic en instalar.
4. Instalación de Broker local Mosquitto MQTT.
5. Cuenta en OpenWeatherMap.org. Este es el servidor del cual se obtendrán los datos del clima por API
6. API Key valida. Deberás generar una API Key con tu cuenta de openweathermaps.org

### Instrucciones de preparación del entorno

Para ejecutar este flow, es necesario lo siguiente:
1. Arrancar NodeRed con el comando `node-red`
2. Importar el flow del repositorio.
3. Coloca tu API Key personal en la API Call del nodo HTTP Request.
4. Actualiza la IP del broker público.
5. Hacer clic en el boton Deploy.

### Instrucciones de operación

- Para observar el resutlado de este flow, abre un navegador y dirígete a localhost:1880/ui.
- Para activar las gráficas de clima manual, debes enviar por MQTT un mensaje que contenga un JSON con las variables ID, temp y hum.


## Resultados

A continuación puedes ver los nodos del flow.
![image](https://user-images.githubusercontent.com/111893490/190843807-1c878f8b-7c89-4851-803c-2e80259e50fc.png)


A continuación puede ver el tablero resultante.
![image](https://user-images.githubusercontent.com/111893490/190843962-9485a886-1b1f-4b2e-b3f4-81947dc740df.png)


## Evidencias

# Créditos

Desarrollado por David Sanchez Vazquez
- [GitHub](https://github.com/DavidSv00)
