# Ejercicio 1

## Subred de 2000 hosts

Para conseguir 1000 hosts hay qeu coger 11 bits porque 2^11 son 2044 hosts disponibles.

Esto dejaría la máscara como: 255.255.11111000.00000000 = 255.255.248.0 = /21

Dirección de red: 172.25.0.0

Rango: 172.25.0.1 - 172.25.7.254

Broadcast: 172.25.7.255

## Subred de 1000 hosts

Para conseguir 1000 hosts hay que coger 10 bits porque 2^10 son 1022 hosts disponibles.

Esto dejaría la máscara de red como: 255.255.11111100.00000000 = 255.255.252.0 = /22

Dirección de red: 172.25.8.0

Rango: 172.25.8.1 - 172.25.11.254

Broadcast: 172.15.11.255

## Subred de 1000 hosts

Para conseguir 1000 hosts hay que coger 10 bits porque 2^10 son 1022 hosts disponibles.

Esto dejaría la máscara de red como: 255.255.11111100.00000000 = 255.255.252.0 = /22

Dirección de red: 172.25.12.0

Rango: 172.25.12.1 - 172.25.15.254

Broadcast: 172.25.15.255

## Subred de 70 hosts

Para conseguir 70 hosts hay que coger 7 bits porque 2^7 son 126 hosts disponibles.

Esto dejaría la máscara de red como: 255.255.255.10000000 = 255.255.255.128 = /25

Dirección de red: 172.25.16.0

Rango: 172.25.16.1 - 172.25.16.126

Broadcast: 172.25.16.127

## Subred de 60 hosts

Para conseguir 60 hosts hay que coger 6 bits porque 2^6 son 62 hosts disponibles.

Esto dejaría la máscara de red como: 255.255.255.11000000 = 255.255.255.192 = /26

Dirección de red: 172.25.16.128

Rango: 172.25.16.129 - 172.25.16.190

Broadcast: 172.25.16.191

## Subred de 5 hosts

Para conseguir 5 hosts hay que coger 3 bits porque 2^3 son 6 hosts disponibles.

Esto dejaría la máscara de red como: 255.255.255.11111000 = 255.255.255.248 = /29

Dirección de red: 172.25.16.192

Rango= 172.25.16.193 - 172.25.16.198

Broadcast= 172.25.16.199

# Subredes de 2 hosts

Para conseguir 2 hosts hay que coger 2 bits porque 2^2 son 2 hosts disponibles

Esto dejaría la máscara de red como 255.255.255.11111100 = 255.255.255.252 = /30



---

# Ejercicio 3

Huelva-Sevilla

| 172.16.64.0 | 10101100 | 00010000 | 01000000 | 00000000 |
|-------------|----------|----------|----------|----------|
| 172.16.65.0 | 10101100 | 00010000 | 01000001 | 00000000 |
| 172.16.66.0 | 10101100 | 00010000 | 01000010 | 00000000 |
| 172.16.67.0 | 10101100 | 00010000 | 01000010 | 00000000 |
|             | 10101100 | 00010000 | 01000000 | 00000000 |

La parte de coincide es 10101100.00010000.01000000.00000000

Cadiz-Sevilla

