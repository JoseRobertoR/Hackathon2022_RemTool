# Hackathon2022_RemTool

En este Hackathon buscamos reforzar conceptos y practicar en la escritura de codigo en Python enfocado en automatización.

Para esto se les pedirá completar 6 postas basicas y 2 finales, las cuales son individuales pero complementarias, por lo que se debe escribir un codigo individual para cada una de las posta, pero puede llegar a necesitarse lo escrito en alguna anterior.

> Por ejemplo, yo terminé de escribir mis archivos **posta_1.py** y **posta_2.py** los cuales funcionaron correctamente y debo escribir **posta_3.py** el cual integra lo realizado en **posta_1.py** y **posta_2.py**, entonces genero el nuevo archivo **posta_3.py** y agrego en este el contenido de **posta_1.py** y **posta_2.py** para utilizarlo nuevamente.

> Otro ejemplo, yo terminé de escribir mis archivos **posta_1.py** y **posta_2.py** los cuales funcionaron correctamente y debo escribir **posta_3.py** el cual integra lo realizado en **posta_1.py** y **posta_2.py**. Modifico **posta_1.py** y **posta_2.py** para poder usar parte de su codigo como funciones que puedo importar desde **posta_3.py** y reutilizalo.

Por lo que si se completan TODAS las posta de este Hackathon se deben tener (como minimo) 8 archivos **'posta_n.py** (siendo 'n' el numero de posta) en 'HT22_Remediation'

## Infraestructura 

<p align="center">
  <img src="Postas/Infra.png" alt="Infraestructura Hackathon"/>
</p>

La infra consiste en 2 VM's alojadas en la misma red y con una concexión SSH pre-configurada, las cuales 'HT22_Monitoring' tiene hosteado a travez de **Docker** un contenedor por cada grupo con el nombre **'grupo_n'** (siendo 'n' el numero del grupo) el cual se encuentra inicialmente *detenido* y 'HT22_Remediation' contiene **Python 3.7** para poder ejecutar nuestros scripts.

En este ultimo 'HT22_Remediation' es en el cual nosotros debemos trabajar, escribiendo nuestros codigos y generando nuestros directorios de trabajo.

> Se le proporcionará a cada grupo la IP, User y Password de 'HT22_Remediation', y la IP y User de 'HT22_Monitoring' para que puedan trabajar.
>
> HT22_Monitoring:
> - IP = 10.54.118.8
> - USER = root
>
> HT22_Remediation:
> - Conexión = ssh -p 55522 h2022-grpNN@190.111.211.46

## Comandos Linux utiles
No es obligatorio el conocimiento profundo de manejo de CLI Linux ya que ejecutaremos tareas basicas.

- Listar archivos
~~~bash
>>> ls
~~~
- Listar archivos (ocultos tambien)
~~~bash
>>> ls -a
~~~
- Moverse entre directorios
~~~bash
>>> cd <nombre_carpeta>
~~~
- Moverse al directorio root
~~~bash
>>> cd ~
~~~
- Crear directorio
~~~bash
>>> mkdir <nombre_carpeta>
~~~
- Crear archivo
~~~bash
>>> nano <nombre_archivo>
~~~
~~~bash
>>> vim <nombre_archivo>
~~~
- Ver contenido archivo
~~~bash
>>> cat <nombre_archivo>
~~~
- Ejecutar script python3
~~~bash
>>> python3 <nombre_archivo>.py
~~~
- Descargar libreria python3
~~~bash
>>> pip3 <nombre_libreria>
~~~

## Objetivo final
Escribir un código en Python para validar el estado de un contenedor en otra VM de forma automática. Si el estado NO es ‘running’ ejecutar una remediación automática, enviando luego un mail y guardando un log con el estado en el cual se encuentra

### Postas
- Posta 1 – [Obtener JSON](Postas/P1.md)
- Posta 2 – [Conexión SSH](Postas/P2.md)
- Posta 3 – [Logging](Postas/P3.md)
- Posta 4 – [Enviar comandos](Postas/P4.md)
- Posta 5 – [Remediacion continua](Postas/P5.md)
- Posta 6 – [Enviar mail](Postas/P6.md)

### Postas Finales
- PF 1 – [Variables Externas](Postas/PF1.md)
- PF 2 – [Remediar interfaz](Postas/PF2.md)

## Validación de las etapas
Se le pedirá que guarde, desde el programa, el output del código en un directorio previamente creado (‘$HOME/output/’) con el nombre ‘posta_n.txt’ (siendo 'n' el numero de posta)
