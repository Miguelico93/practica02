# Practica02

# Vagrant 

## ¿Como creamos una maquina virtual en vagrant?

Para crear una maquina con vagrant lo primero que tendremos que hacer sera crear un directorio en el 
cual almacenemos los diferentes archivos de configuracion de nuestra maquina, emplearemos los siguientes 
comandos en la consola:

``` mkdir vagrant_getting_started ```

``` cd vagrant_getting_started ```

Dentro del directorio que hemos creado tendremos un archivo que se llama vagrantfile.

``` vagrant init ```

Este archivo es un archivo de texto el cual modificaremos en nuestro caso con visual studio code y estara escrito con el idioma de
programación Ruby.

En el siguiente espacio seleccionaremos el sistema operativo que queremos instalar, que en nuestro caso sera un ubuntu server.
El box que vamos a emplear se llama ubuntu/bionic64 que esta en la pagina de vagrant y el tipo de red que emplearemos ser ''private-network''
y le pondremos la ip de forma manual.

Por ultimo vamos a determinar que los script que queremos que se ejecuten en la postinstalación vengan del archivo de ''script.sh''

En este script vamos a determinar los comando para poder instalar automaticamente desde la instalación los programas que vamos a meter dentro de nuestro sistema.

## comandos que vamos a emplear para tener una buena utilizacion de vagrant:

Para arrancar la paquina emplearemos el siguiente comando:
```vagrant up```

Para meternos en la maquina conectaremos a ella por ssh con el siguiente comando:
```vagrant ssh```

Este comando nos vale para parar la maquina:
```vagrant halt```

Para que ejecute la parte de los script que hemos modificado sin para la maquina emplearemos el siguiente comando:
```vagrant provision```

Y por ultimo para destruir/desinstalar la maquina que hemos empleado utilizaremos el siguiente comando:
```vagrant destroy```
