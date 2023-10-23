<center>

# Clonación de discos mediante Clonezilla


</center>

***Nombre:Bruno Amancio González Gorrín y Hugo Suárez Pérez***
***Curso:*** 2º de Ciclo Superior de Administración de Sistemas Informáticos en Red.

### ÍNDICE

+ [Introducción](#id1)
+ [Objetivos](#id2)
+ [Material empleado](#id3)
+ [Desarrollo](#id4)
+ [Conclusiones](#id5)


#### ***Introducción***. <a name="id1"></a>

En esta práctica vamos a usar la herramienta de clonación de discos y particiones de Clonezilla.

#### ***Objetivos***. <a name="id2"></a>



+Probar Clonezilla cliente para clonar una partición en otra partición. Para ello utilizaremos máquinas virtuales y añadiremos un segundo disco duro a una máquina existente.

+Probar clonezilla con un servidor SSH y con otro SMB.

#### ***Material empleado***. <a name="id3"></a>

Dos MV Ubuntu 20.04.

#### ***Desarrollo***. <a name="id4"></a>

Partimos de unas máquinas Ubuntu ya creadas, por tanto no vamos a mostrar nada de la configuración.

Para comenzar, añadimos un disco extra.

![](img/1.png)

Para usar Clonezilla, tenemos que usar la ISO y arrancar la MV con ella, de la siguiente manera.

![](img/2.png)

Vemos el disco nuevo que añadimos.

![](img/3.png)

En la MV de Hugo:

![](img2/01.png)

Para montar y poder clonar el disco, tenemos que usar Gparted. No es obligatorio, pero es más cómodo hacerlo de esta manera.

![](img/5.png)

Entramos.

![](img/6.png)

Tenemos que añadir un usuario nuevo llamado mantenimiento.

![](img2/03.png)

Hacemos la partición correspondiente (extendida), y luego apagamos la MV y lanzamos Clonezilla.

![](img/7.png)

Nos recibe la siguiente pestaña, donde pulsamos Iniciar.

![](img/8.png)

Hacemos de partición a partición, ya que no queremos clonar el disco completo.

![](img/9.png)

De local a local.

![](img/10.png)

Aquí elegimos el disco origen.

![](img/11.png)

Y en la siguiente página elegimos el disco destino, es decir, donde vamos a clonar el disco origen.

![](img/12.png)

Continuamos y comienza la clonación.

![](img/13.png)

![](img/14.png)

Vamos a intentar ahora botear desde la partición clonada. En esta pantalla apretamos el 3.

![](img2/17.png)

Vemos que se inicia el SO de manera correcta, tal como se iniciaría con el disco origen.

![](img2/18.png)

Ya que hemos logrado clonar localmente de manera correcta, ahora vamos a hacerlo vía SSH, es decir, de máquina remota a máquina remota.

La forma de proceder es similar. Entramos en Clonezilla y elegimos ssh_server.

![](img/16.png)

En la página siguiente se tendría que añadir la dirección IP de la máquina a la que queremos clonar el disco.

![](img/17.png)

Nos pide otras cosas, como máscara, servidor DNS y el disco que queremos clonar. Usamos el mismo que antes.
Iniciamos la clonación.

![](img/18.png)

Es importante que nuestro compañero tenga creada una carpeta llamada partimag, que es donde se nos guardará la clonación.

![](img2/19.png)

Se nos inicia sin problemas la clonación.

![](img2/aaaa.png)


> ***IMPORTANTE:*** si estamos capturando una terminal no hace falta capturar todo el escritorio y es importante que se vea el nombre de usuario.

Si encontramos dificultades a la hora de realizar algún paso debemos explicar esas dificultades, que pasos hemos seguido para resolverla y los resultados obtenidos.

#### ***Conclusiones***. <a name="id5"></a>

Hemos aprendido a usar la herramienta de clonado de discos y particiones Clonezilla, tanto de forma local (de disco a disco) como de manera remota (de máquina a máquina).