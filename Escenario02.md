# Escenario 02 

Solución del segundo taller **Sistemas Distribuidos**

## Proceso

1. **Maquina Virtual CentOS7:** Para crear la primera maquina virtual con Vagran, es necesario usar la consola de Visual Studio Code. Se unica la ruta (path) del archivo Vagranfile y mediante el comando **vagrant up** se hace efectiva la instalación de la MV en Virtual Box, usando como proovedor **Virtual Box.**

- Este es el archivo vagrant file de configuraicon inicial para nuestra maquina virtual CentOS7

  <img src ="E02/vagranfile1.JPG" height="280" >
  
- Se hace efectiva la creación de la maquina con el comando vagrant up

  <img src ="E02/vagrantup1.JPG" height="70" >
  
- Por ultimo se verifica que la maquina, efectivamente se ha creado y se puede acceder en Virtual Box

<img src ="E02/prueba1.JPG" height="240" >

2. **Acceder por SSH:** Despues de crear la MV, accedemos a ella de manera remota, para poder hacer gestion o tener acceso a la consola. Esto se logra mediante SSH y se hace efectivo con el comando **vagran ssh default** en la consola de Visual, depues de ello se veficia que ya tenemos acceso a la consola de la maquina virtual que hemos creado anteriormente.   


<img src ="E02/ssh.JPG" height="60" >


3. **Destruir un servidor y construir:** Para destruir una MV , se usa el comando **Vagrant destroy** , este detiene la maquina en ejecuccion y destruye todos los recursos y procesos que se crearon durante su ejecucción. Dejando la maquina host como si nunca hubiese creado nunca la maquina virtual. Sin embargo la caja que contiene la imagen de la MV seguira instalada en el host.


  <img src ="E02/destroy.JPG" height="50" >
   
- Se evidencia que la maquina virtual ha sido destruida y no se encuentra en ejecucción.

  <img src ="E02/destruida.JPG" height="90" >
  
- Con el comando **vagrant up** es posible reconstruir la MV y se evidencia con el comando **vagrant status**

  <img src ="E02/reconstruida.JPG" height="90" >


4. **Crear dos servidores:** El siguiente paso es crear dos servidores virtuales, usando la herramienta Vagrant, que permite automatizar el proceso, y mediante un script crear las dos maquinas virtuales, con su configuración inicial. Para ello es necesario un archivo Vagrant file que se ejecute en la consola de Visual.


- Este es el archivo vagrant file de configuracion inicial, para la creacion de los dos servidores.

<img src ="E02/vagranfile2.JPG" height="280" >

- Con el comando **vagrant status** , se evidencia que los dos servidoreshan sido creados y se encuentran corriendo.

<img src ="E02/prueba2.JPG" height="80" >

- Igualmente se puede evidenciar que las maquinas efectivamente han sido creadas en Virtual Box


<img src ="E02/prueba3.JPG" height="220" >


5. **Aprovisionamiento de los servidores:** Utilizando Ansible se pueden aprovisionar las maquinas virtuales de manera automatizada mendiante scripts que permiten hacer la gestion de las aplicaciones o servidios que se instalan en las maquinas.


