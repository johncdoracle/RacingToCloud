# Bienvenidos a Oracle Racing To The Cloud
## Laboratorio de Container Instances
![](https://github.com/johncdoracle/RacingToCloud/blob/main/images/OCI_Container_instances.png)

#### Prerrequisitos para la realizacion del Laboratorio
* Creacion de la VCN y subredes, una publica y una privada
* Creacion de Internet Gateway y entrada en la tabla de rutas para la subred publica
* Creacion de NAT Gateway y entrada en la tabla de rutas para la subred privada
+ Configuracion de Security Lists:
  + Para la subred publica permitir el trafico por el puerto 80
  + Para la subred privada permitir todo el trafico desde la subred publica
  
# 1. Creación de Container Instance

### Menu principal >Developer Services > Container instances

![](https://github.com/johncdoracle/RacingToCloud/blob/main/images/create_container_instance.jpg)

## Configuración de la instancia
Debemos ingresar la informacion del nombre de la instancia, AD, Shape y capacidades de computo(OCPU y Memoria RAM)

![](https://github.com/johncdoracle/RacingToCloud/blob/main/images/create_container_instance1.jpg)

En la parte de Networking seleccionamos la VCN y la subred privada, luego, desplegamos Advance Options e ingresamos una IP correspondiente al bloque de la subred privada
![](https://github.com/johncdoracle/RacingToCloud/blob/main/images/create_container_instance2.jpg)

### Configuración de los contenedores
En esta parte vamos a asignar el/los nombres de los contenedores, seleccionamos la/las imagenes a utilizar y creamos las variables de ambiente que necesita el contenedor para funcionar adecuadamente. Para el laboratorio vamos a utilizar las imagenes publicas del Docker Hub
![](https://github.com/johncdoracle/RacingToCloud/blob/main/images/create_container_1.jpg)




