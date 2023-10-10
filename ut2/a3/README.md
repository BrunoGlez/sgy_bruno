<center>

# GPG


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

En esta práctica vamos a hacer uso de la herramienta de cifrado GPG en una máquina Linux.

#### ***Objetivos***. <a name="id2"></a>

El objetivo es generar una clave que se compartirá con nuestro compañero y viceversa. De esta manera, si nosotros le enviámos un mensaje cifrado, él es capaz de verlo al tener nuestra clave. Lo mismo pasaría si el que envía el mensaje es la otra persona.

#### ***Material empleado***. <a name="id3"></a>

Dos máquinas virtuales Ubuntu 20.04.

#### ***Desarrollo***. <a name="id4"></a>

Lo primero que tenemos que hacer es generar la clave que luego vamos a compartir con nuestro compañero. Esto se hace con el siguiente comando.

![](img/1.png)

Las genera Hugo

![](img/01.png)

Nos pide que le asignemos una contraseña para proteger nuestra nueva clave. Como esto es una práctica, creo una contraseña fácil de recordar.

![](img/2.png)

Vemos la nueva clave que hemos creado.

![](img/4.png)

La de Hugo.

Hacemos cat para ver la clave completa. Es la siguiente.

![](img/7.png)

![](img/03.png)

Nuestro compañero nos tiene que pasar su clave, que ha generado con el mismo procedimiento que nosotros. El proceso para importar esta clave es el siguiente.

![](img/8.png)

Se importa la clave en el PC de Hugo.

![](img/05.png)

Para comprobar que se encriptan correctamente los mensajes, vamos a crear un archivo llamado "hola" con un mensaje aleatorio dentro, en este caso "hola". Luego encriptamos con el siguiente comando.

![](img/9.png)

Se nos crea un nuevo archivo, pero con extensión distinta, en este caso .asc. Si abrimos el mensaje vemos el mensaje encriptado.

![](img/10.png)

Al hacer el desencriptado nos pide la contraseña.

![](img/11.png)

Y vemos que se desencripta.

![](img/12.png)

Y leemos el archivo mediante la interfaz gráfica.

![](img/13.png)

Hugo hace el mismo proceso que el anterior pero con el archivo que le paso yo.

![](img/H10.png)

> ***IMPORTANTE:*** si estamos capturando una terminal no hace falta capturar todo el escritorio y es importante que se vea el nombre de usuario.

Si encontramos dificultades a la hora de realizar algún paso debemos explicar esas dificultades, que pasos hemos seguido para resolverla y los resultados obtenidos.

#### ***Conclusiones***. <a name="id5"></a>

Hemos aprendido a usar la herramienta GPG para encriptar mensajes entre equipos.