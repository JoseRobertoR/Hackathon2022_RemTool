# Logicalis - Remediation Tool

[Home](../README.md) - [Next](PF2.md)

# Posta extra 1 - Variables Externas
## Objetivo
Para esta posta debemos escribir un código en python 'posta_7.py' que integre todo lo resuelto en las postas anteriores, pero que las variables 
- MonitoringIP
- MonitoringUser
- PrivateKeyPath
- ContainerName

Las tome desde fuera del codigo como variables externas

> Esto quiere decir, que yo deberia pasarle estas variables una vez ejecute el codigo desde la linea de comandos:
> ~~~bash
> python3 posta_7.py <MonitoringIP> <MonitoringUser> <PrivateKeyPath> <ContainerName>
> ~~~

## Contexto
Lo que no podemos negar es la comodidad de trabajar con una variable global hard-codeada dentro del código representando una IP o una dirección dentro de mi proyecto, pero la realidad es que esto una vez que nuestro proyecto se encuentra en producción no sucede. 
  
Por esto mismo debemos aprender a tomar estas variables hard-codeadas como variables que me pasan de manera externa a mi programa, acotando lo mas posible la utilización de estas, haciendo a nuestro código lo mas flexible posible.

## Validación
Ejecución correcta del código posta_7.py enviandole variables externas.


[Home](../README.md) - [Next](PF2.md)
