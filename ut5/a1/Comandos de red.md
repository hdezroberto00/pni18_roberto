
<center>

# TÍTULO DE LA PRÁCTICA


</center>

***Nombre:***
***Curso:*** 2º de Ciclo Superior de Administración de Sistemas Informáticos en Red.

### ÍNDICE

+ [Introducción](#id1)
+ [Objetivos](#id2)
+ [Material empleado](#id3)
+ [Desarrollo](#id4)
+ [Conclusiones](#id5)


#### ***Introducción***. <a name="id1"></a>

Aquí explicamos brevemente la parte teórica que tiene que ver con la práctica que se va a realizar

#### ***Objetivos***. <a name="id2"></a>

Voy a aprender algunos comandos importantes para administrar una red. Más importantes que saber atarse los zapatos.

#### ***Material empleado***. <a name="id3"></a>

Usaré para la parte de windows mi máquina real y para la parte de linux una máquina virtual en VirtualBox. 

#### ***Desarrollo***. <a name="id4"></a>

## Comando	ipconfig	(Windows)

|                              |                                              |
|------------------------------|----------------------------------------------|
| Dirección IP v4              | 172.18.99.160                                 |
| Máscara                      | 255.255.0.0                                  |
| Gateway                      | 172.18.0.1                                   |
| MAC                          | 08-00-27-69-C6-B9                            |
| Fabricante                   | Cadmus Computer Systems                      |
| Dirección IP v6              | fe80::5191:fa13:9f08:28ed                    |
| Servidores DNS               | 80.58.61.250                                 |
| Tiempo de concesión de la IP | jueves 10 febrero - viernes 11 de febrero    |
| Nombre del adaptador de red  | Intel(R) PRO/1000 MT Desktop Adapter         |

Haciendo uso del comando `ipconfig /all` saco toda esta información desde el powershell de windows.

<img source="./img/1">

---

### Liberar la configuración IP del adaptador con ipconfig /release y a continuación volver a usar el comando ipconfig. ¿Cuál es la ip ahora?

No hay ip.

![02]()

---

### Ejecutar el comando ipconfig /renew solicitando una renovación de dirección IP. A continuación volver a ejecutar ipconfig. ¿Cuál es la nueva ip?

La ip es la misma.

![03]()

---

### Ejecutar el comando ipconfig /displaydns y comprobar la información que contiene la caché DNS de tu equipo. Ejecuta ahora el comando ipconfig /flushdns y después muestra otra vez el contenido de la caché DNS. ¿Qué información muestra ahora? ¿Qué ha ocurrido?

![04]()

Se muestra la caché de la DNS.

![05]()

Por el uso del comando `ipconfig /flushdns`se muestra vacía la caché de la DNS.

---

### Usar el navegador para ir a la web http://www.iespuertodelacruz.es y luego ejecutar el comando ipconfig /displaydns. Hacer una captura de pantalla donde se muestre que se ha cacheado la ip de ese nombre de dominio y pegarla aquí debajo.

![06]()

---

### Borra la caché DNS con el comando ipconfig /flushdns y muestra una captura de pantalla en que se vea que ya no hay registros DNS en caché.

![07]()

---

## Comando	ifconfig	(Línux)

¿?

---

### Desactiva tu tarjeta de red con el comando ifconfig eth0 down. A continuación, comprueba con un ifconfig que la tarjeta ya no aparece, se ha desactivado. Haz una captura de pantalla donde se vea que ya no está activada.

¿?

---

### Usa el comando ifconfig –a para ver que la tarjeta está desactivada, pero nadie la ha robado. Sigue ahí. Ahora activa la tarjeta con el comando ifconfig eth0 up y luego con el comando ifconfig comprueba que ya está habilitada.

¿?

---

### Usa el comando ifconfig eth0 192.168.99.99 netmask 255.255.255.0 y pega una captura de pantalla que muestre que el adaptador de red se ha configurado correctamente.

¿?

---

### Usa el comando ifconfig eth0 IP netmask Máscara (con la configuración inicial de red) y pega una captura de pantalla que muestre que el adaptador de red se ha configurado correctamente.

¿?

---


#### ***Conclusiones***. <a name="id5"></a>

En esta parte debemos exponer las conclusiones que sacamos del desarrollo de la prácica.