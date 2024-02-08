<center>

# CONFIGURACIÓN DE UN PROXY USANDO PFSENSE


</center>

***Nombre: Bruno Amancio González Gorrín***
***Curso:*** 2º de Ciclo Superior de Administración de Sistemas Informáticos en Red.

### ÍNDICE

+ [Introducción](#id1)
+ [Objetivos](#id2)
+ [Material empleado](#id3)
+ [Desarrollo](#id4)
+ [Conclusiones](#id5)


#### ***Introducción***. <a name="id1"></a>

pfSense1​ es una distribución personalizada de FreeBSD adaptado para su uso como Firewall y Enrutador. Se caracteriza por ser de código abierto, puede ser instalado en una gran variedad de ordenadores, y además cuenta con una interfaz web sencilla para su configuración.

#### ***Objetivos***. <a name="id2"></a>

- El objetivo de esta práctica es montar un servidor proxy sobre PFSense que nos va a permitir conectarnos desde Internet a nuestra red local desde prácticamente cualquier dispositivo que soporte VPNs. Para ello en el servidor vamos a instalar y configurar pptpd que es un servidor de protocolo PPTP.

- La VPN que vamos a montar será una VPN de acceso remoto y va a permitir que clientes desde sitios remotos se puedan conectar a nuestra red local y trabajar como si estuvieran en la misma red.


#### ***Material empleado***. <a name="id3"></a>

- Una máquina virtual Ubuntu que actuará de servidor.

- Una máquina virtual de Ubuntu que actuará de cliente.

#### ***Desarrollo***. <a name="id4"></a>

Lo primero que tenemos que hacer es instalar los paquetes necesarios usando el instalador de paquetes -->

![](img/1.png)

Luego tenemos que borrar los servidores DNS o gateways que tengamos.

![](img/2.png)

Entramos al portal cautivo.

![](img/3.png)

Una vez nos hemos verificado, tenemos que activar el proxy con la IP de nuestro servidor. Esto lo hacemos desde el cliente -->

![](img/4.png)

Ahora vamos a instalar el paquete SquidGuard, del cual ya tenemos las dependencias, que hemos intalado en los pasos anteriores. Usaremos el instalador de paquetes -->

![](img/5.png)

Ahora, si queremos añadir una blacklist o lista negra, tendremos que dirigirnos al menú de SquidGuard y la añadiremos aquí. Se nos descargará.

![](img/6.png)

![](img/7.png)

#### ***Conclusiones***. <a name="id5"></a>

Hemos aprendido a configurar un proxy usando PFSense, además de añadir listas negras para evitar que se puedan acceder a las páginas que estas contienen.