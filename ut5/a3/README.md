
<center>

# EJERCICIOS PACKET TRACER NIVEL DE ENLACE II


</center>

***Nombre:*** Roberto Hernández Martín
***Curso:*** 1º de Ciclo Superior de Administración de Sistemas Informáticos en Red.

### ÍNDICE

+ [Introducción](#id1)
+ [Objetivos](#id2)
+ [Material empleado](#id3)
+ [Desarrollo](#id4)
+ [Ejercicio 5](#id6)
+ [Ejercicio 6](#id7)
+ [Ejercicio 7](#id8)
+ [Conclusiones](#id5)


#### ***Introducción***. <a name="id1"></a>

Vamos a crear unos esquemas de redes en packet tracer.

#### ***Objetivos***. <a name="id2"></a>

Ver como funcionan las redes en el nivel de enlace.

#### ***Material empleado***. <a name="id3"></a>

+ Packet tracer

#### ***Desarrollo***. <a name="id4"></a>

## Ejercicio 5 <a name="id6"></a>

### Paso 1

![5.9](./img/ejercicio5/09.png)

Coloco 3 switchs 2950-24 con sus respectivos nombres y conexiones entre ellos.

### Paso 2

![5.10](./img/ejercicio5/10.png)

Coloco los 15 ordenadores con sus respectivas IP's.

### Paso 3

![5.3](./img/ejercicio5/03.png)
![5.4](./img/ejercicio5/04.png)
![5.5](./img/ejercicio5/05.png)

Aquí encima vemos una tabla con los PC's, sus respectivas Ip's y las subredes a las que pertenecen. A la derecha de la tabla se ven los PC's a los que se pueden conectar.

### Paso 4

![5.6](./img/ejercicio5/06.png)

Aqui se ven se ven las direcciones MAC.

![5.7](./img/ejercicio5/07.png)

Aquí podemos ver la tabla arp de uno de los PC's.

### Paso 5

En este paso cambio las IP's de todos los PC's para que en grupos de 5 estén dentro de la misma subred. Esto se puede ver en el archivo `ejercicio_5_ipscambiadas` subido a este repositorio.

## Ejercicio 6 <a name="id7"></a>

### Paso 1

![6.1](./img/ejercicio6/01.png)

Me conecto al switch a través de la consola del pc.

---

### Paso 2

![6.2](./img/ejercicio6/02.png)

Le cambio el nombre del switch a `Mi_primer_switch`.

---

### Paso 3

![6.3](./img/ejercicio6/03.png)

Desactivo la aparición de mensajes por consola.

---

### Paso 4

![6.4](./img/ejercicio6/04.png)

Activo la contarseña

---

### Paso 5

![6.6](./img/ejercicio6/06.png)

Configuro la ip del switch.

---

![6.7](./img/ejercicio6/07.png)

Aquí hago ping entre el PC y el Switch. En este paso tuve problemas ya que en la práctica no se menciona que hay que unirlos con un cable de cobre, y sin este paso no se puede hacer ping.

---

### Paso 6

![6.8](./img/ejercicio6/08.png)

Reincio el switch.

---

![6.9](./img/ejercicio6/09.png)

Compruebo que se borran los datos.

---

![6.10](./img/ejercicio6/10.png)

Copio running config a startup config. Y así no se borra la configuración.

---

### Paso 7

![6.11](./img/ejercicio6/11.png)

En la práctica dice que hay que escribir el comando `enable password cisco`cuando se tiene # en la terminal, pero al escribirlo yo me sale error.

---

![6.12](./img/ejercicio6/12.png)

Cambiando la contraseña y line.

---

![6.13](./img/ejercicio6/13.png)

Cuando hago el comando telnet desde el pc con la IP del switch me da error en este paso y no se llega a conectar.

---

## Ejercicio 7 <a name="id8"></a>

### Paso 1

![7.1](./img/ejercicio7/01.png)

Colocamos una tarjeta de par trenzado Gigabit en el PC.

---

![7.2](./img/ejercicio7/02.png)

Compruebo que el puerto da velocidad Gigabit.

---

![7.3](./img/ejercicio7/03.png)

Bajo la velocidad del puerto por comandos.

---

![7.4](./img/ejercicio7/04.png)

Compruebo que se ha bajado la velocidad del puerto.

---

![7.5](./img/ejercicio7/05.png)

Vuelvo a poner la velocidad en auto para que se ponga por defecto a la del puerto (Gigabit).

---

### Paso 2

![7.6](./img/ejercicio7/06.png)

Desactivo el puerto y compruebo en la interfaz gráfica que se ha dejado de tener conexión.

---

#### ***Conclusiones***. <a name="id5"></a>

En esta práctica he tenido algunas dificultades ya que ha habido algunos pasos que no he conseguido llevar a cabo, pero en general me ha quedado claro el desarrollo y no me han parecido muy dificiles los comandos utilizados.