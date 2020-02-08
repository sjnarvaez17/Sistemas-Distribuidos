# Escenario 02 

Solución del segundo taller **Sistemas Distribuidos**

## Proceso

1. **Maquina Virtual CentOS7:** Para crear la primera maquina virtual con Vagran, es necesario usar la consola de Visual Studio Code. Se unica la ruta (path) del archivo Vagranfile y mediante el comando **vagrant up** se hace efectiva la instalación de la MV en Virtual Box, usando como proovedor Vagrant

- Este es el archivo vagrant file de configuraicon inicial para nuestra maquina virtual CentOS7

  <img src ="E02/vagranfile1.JPG" height="260" >
  
- Se hace efectiva la creación de la maquina con el comando vagrant up

  <img src ="E02/vagrantup1.JPG" height="70" >
  
- Por ultimo se verifica que la maquina, efectivamente se ha creado y se puede acceder en Virtual Box

<img src ="E02/prueba1.JPG" height="260" >

2. **Acceder por SSH:** Despues de crear la MV, accedemos a ella de manera remota, para poder hacer gestion o tener acceso a la consola. Esto se logra mediante SSH y se hace efectivo con el comando **vagran ssh default** en la consola de Visual, depues de ello se veficia que ya tenemos acceso a la consola de la maquina virtual que hemos creado anteriormente.   


<img src ="E02/ssh.JPG" height="70" >
