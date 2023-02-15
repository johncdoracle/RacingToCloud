# Bienvenidos a Oracle Racing To The Cloud
## Laboratorio de Container Instances
![](https://github.com/johncdoracle/RacingToCloud/blob/main/images/OCI_Container_instances.png)

#### Prerrequisitos para la realizacion del Laboratorio
* Creacion de la VCN y subredes, una publica y una privada
* Creacion de Internet Gateway y entrada en la tabla de rutas para la subred publica
* Creacion de NAT Gateway y entrada en la tabla de rutas para la subred privada
+ Configuracion de Security Lists:
  + Para la subred publica permitir el trafico por el puerto 80
  + Para la subred privada permitir todo el trafico desde la subred privada
  
# 1. Creacion de Container Instance

Menu principal >Developer Services > Container instances

![](https://github.com/johncdoracle/RacingToCloud/blob/main/images/create_container_instance.jpg)

## Configuracion de la instancia
![](https://github.com/johncdoracle/RacingToCloud/blob/main/images/create_container_instance1.jpg)

En la parte de Networking seleccionamos la VCN y la subred privada en Advance Options ingresamos una IP correspondiente al bloque de la subred privada
![](https://github.com/johncdoracle/RacingToCloud/blob/main/images/create_container_instance2.jpg)

