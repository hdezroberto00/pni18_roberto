## 1. ¿Qué niveles OSI son los niveles de soporte de red? 

Los niveles 1 (Físico), 2 (Enlace de datos), 3 (Red).

## 2. ¿Qué niveles OSI son los niveles de soporte de usuario? 

Los niveles 5 (sesión), 6 (presentación), 7 (aplicación).

## 3. ¿Cómo están OSI e ISO relacionadas entre sí? 

La ISO, fue la encargada de desarrollar el modelo de red OSI.

## 4. Enumere los niveles del modelo OSI. 

1. Física.

2. Enlace de datos.

3. Red.

4. Transporte.

5. Sesión.

6. Presentación.

7. Aplicación.

## 5. ¿Cómo pasa la información de un nivel OSI al siguiente? 

Pasa entre niveles adyacentes, antes de transmitirlo, exceptuando el nivel físico, añade una cabecera para datos de protocolo de dicho nivel. Cuando los datos llegan al receptor se van eliminando las cabeceras hasta que finalmente llega hasta la aplicación destino.

## 6. ¿Qué son las cabeceras y cola y cómo se añaden y se quitan? 

Las cabeceras son datos que se añaden en cada uno de los niveles por los protocolos correspondientes para proporcionar los servicios. Se añaden según descienden los datos de nivel en nivel en el lado del emisor, y se quitan según ascienden en el lado del receptor.

Las colas incluyen código de detección de errores.

## 7. ¿Cuáles son las responsabilidades del nivel físico? 

Transmite los bits a lo largo de un canal de comunicación, se ocupa de cuantos microsegundos dura un bit, y que voltaje representa un 1 o un 0.

## 8. ¿Cuáles son las responsabilidades del nivel de enlace? 

Provee mecanismos para la detección y corrección de errores. Define un esquema de direccionamiento. Provee conectividad nodo a nodo y libre de errores. Provee mecanismos de control de flujo. Define una unidad de intercambio de datos la cual se conoce con el nombre de Frame o trama.

## 9. ¿Cuáles son las responsabilidades del nivel de red? 

Provee un esquema de direccionamiento lógico. Provee conectividad entre sistemas finales. Es la encargada del enrutamiento de los paquetes. Provee control de congestión, Define una unidad de intercambio de datos llamada paquete.

## 10. ¿Cuáles son las responsabilidades del nivel de transporte? 

Provee comunicación entre entidades finales. Hace multiplexamiento. Garantiza la transmisión confiable de los mensajes. Detecta errores en la transmisión de segmentos y los corrige. Establece y termina circuitos virtuales. Realiza un control del flujo. Define una unidad de intercambio de datos llamada segmento.

## 11. El nivel de transporte crea una conexión entre el origen y el destino. ¿Cuáles son los tres eventos involucrados en la conexión? 

+ Establecimiento de la conexión.

+ Transferencia de datos.

+ Liberación de la conexión.

## 12. ¿Cuál es la diferencia entre una dirección de punto en servicio, una dirección lógica y una dirección fisica? 

+ Una dirección lógica está dada por la IP.

+ Una dirección física está dada por la MAC.

## 13. ¿Cuáles son las responsabilidades del nivel de sesión? 

Establece, coordina y termina las conversacones entre aplicaciones.

Administra el intercambio de datos y sincroniza el diálogo entre niveles de presentación de cada sistema.

Ofrece las herramientas para que la capa de aplicación, la de presentación, y la de sesión reporten sus problemas y los recursos disponibles para la comunicación.

## 14. ¿Cuáles son las responsabilidades del nivel de presentación? 

Se ocupa de los aspectos de sintaxis y semántica de la información que se transmite. Compatibiliza la codificación y compime los datos.

## 15. ¿Cuál es el objetivo de la traducción en el nivel de presentación? 

Traducir la información a flujos de bits antes de transmitirla, ya que cada computadora usa un sistema de codificación distinto.

## 16. Indique alguno de los servicios proporcionados por el nivel de aplicación. 

+ Correo electrónico.

+ FTP

+ Telnet

## 17. ¿Cómo se relacionan los niveles de la familia del protocolo TCP/IP con los niveles del modelo OSI?

El nivel de aplicación, presentación y sesión del modelo OSI se agrupa en el nivel de aplicación del protocolo TCP/IP. El nivel de vínculo de datos y nivel físico del modelo OSI se agrupa en el nivel de interfaz de red del protocolo TCP/IP. El nivel de transporte y el de red se mantienen iguales en ambos.

## 18. El nivel____________ decide la localización de los puntos de sincronización.

+ sesión

## 19. En el nivel _______________, la unidad de datos se denomina trama.

+ enlace de datos

## 20. Los servicios de correo y de directorio están disponibles a los usuarios de la red a través del nivel:

+ aplicación

## 21. A medida que los paquetes de datos se mueven  de los niveles inferiores a los superiores las cabeceras:

+ eliminadas
