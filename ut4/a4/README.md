<center>

# TÍTULO DE LA PRÁCTICA


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

-   Instalar y configurar pfsense
-   Configurar wifiradius


#### ***Material empleado***. <a name="id3"></a>

-   Una MV Ubuntu (servidor)
-   Una MV Windows (cliente) 

#### ***Desarrollo***. <a name="id4"></a>

Necesitaremos dos interfaces de red en nuestra MV servidor.

![](img/1.png)

![](img/2.png)

Metemos la ISO de pfsense.

![](img/3.png)

Comenzamos con la instalación usando la interfaz de pfsense.

![](img/4.png)

Finalizamos la instalación y nos recibe el menú de pfsense.

![](img/5.png)

Se nos abre el menú en la terminal donde nos da la IP que tendremos que usar.

![](img/6.png)

Vamos a asignar una IP estática dentro de la misma red. Más tarde lo cambiaremos a DHCP.

![](img/7.png)

Si entramos en la IP vía navegador nos abrirá el inicio de sesión de pfsense.

![](img/8.png)

Entramos usando "admin" y "pfsense" como usuario y contraseña, respectivamente.

![](img/9.png)

Configuramos el nombre del host y el dominio.

![](img/10.png)

Configuramos la interfaz WAN para que sea DHCP.

![](img/11.png)

Y la interfaz LAN la vamos a configurar con la IP siguiente, con su respectiva máscara de red.

![](img/12.png)

Hecho esto, nos recibe el "Dashboard" de pfsense.

![](img/13.png)

Tendremos que habilitar el DHCP en la interfaz LAN.

![](img/14.png)

Comprobamos ahora que nos ha dado la IP el servicio DHCP. Esta tiene que estar dentro de un rango especificado.

![](img/15.png)

Buscamos ahora freeradius para añadirlo a la pestaña de servicios.

![](img/16.png)

Editamos la configuración de las interfaces.

![](img/17.png)

![](img/18.png)

![](img/19.png)

Añadimos dos usuarios nuevos. Uno se llamará alumno y otro se llamará bruno.

![](img/20.png)

Habilitamos la autenticación MAC y deshabilitamos "Acct_Unique".

![](img/21.png)

Tenemos esto configurado. Ahora vamos a especificarle a pfsense que use la interfaz LAN, que es la que tenemos configurada para esto.

![](img/22.png)

Ahora tendremos que asignar el server de autenticación. No lo hemos creado, por lo que de momento lo dejamos así.

![](img/23.png)

Ahora creamos lo anterior, con los siguientes datos.

![](img/24.png)

Con esto creado, ahora vamos a asignar esto en la página anterior.

![](img/25.png)

Ya tendríamos todo configurado.

#### ***Conclusiones***. <a name="id5"></a>

Hemos aprendido a configurar pfsense para que nos brinde servicios de enrutamiento y firewall.