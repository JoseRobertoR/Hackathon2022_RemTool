# Logicalis - Remediation Tool

[Back](PF1.md) - [Home](../README.md)

# Posta extra 2 - Remediar interfaz
## Objetivo
Para esta posta debemos escribir un código en python 'posta_8.py' que se conecte la interfaz Eth1/11 del laboratorio, guardando el estado de la misma cada vez que haga un cambio mientras se ejecuta mi codigo en un archivo 'root/output/posta_8.txt'.

Si el estado de la interfaz no es 'up' ejecutar los comandos 'int eth1/11' y 'no shut', siguiendo la estructura de logging y aviso por mail de las anteriores etapas.

> Device_type = "cisco_xe"
> Host = "10.54.100.248"
> Username = "admin"
> Password = "cisco123"

## Contexto
Un caso de automatizacion de networking puede ser este, en el cual tengo una interfaz de red de un equipo Nexus el cual necesito que este siempre 'up', por lo que le hago un seguimiento continuo para mantenerlo en este estado.

## Validación
Generar archivo 'root/output/posta_8.txt' con los cambios de estado de la interfaz, generar el archivo HT22.log y enviar mail.

[Back](PF1.md) - [Home](../README.md)
