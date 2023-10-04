<center>

# BITWARDEN COMO GESTOR DE CONTRASEÑAS Y LA 2FA


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

En esta prácica vamos a usar el gestor de contraseñas y de autenticación en dos pasos. Con esta aplicación conseguiremos almacenar de forma segura nuestras contraseñas para que nos sea más cómodo el logear en las cuentas, sin perder el factor de seguridad con ello.

#### ***Objetivos***. <a name="id2"></a>


    -Cada miembro del grupo debe usar una máquina virtual con el sistema operativo a elegir que tenga interfaz gráfica, ya que vamos a hacer uso del navegador. En dicha máquina, cada uno debe descargar la versión de  Bitwarden compatible con el sistema operativo escogido, proceder a la inslación y a la creación de una cuenta personal gratuita en la que alojar tus contraseñas.
    -Cada miembro del grupo descargará la extensión para el navegador que uses en esa máquina virtual, procediento  a la instalación y el login con la cuenta que has creado en el punto anterior.
    -Para generar los códigos del 2FA vamos a utilizar la propia app de Bitwarden, debes configurar los códigos de doble factor.
    -Configura el acceso a una cuenta Gmail y configura la “autenficación de doble factor para la misma”.
    -Para probar el acceso seguro debes logearte en la máquina virtual de tu compañero de modo que el sistema te pida el 2FA 🚨 ES IMPORTANTE NO GUARDAR LA CONTRASEÑA EN EL NAVEGADOR DE LA MÁQUINA VIRTUAL DEL COMPAÑERO DE GRUPO 🚨
    -Instala la app ( Bitwarden ) en tu teléfono móvil y úsala para logearte en la cuenta Gmail creada, comprobando que para hacerlo se use el 2FA.


#### ***Material empleado***. <a name="id3"></a>

Dos máquinas vituales de Ubuntu 20.04 y nuestros dispositivos móviles.

#### ***Desarrollo***. <a name="id4"></a>

Vamos a comenzar instalando Bitwarden mediante la terminal de la siguiente manera.
En la máquina de Bruno.

![](img/1.png)

En la máquina de Hugo.

![](img/a.png)

Entramos en bitwarden poniendo en la terminal el nombre de la aplicación.

![](img/2.png)

![](img/b.png)

Se nos pide un correo, por lo que cogemos uno ya existente.

![](img/b1.png)

Y una contraseña.

![](img/3.png)

Entramos después de esto en bitwarden.

![](img/4.png)

Ahora tenemos que añadir una extensión al navegador que vamos a usar para que se guarden nuestras contraseñas y luego podamos introducirlas rápidamente.

![](img/d.png)

Confirmamos.

![](img/5.png)

Se nos abre la siguiente pestaña.

![](img/6.png)

Ahora vamos a logearnos en Gmail para poder guardar la contraseña. Deslogueamos primero.

![](img/11.png)

Y ahora viendo que se nos ha guardado la contraseña volvemos a entrar.

![](img/12.png)

Se nos rellena clickando en la pestaña anterior.

![](img/13.png)

Para que nos pida 2FA para gmail tenemos que activar la opción de usar una aplicación externa para esto. Lo hacemos en la siguiente pestaña.

![](img/g.png)

Añadimos.

![](img/16.png)

Y probamos que funciona entrando de nuevo a la cuenta.

![](img/h1.png)

Para hacer lo mismo pero con bitwarden entramos en la sección de seguridad y activamos el 2FA.

![](img/14.png)

Vemos que se activa.

![](img/15.png)

Y nos pide de nuevo el 2FA a la hora de entrar en bitwarden.

![](img/16.png)

Entramos sin problemas a la aplicaión web.

![](img/17.png)



> ***IMPORTANTE:*** si estamos capturando una terminal no hace falta capturar todo el escritorio y es importante que se vea el nombre de usuario.

Si encontramos dificultades a la hora de realizar algún paso debemos explicar esas dificultades, que pasos hemos seguido para resolverla y los resultados obtenidos.

#### ***Conclusiones***. <a name="id5"></a>

Con esta práctica hemos aprendido a utilizar el gestor de contraseñas Bitwarden, que es muy útil a la hora de almacenar nuestras contraseñas, facilitando el acceso sin comprometer la seguridad.
