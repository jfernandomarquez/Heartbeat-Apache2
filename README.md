# Configuración de Heartbeat con Apache2

Se presenta una configuración de heartbeat para tener una pagina web en alta disponibilidad.  

## Prerequisitos 

* Tres maquinas virtual linux en VirtualBox: Dos ubuntu-server y una ubuntu-desktop
* Instalar apache2 y modificar los index.html de tal manera que permita identificar en que servidor esta mostrando la pagina web.

[![index](https://github.com/jfernandomarquez/Heartbeat-Apache2/blob/master/index.png)](https://jfernandomarquez.blogspot.com/) 

## Topología

[![config](https://github.com/jfernandomarquez/Heartbeat-Apache2/blob/master/topologia.png
)](https://jfernandomarquez.blogspot.com/) 


## Configuración 

En ambos servidores se debe configuras los archivos que se ven en la siguiente imagen.

[![config](https://github.com/jfernandomarquez/Heartbeat-Apache2/blob/master/configuraci%C3%B3n-heartbeat.png)](https://jfernandomarquez.blogspot.com/) 


## Prueba

Para probarlo se debe consultar la pagina web y verificar que se muestre la página del servidor primario(nodo1) y al detener heartbeat en dicho servidor se debe observar el cambio  la página del servidor secundario (nodo2)

## Referencias

https://www.youtube.com/watch?v=gjTNFxj06qU
