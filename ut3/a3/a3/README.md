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

| Número de red | Dirección de subred | Primer host | Último host |
|---------------|---------------------|-------------|-------------|
|               |                     |             |             |
|               |                     |             |             |
|               |                     |             |             |
|               |                     |             |             |


</center>

3. Dada la dirección de red `192.168.55.0`, indica qué máscara de subred deberías escoger para tener 8 subredes. Rellena a continuación la siguiente tabla.

<center>

| Número de red | Dirección de subred | Primer host | Último host |
|---------------|---------------------|-------------|-------------|
|               |                     |             |             |
|               |                     |             |             |
|               |                     |             |             |
|               |                     |             |             |
|               |                     |             |             |
|               |                     |             |             |
|               |                     |             |             |
|               |                     |             |             |

</center>


4. Dada la dirección de clase B `150.40.0.0`, indica qué máscara de subred deberías escoger para tener 4 subred. Rellena a continuación la siguiente tabla.

<center>


| Número de red | Dirección de subred | Primer host | Último host |
|---------------|---------------------|-------------|-------------|
|               |                     |             |             |
|               |                     |             |             |
|               |                     |             |             |
|               |                     |             |             |

</center>


5. ¿Cuál es el intervalo decimal y binario del primer octeto para todas las direcciones `ip` clase "B" posibles?
¿Qué octeto u octetos representan la parte que corresponde a la red de una dirección `ip` clase "C"?
¿Qué octeto u octetos representan la parte que corresponde al host de una dirección `ip` clase "A"?

6. Completa la siguiente tabla:

<center>


| Dirección `ip` del host | Dirección clase | Dirección de red | Dirección de host | Dirección de broadcast de red | Máscara de subred por defecto |
|-----------------------|-----------------|------------------|-------------------|-------------------------------|-------------------------------|
| 216.14.55.137         |                 |                  |                   |                               |                               |
| 123.1.1.15            |                 |                  |                   |                               |                               |
| 123.1.1.15            |                 |                  |                   |                               |                               |
| 123.1.1.15            |                 |                  |                   |                               |                               |
| 123.1.1.15            |                 |                  |                   |                               |                               |

</center>

7. Dada una dirección `142.226.0.15` :

    + ¿Cuál es el equivalente binario del segundo octeto?
    + ¿Cuál es la Clase de la dirección?
    + ¿Cuál es la dirección de red de esta dirección `ip`?
    + ¿Es ésta una dirección de host válida? ¿Por qué? o ¿Por qué no?
    + ¿Cuál es la cantidad máxima de hosts que se pueden tener con una dirección de red de clase C? 
    + ¿Cuántas redes de clase B puede haber?
    + ¿Cuántos hosts puede tener cada red de clase B?
    + ¿Cuántos octetos hay en una dirección `ip`?
    + ¿Cuántos bits puede haber por octeto?

8. Determinar, para las siguientes direcciones de host `ip`, cuáles son las direcciones que son válidas para redes comerciales. Válida significa que se puede asignar a una estación de trabajo, servidor, impresora, interfaz de router, etc.

<center>

| Dirección `ip`  | ¿La dirección es válida? | ¿Por qué? |
|-----------------|--------------------------|-----------|
| 150.100.255.255 |                          |           |
| 175.100.255.18  |                          |           |
| 100.0.0.23      |                          |           |
| 188.258.221.176 |                          |           |
| 127.34.25.189   |                          |           |
| 224.156.217.73  |                          |           |

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

<center>

![](img/001.png)

</center>

11. Tu empresa tiene una dirección de red de Clase C de `200.10.57.0` .Desea subdividir la red física en 3 subredes.

    + Indica una máscara que permita dividir la red de clase C (al menos) en tres subredes.
    + ¿Cuántos hosts (ordenadores) puede haber por subred?
    + ¿Cuál es la dirección de red y la dirección de broadcast de cada una de las 3 subredes creadas?

12. Se desea subdividir la dirección de red de clase C de `200.10.57.0` en 4 subredes. Responde a las siguientes preguntas:

    + ¿Cuál es el equivalente en números binarios de la dirección de red de clase C `200.10.57.0` de este ejercicio?
    + ¿Cuál(es) es (son) el (los) octeto(s) que representa(n) la porción de red y cuál(es) es (son) el (los) octeto(s) que representa(n) la porción de host de esta dirección de red de clase C?
    + ¿Cuántos bits se deben pedir prestados a la porción de host de la dirección de red para poder suministrar 8 subredes?
    + ¿Cuál será la máscara de subred (utilizando la notación decimal) basándose en la cantidad de bits que se pidieron prestados en el paso 3?
    + ¿Cuál es el equivalente en números binarios de la máscara de subred a la que se hace referencia anteriormente?

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

