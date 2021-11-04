1. Convierte las siguientes direcciones a binario e indica si se trata de direcciones de tipo A, B o C. 

    + `10.0.3.2`
    + `128.45.7.1` 
    + `192.200.5.4` 
    + `51.23.32.50` 
    + `47.50.3.2`  
    + `100.90.80.70` 
    + `124.45.6.1` 

2. Dada la dirección de red `192.168.30.0`, indica qué máscara de subred deberías escoger para tener 4 subredes. Rellena a continuación la siguiente tabla. 

<center>

| Número de red | Dirección de subred | Primer host  | Último host  |
|---------------|---------------------|--------------|--------------|
|1              |192.168.30.0         |192.168.30.1  |192.168.30.62 |
|2              |192.168.30.64        |192.168.30.65 |192.168.30.126|
|3              |192.168.30.128       |192.168.30.129|192.168.30.190|
|4              |192.168.30.192       |192.168.30.193|192.168.30.254|


</center>

3. Dada la dirección de red `192.168.55.0`, indica qué máscara de subred deberías escoger para tener 8 subredes. Rellena a continuación la siguiente tabla.

~~~

Máscara de red: 255.255.255.0

11111111.11111111.11111111.11100000 Cojo los 3 primeros bits del último octeto para la subred.

Máscara de subred: 255.255.255.224

11000000.10101000.00110111.00000000--> 192.168.55.0

11000000.10101000.00110111.00100000--> 192.168.55.32

11000000.10101000.00110111.01000000--> 192.168.55.64

11000000.10101000.00110111.01100000--> 192.168.55.96

11000000.10101000.00110111.10000000--> 192.168.55.128

11000000.10101000.00110111.10100000--> 192.168.55.160

11000000.10101000.00110111.11000000--> 192.168.55.192

11000000.10101000.00110111.11100000--> 192.168.55.224

~~~

<center>

| Número de red | Dirección de subred | Primer host  | Último host  |
|---------------|---------------------|--------------|--------------|
|1              |192.168.55.0         |192.168.55.1  |192.168.55.30 |
|2              |192.168.55.32        |192.168.55.33 |192.168.55.62 |
|3              |192.168.55.64        |192.168.55.65 |192.168.55.94 |
|4              |192.168.55.96        |192.168.55.97 |192.168.55.126|
|5              |192.168.55.128       |192.168.55.129|192.168.55.129|
|6              |192.168.55.160       |192.168.55.161|192.168.55.161|
|7              |192.168.55.192       |192.168.55.193|192.168.55.222|
|8              |192.168.55.224       |192.168.55.225|192.168.55.254|

</center>


4. Dada la dirección de clase B `150.40.0.0`, indica qué máscara de subred deberías escoger para tener 4 subred. Rellena a continuación la siguiente tabla.

~~~

Máscara de red: 255.255.0.0

11111111.11111111.11000000.00000000 Cojo los 2 primeros bits del segundo octeto para crear la subred.

Máscara de subred: 255.255.192.0

10010110.00101000.00000000.00000000--> 150.40.0.0

10010110.00101000.01000000.00000000--> 150.40.64.0

10010110.00101000.10000000.00000000--> 150.40.128.0

10010110.00101000.11000000.00000000--> 150.40.192.0

~~~

<center>


| Número de red | Dirección de subred | Primer host | Último host  |
|---------------|---------------------|-------------|--------------|
|1               |150.40.0.0          |150.40.0.1   |150.40.63.254 |
| 2              |150.40.64.0         |150.40.64.1  |150.40.127.254|
| 3              |150.40.128.0        |150.40.128.1 |150.40.191.254|
| 4              |150.40.192.0        |150.40.192.1 |150.40.255.254|

</center>


5. ¿Cuál es el intervalo decimal y binario del primer octeto para todas las direcciones `ip` clase "B" posibles?

Desde 128 a 191 en decimal, en binario, de 10000000 hasta 10111111.

¿Qué octeto u octetos representan la parte que corresponde a la red de una dirección `ip` clase "C"?

Los 3 primeros octetos.

¿Qué octeto u octetos representan la parte que corresponde al host de una dirección `ip` clase "A"?

Los 3 últimos octetos, porque el primero es para la red.

6. Completa la siguiente tabla:

<center>


| Dirección `ip` del host | Dirección clase | Dirección de red | Dirección de host | Dirección de broadcast de red | Máscara de subred por defecto |
|-----------------------|-----------------|------------------|-------------------|-------------------------------|-------------------------------|
| 216.14.55.137         | C               |216.14.55.0       |216.14.55.137      |216.14.55.255                  |255.255.255.0                  |
| 123.1.1.15            | A               |123.0.0.0         |123.1.1.15         |123.255.255.255                |255.0.0.0                      |
| 150.127.221.224       | B               |150.127.0.0       |150.127.221.224    |150.127.255.255                |255.255.0.0                    |
| 194.125.35.199        | C               |194.125.0.0       |194.125.35.199     |                               |                               |
| 175.12.239.244        |                 |                  |                   |                               |                               |

</center>

7. Dada una dirección `142.226.0.15` :

    + ¿Cuál es el equivalente binario del segundo octeto?

        11100010

    + ¿Cuál es la Clase de la dirección?

        B

    + ¿Cuál es la dirección de red de esta dirección `ip`?

        142.226.0.0 porque se multiplica por la máscara de red 255.255.0.0

    + ¿Es ésta una dirección de host válida? ¿Por qué? o ¿Por qué no?

        Si, porque no corresponde a ninguna de las direcciones reservadas (la primera o la última).

    + ¿Cuál es la cantidad máxima de hosts que se pueden tener con una dirección de red de clase C? 

        254 porque la primera y la última dirección están reservadas. 2⁸-2=254

    + ¿Cuántas redes de clase B puede haber?

        2¹⁶= 65536. 16 porque tiene dos octetos para identificador de red.

    + ¿Cuántos hosts puede tener cada red de clase B?

        2¹⁶-2=

    + ¿Cuántos octetos hay en una dirección `ip`?

        4

    + ¿Cuántos bits puede haber por octeto?

        8


8. Determinar, para las siguientes direcciones de host `ip`, cuáles son las direcciones que son válidas para redes comerciales. Válida significa que se puede asignar a una estación de trabajo, servidor, impresora, interfaz de router, etc.

<center>

| Dirección `ip`  | ¿La dirección es válida? | ¿Por qué? |
|-----------------|--------------------------|-----------|
| 150.100.255.255 | No                         |Usa la dirección reservada para broadcast           |
| 175.100.255.18  | Si                         |           |
| 100.0.0.23      | Si                         |Es de clase A, y la dirección de host en la número 23           |
| 188.258.221.176 | No                         |La dirección de red se pasa de 255           |
| 127.34.25.189   | No                         |127 Está reservado           |
| 224.156.217.73  | No                         |224 Está reservado          |

</center>


9. Completa la siguiente tabla:

<center>


|  `ip`         | Máscara | Subred | Broadcast |
|---------------|---------|--------|-----------|
| 192.168.1.130 |         |        |           | 
| 10.1.1.3      |         |        |           |
| 10.1.1.8      |         |        |           |
| 200.1.1.23    |         |        |           |
| 172.16.8.48   |         |        |           |
| 172.16.8.48   |         |        |           |

</center>

10. Asignar direcciones `ip` válidas a las interfaces de red (interfaz de red = tarjeta de red) que les falte para conseguir que exista comunicación entre los host A, B, C, D, E y F. La máscara en todos los casos será `255.255.224.0`. Justifica la respuesta.

~~~

A: 172.33.43.5  Multiplico la dirección ip por la máscara de red

254x43= 00101011*11100000= 00100000

Hacer operación and

Dirección de subred: 172.33.32.0

Coge 3 bits, porque al pasar 254 a binario cambia 3 bits.



<center>

![](img/001.png)

</center>

11. Tu empresa tiene una dirección de red de Clase C de `200.10.57.0` .Desea subdividir la red física en 3 subredes.

    + Indica una máscara que permita dividir la red de clase C (al menos) en tres subredes.

        255.255.255.192

    + ¿Cuántos hosts (ordenadores) puede haber por subred?

        2⁶-2=62

    + ¿Cuál es la dirección de red y la dirección de broadcast de cada una de las 3 subredes creadas?

        De red: 200.10.57.0, 200.10.57.64, 200.10.57.128

        De broadcast: 200.10.57.63, 200.10.57.127, 200.10.57.127


12. Se desea subdividir la dirección de red de clase C de `200.10.57.0` en 4 subredes. Responde a las siguientes preguntas:

    + ¿Cuál es el equivalente en números binarios de la dirección de red de clase C `200.10.57.0` de este ejercicio?

        11001000.00001010.00111001.00000000

    + ¿Cuál(es) es (son) el (los) octeto(s) que representa(n) la porción de red y cuál(es) es (son) el (los) octeto(s) que representa(n) la porción de host de esta dirección de red de clase C?

        En la clase C, los primeros 3 octetos representan a la red y el último al host.

    + ¿Cuántos bits se deben pedir prestados a la porción de host de la dirección de red para poder suministrar 8 subredes?

        3, porque 2³=8

    + ¿Cuál será la máscara de subred (utilizando la notación decimal) basándose en la cantidad de bits que se pidieron prestados en el paso 3?

        255.255.255.224

    + ¿Cuál es el equivalente en números binarios de la máscara de subred a la que se hace referencia anteriormente?

        11111111.11111111.11111111.11100000

13. Teniendo en cuenta la dirección `ip` del ejercicio anterior (`200.10.57.0`) completa la siguiente tabla para cada una de las posibles subredes que se pueden crear pidiendo prestados 3 bits para subredes al cuarto octeto (octeto de host). Identifica la dirección de red, la máscara de subred, el intervalo de direcciones `ip` de host posibles para cada subred, la dirección de broadcast para cada subred.

<center>


|  Subred | Dirección de subred | Primer host      | Último host      |
|---------|---------------------|------------------|------------------|
| 1       |                     |                  |                  |
| 2       |                     |                  |                  |
| 3       |                     |                  |                  |
| 4       |                     |                  |                  |
| 5       |                     |                  |                  |
| 6       |                     |                  |                  |
| 7       |                     |                  |                  |
| 8       |                     |                  |                  |

</center>


14. Completa la siguiente tabla:

<center>


| `ip`          | Máscara         | Subred        | Broadcast     | Número hosts |
|---------------|-----------------|---------------|---------------|--------------|
| 192.168.1.130 | 255.255.255.128 | 192.168.1.128 | 192.168.1.255 | 128-2        |
| 200.1.17.15   | 255.255.255.0   | 200.1.17.0    | 200.1.17.255  |              |
| 133.32.4.61   | 255.255.255.224 |               |               | 32-2         |
| 132.4.60.99   | 255.255.0.0     |               |               |              |
| 222.43.15.41  |                 | 222.43.15.0   | 222.43.15.255 |              |
|               | 255.255.255.192 | 192.168.0.0   |               |              |

</center>

15. Responde a las siguientes preguntas:

    + Si tenemos una red `147.84.32.0` con máscara de red `255.255.255.252`, indica la dirección de broadcast, la de red y la de los posibles nodos de la red.
    + La red `192.168.0.0`, ¿de qué clase es?
    + Escribe el rango de direcciones `ip` que pertenecen a la subred definida por la dirección `140.220.15.245` con máscara `255.255.255.240`.
    + Una red de clase B en Internet tiene una máscara de subred igual a `255.255.240.0`. ¿Cuál es el máximo de nodos por subred?

16. Calcular la dirección de red y la dirección de broadcast (difusión) de las máquinas con las siguientes direcciones IP y máscaras de subred (si no se especifica, se utiliza la máscara por defecto).

    + `18.120.16.250`
    + `18.120.16.255 / 255.255.0.0`
    + `155.4.220.39`
    + `194.209.14.33`
    + `190.33.109.133 / 255.255.255.0`
    + `190.33.109.133 / 255.255.255.128`
    + `192.168.20.25 / 255.255.255.240` 
    + `192.168.20.25 / 255.255.255.192`

17. Responde a las siguientes preguntas:

    + ¿Cuántos ordenadores como máximo se pueden tener en una red de clase A?
    + ¿Cuántos ordenadores como máximo se pueden tener en una red de clase B?
    + ¿Cuántos ordenadores como máximo se pueden tener en una red de clase C?
    + En una red de clase C con máscara `255.255.255.128`, ¿cuántos ordenadores se pueden tener en cada subred?
    + En una red de clase C con máscara `255.255.255.192`, ¿cuántos ordenadores se pueden tener en cada subred?

18. Tu empresa tiene una dirección de red de Clase B de `150.10.0.0`. Desea subdividir la red física en 3 subredes.

    + Indica una máscara que permita dividir la red de clase B (al menos) en tres subredes.
    + ¿Cuántos hosts puede haber por subred?
    + ¿Cuál es la dirección de red y la dirección de broadcast de cada una de las 3 subredes creadas?

19. Dada la dirección de clase B `120.32.0.0`, indica qué máscara de subred deberías escoger para tener 4 subredes. Rellena a continuación la siguiente tabla.

<center>

| Número de red | Dirección de subred | Primer host | Último host |
|---------------|---------------------|-------------|-------------|
|               |                     |             |             |
|               |                     |             |             |
|               |                     |             |             |
|               |                     |             |             |

</center>

20. Responde a las siguientes preguntas:

    + Si tenemos una red `150.84.32.0` con máscara de red `255.255.255.224`, indica la dirección de broadcast, la de red y la de los posibles nodos de la red.
    + La red `192.168.0.0`, ¿de qué clase es?
    + Escribe el rango de direcciones `ip` que pertenecen a la subred definida por la dirección  `150.84.32.245` con máscara `255.255.255.240`.
    + Una red de clase B en Internet tiene una máscara de subred igual a `255.255.240.0`. ¿Cuál es el máximo de nodos por subred?

