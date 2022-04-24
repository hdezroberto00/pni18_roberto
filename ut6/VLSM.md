# Ejercicio VSLM

Dada la red 192.168.0.0/24

Conseguir:

+ Una subred de 80 hosts
+ Una subred de 20 hosts
+ Una subred de 20 hosts
+ Una subred de 2 hosts

## Subred de 80 hosts

Para conseguir 80 hosts hay que coger 7 bits para hosts, porque 2^7=128, el numero más proximo por encima de 80.

Esto dejaría la máscara de red como, 255.255.255.10000000 = 255.255.255.128 = /25

La dirección de red sería `192.168.0.0/25`

## Subred de 20 hosts

Para conseguir 20 hosts hay que coger 5 bits para hosts, porque 2^5=32, el número más proximo por encima de 20.

Esto dejaría la máscara de red como, 255.255.255.11100000 = 255.255.255.224 = /27

La dirección de red sería `192.168.0.128/27`

## Subred de 20 hosts

Para conseguir 20 hosts hay que coger 5 bits para hosts, porque 2^5=32, el número más proximo por encima de 20.

Esto dejaría la máscara de red como, 255.255.255.11100000 = 255.255.255.224 = /27

La dirección de red sería `192.168.0.160/27`

## Subred de 2 hosts

Para conseguir 2 hosts hay que coger 1 bit para hosts, porque 2^1=2.

Esto dejaría la máscara de red como, 255.255.255.11111110 = 255.255.255.254 = /31

La dirección de red sería `192.168.0.162/31`

# Sumarización de rutas

Tenemos las redes:

+ `192.168.0.0/25`
+ `192.168.0.128/27`
+ `192.168.0.160/27`
+ `192.168.0.162/31`

## Paso 1

Enumeramos en binario

| Dirección de red | octeto 1 | octeto 2 | octeto 3 | octeto 4 |
|------------------|----------|----------|----------|----------|
| 192.168.0.0      | 11000000 | 10101000 | 00000000 | 00000000 |
| 192.168.0.128    | 11000000 | 10101000 | 00000000 | 10000000 |
| 192.168.0.160    | 11000000 | 10101000 | 00000000 | 10100000 |
| 192.168.0.162    | 11000000 | 10101000 | 00000000 | 10100010 |

## Paso 2

Contar el número de bits coincidentes

| Dirección de red | octeto 1 | octeto 2 | octeto 3 | octeto 4 |
|------------------|----------|----------|----------|----------|
| **192.168.0.0**      | **11000000** | **10101000** | **00000000** | 00000000 |
| **192.168.0.128**    | **11000000** | **10101000** | **00000000** | 10000000 |
| **192.168.0.160**    | **11000000** | **10101000** | **00000000** | 10100000 |
| **192.168.0.162**    | **11000000** | **10101000** | **00000000** | 10100010 |

Coinciden los 24 primeros bits desde la izquierda, por lo tanto la máscara de subred para la ruta sumarizada es /24 ó 255.255.255.0

## Paso 3

Copiar los bits coincidentes y agregar bits 0 para determianar la dirección de red sumariazada.

`192.168.0.0      | 11000000 | 10101000 | 00000000 | 00000000`

La dirección de red sumarizada es 192.168.0.0/24