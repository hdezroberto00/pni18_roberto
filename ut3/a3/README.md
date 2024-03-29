1. Convierte las siguientes direcciones a binario e indica si se trata de direcciones de tipo A, B o C. 

    + `10.0.3.2` = 00001010.00000000.00000011.00000010 Clase A
    + `128.45.7.1` = 10000000.00101101.00000111.00000001 Clase B
    + `192.200.5.4` = 11000000.11001000.00000101.00000100 Clase C
    + `51.23.32.50` = 00110011.00010111.00100000.00110010 Clase A
    + `47.50.3.2`  = 00101111.00110010.00000011.00000010 Clase A
    + `100.90.80.70` = 01100100.01011010.01010000.01000110 Clase A
    + `124.45.6.1` = 01111100.00101101.00000110.00000001 Clase A

2. Dada la dirección de red `192.168.30.0`, indica qué máscara de subred deberías escoger para tener 4 subredes. Rellena a continuación la siguiente tabla. 

Para tener 4 subredes necesito 2^2, por lo tanto cogería los 2 primeros bits del último octeto que es el que define al host.

Por lo tanto, 11111111.11111111.11111111.11000000 Esto pasado a decimal sería: 255.255.255.192

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
|5              |192.168.55.128       |192.168.55.129|192.168.55.158|
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
|2              |150.40.64.0         |150.40.64.1  |150.40.127.254|
|3              |150.40.128.0        |150.40.128.1 |150.40.191.254|
|4              |150.40.192.0        |150.40.192.1 |150.40.255.254|

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
| 194.125.35.199        | C               |194.125.0.0       |194.125.35.199     |194.125.35.255                 |255.255.255.0                  |
| 175.12.239.244        | B               |175.12.0.0        |175.12.239.244     |175.12.255.255                 |255.255.0.0                    |

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
| 150.100.255.255 | No                       |Usa la dirección reservada para broadcast           |
| 175.100.255.18  | Si                       |Porque es clase B, que se usa para redes comerciales           |
| 100.0.0.23      | Si                       |Es de clase A, y la dirección de host en la número 23           |
| 188.258.221.176 | No                       |La dirección de red se pasa de 255           |
| 127.34.25.189   | No                       |127 Está reservado           |
| 224.156.217.73  | No                       |224 Está reservado          |

</center>


9. Completa la siguiente tabla:

<center>

| ip           | Máscara         | Subred        | Broadcast     |
|--------------|-----------------|---------------|---------------|
| 192.168.1.30 | 255.255.255.128 | 192.168.1.128 | 192.168.1.255 |
| 10.1.1.3     | 255.255.0.0     |**10.1.0.0**   | 10.1.255.255  |
| 10.1.1.8     |`255.255.0.0`    | 10.1.0.0      | 10.1.255.255  |
| 220.1.1.23   | 255.0.0.0       |**220.0.0.0**  |**220.255.255.255**|
| 172.168.8.48 | 255.255.248.0   |**172.168.8.0**|**172.168.15.255**|
| 172.16.8.48  | 255.255.255.224 |**172.16.8.32**|`172.16.8.63`  |

~~~

Subred nº2: Operación `and` entre ip y máscara: 00001010.00000001.00000001.00000011
                                                11111111.11111111.00000000.00000000
                                            =   00001010.00000001.00000000.00000000= 10.1.0.0

Subred nº4: Operación `and` entre ip y máscara: 11011100.00000001.00000001.00010111
                                                11111111.00000000.00000000.00000000
                                            =   11011100.00000000.00000000.00000000= 220.0.0.0

Subred nº5: Operación `and` entre ip y máscara: 10101100.10101000.00001000.00110000
                                                11111111.11111111.11111000.00000000
                                            =   10101100.10101000.00001000.00000000= 172.168.8.0

Subred nº6: Operación `and` entre ip y máscara: 10101100.00010000.00001000.00110000
                                                11111111.11111111.11111111.11100000
                                            =   10101100.00010000.00001000.00100000= 172.16.8.32

~~~                               

</center>

10. Asignar direcciones `ip` válidas a las interfaces de red (interfaz de red = tarjeta de red) que les falte para conseguir que exista comunicación entre los host A, B, C, D, E y F. La máscara en todos los casos será `255.255.224.0`. Justifica la respuesta.

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

~~~

Máscara de red: 255.255.255.0

Máscara de subred: 255.255.255.224

Dirección de red (multiplicando máscara de red por ip): 255.255.255.0

11001000.00001010.00111001.00000000-> 200.10.57.0

11001000.00001010.00111001.00100000-> 200.10.57.32

11001000.00001010.00111001.01000000-> 200.10.57.64

11001000.00001010.00111001.01100000-> 200.10.57.96

11001000.00001010.00111001.10000000-> 200.10.57.128

11001000.00001010.00111001.10100000-> 200.10.57.160

11001000.00001010.00111001.11000000-> 200.10.57.192

11001000.00001010.00111001.11100000-> 200.10.57.224

~~~

<center>


|  Subred | Dirección de subred | Primer host      | Último host      | Dirección de Broadcast |
|---------|---------------------|------------------|------------------|------------------------|
| 1       |200.10.57.0          |200.10.57.1       |200.10.57.30      |200.10.57.31|
| 2       |200.10.57.32         |200.10.57.33      |200.10.57.62      |200.10.57.63|
| 3       |200.10.57.64         |200.10.57.65      |200.10.57.94      |200.10.57.95|
| 4       |200.10.57.96         |200.10.57.97      |200.10.57.126     |200.10.57.98|
| 5       |200.10.57.128        |200.10.57.129     |200.10.57.158     |200.10.57.130|
| 6       |200.10.57.160        |200.10.57.161     |200.10.57.190     |200.10.57.162|
| 7       |200.10.57.192        |200.10.57.193     |200.10.57.222     |200.10.57.223|
| 8       |200.10.57.224        |200.10.57.225     |200.10.57.254     |200.10.57.255|

</center>


14. Completa la siguiente tabla:

<center>


| `ip`          | Máscara         | Subred        | Broadcast     | Número hosts |
|---------------|-----------------|---------------|---------------|--------------|
| 192.168.1.130 | 255.255.255.128 | 192.168.1.128 | 192.168.1.255 | 128-2        |
| 200.1.17.15   | 255.255.255.0   | 200.1.17.0    | 200.1.17.255  |`255-2`       |
| 133.32.4.61   | 255.255.255.224 |`133.32.4.32`  |               | `30`         |
| 132.4.60.99   | 255.255.0.0     | 132.4.0.0     | 132.4.255.255 | 65534        |
| 222.43.15.41  | `255.255.255.0` | 222.43.15.0   | 222.43.15.255 |              |
|               | 255.255.255.192 | 192.168.0.0   |               |              |

</center>

15. Responde a las siguientes preguntas:

    + Si tenemos una red `147.84.32.0` con máscara de red `255.255.255.252`, indica la dirección de broadcast, la de red y la de los posibles nodos de la red.

        ?

    + La red `192.168.0.0`, ¿de qué clase es?

        Clase C

    + Escribe el rango de direcciones `ip` que pertenecen a la subred definida por la dirección `140.220.15.245` con máscara `255.255.255.240`.



    + Una red de clase B en Internet tiene una máscara de subred igual a `255.255.240.0`. ¿Cuál es el máximo de nodos por subred?

16. Calcular la dirección de red y la dirección de broadcast (difusión) de las máquinas con las siguientes direcciones IP y máscaras de subred (si no se especifica, se utiliza la máscara por defecto).

    + `18.120.16.250` Máscara de red: 255.0.0.0 Dirección de red: 18.0.0.0 Dirección de broadcast:
    + `18.120.16.255 / 255.255.0.0` Dirección de red: Operación `and` entre ip y máscara de red: 00010010.01111000.00010000.11111111

         11111111.11111111.00000000.00000000

         00010010.01111000.00000000.00000000 = **18.120.0.0 (Dirección de red)**

      Dirección de broadcast:  

    + `155.4.220.39`    Máscara de red de clase B: 255.255.0.0

    Opeación `and` entre ip y máscara de red:

    10011011.00000100.11011100.00100111

    11111111.11111111.00000000.00000000

    10011011.00000100.00000000.00000000 = **155.4.0.0 (Dirección de red)**

    Dirección de broadcast: 

    + `194.209.14.33` Máscara de red clase C: 255.255.255.0

    Opearación `and` entre ip y máscara:

    11000010.11010001.00001110.00100001

    11111111.11111111.11111111.00000000

    11000010.11010001.00001110.00000000 = **194.209.14.0 (Dirección de red)**

    Dirección de broadcast: **194.209.14.255**

    + `190.33.109.133 / 255.255.255.0`

    Operación `and` entre ip y máscara de red:

    10111110.00100001.01101101.10000101

    11111111.11111111.11111111.00000000

    10111110.00100001.01101101.00000000 = **190.33.109.0 (Dirección de red)**

    Dirección de broadcast: **190.33.109.255**

    + `190.33.109.133 / 255.255.255.128`

    Operación `and` entre ip y máscara de red:

    10111110.00100001.01101101.10000101

    11111111.11111111.11111111.10000000

    10111110.00100001.01101101.10000000 = **190.33.109.128 (Dirección de red)**

    Dirección de broadcast:

    + `192.168.20.25 / 255.255.255.240` 

    Operación `and` entre ip y máscara de red:

    11000000.10101000.00010100.00011001

    11111111.11111111.11111111.11110000

    11000000.10101000.00010100.00010000 = **192.168.20.16 (Dirección de red)**

    Dirección de broadcast: **192.168.20.255**

    + `192.168.20.25 / 255.255.255.192`

    Operación `and` entre ip y máscara de red:

    11000000.10101000.00010100.00011001

    11111111.11111111.11111111.11000000

    11000000.10101000.00010100.00000000 = 192.168.20.0

    Dirección de broadcast: 

17. Responde a las siguientes preguntas:

    + ¿Cuántos ordenadores como máximo se pueden tener en una red de clase A?

        254 porque el primer y el último número están reservados.

    + ¿Cuántos ordenadores como máximo se pueden tener en una red de clase B?

        254x255= 64.770

    + ¿Cuántos ordenadores como máximo se pueden tener en una red de clase C?

        254x255x255= 16.516.350

    + En una red de clase C con máscara `255.255.255.128`, ¿cuántos ordenadores se pueden tener en cada subred?

        

    + En una red de clase C con máscara `255.255.255.192`, ¿cuántos ordenadores se pueden tener en cada subred?



18. Tu empresa tiene una dirección de red de Clase B de `150.10.0.0`. Desea subdividir la red física en 3 subredes.

    + Indica una máscara que permita dividir la red de clase B (al menos) en tres subredes.

        Al ser de clase B hay que coger 2 bits del tercer octeto por lo tanto:

        **Máscara de red: 255.255.0.0**

        11111111.11111111.11000000.00000000= 255.255.192.0 Máscara de subred

        10010110.00001010.00000000.00000000= 150.10.0.0

        10010110.00001010.01100000.00000000= 150.10.96.0

        10010110.00001010.10000000.00000000= 150.10.128.0

        10010110.00001010.11100000.00000000= 150.10.224.0

    + ¿Cuántos hosts puede haber por subred?

    Subred 1: 150.10.0.1 hasta 150.10.95.254

    Subred 2: 150.10.96.1 hasta 150.10.127.254

    Subred 3: 150.10.128.1 hasta 150.10.223.254

    Subred 4: 150.10.224.1 hasta 150.10.255.254

    + ¿Cuál es la dirección de red y la dirección de broadcast de cada una de las 3 subredes creadas?

        Subred 1: Dirección de red: 150.10.0.0 Dirección de broadcast: 150.10.95.255

        Subred 2: Dirección de red: 150.10.96.0 Dirección de broadcast: 150.10.127.255

        Subred 3: Dirección de red: 150.10.128.0 Dirección de broadcast: 150.10.223.255

        Subred 4: Dirección de red: 150.10.224.0 Dirección de broadcast: 150.10.255.255

19. Dada la dirección de clase B `120.32.0.0`, indica qué máscara de subred deberías escoger para tener 4 subredes. Rellena a continuación la siguiente tabla.

Dirección de red en binario= 11110000.10000000.00000000.00000000

Máscara de red: 255.255.0.0

Máscara de subred: 11111111.11111111.11000000.00000000= 255.255.192.0

11110000.10000000.00000000.00000000= 120.32.0.0

11110000.10000000.01000000.00000000= 120.32.64.0

11110000.10000000.10000000.00000000= 120.32.128.0

11110000.10000000.11000000.00000000= 120.32.192.0

<center>

| Número de red | Dirección de subred | Primer host | Último host |
|---------------|---------------------|-------------|-------------|
|1               |120.32.0.0          |120.32.0.1   |120.32.63.254|
|2               |120.32.64.0         |120.32.64.1  |120.32.127.254  |
|3               |120.32.128.0        |120.32.128.1 |120.32.191.254     |
|4               |120.32.192.0        |120.32.192.1 |120.32.255.254     |

</center>

20. Responde a las siguientes preguntas:

    + Si tenemos una red `150.84.32.0` con máscara de red `255.255.255.224`, indica la dirección de broadcast, la de red y la de los posibles nodos de la red.




    + La red `192.168.0.0`, ¿de qué clase es?

        Clase C, porque el primer octeto está en el rango de los de clase C.

    + Escribe el rango de direcciones `ip` que pertenecen a la subred definida por la dirección  `150.84.32.245` con máscara `255.255.255.240`.


    
    + Una red de clase B en Internet tiene una máscara de subred igual a `255.255.240.0`. ¿Cuál es el máximo de nodos por subred?

    255+15

