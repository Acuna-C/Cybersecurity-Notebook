# ¿Qué es TCP/IP?

TCP/IP (Transmission Control Protocol / Internet Protocol) es el conjunto de protocolos que permite la comunicación entre dispositivos en una red y en Internet.

Objetivos
- Permitir la comunicación entre equipos.
- Definir cómo se transmiten los datos.
- Garantizar el direccionamiento de dispositivos.
- Asegurar el transporte de información.


# Modelo TCP/IP

El modelo TCP/IP tiene 4 capas:


| Capa TCP/IP   |           Equivalente OSI          |
|---------------|------------------------------------|
| Aplicación    |             5, 6 y 7               |
| Transporte	  |                 4                  |
| Internet      |                 3                  |
| Acceso a Red  |               1 y 2                |



# Diagrama

|                   DIAGRAMA                         |
|----------------------------------------------------|
|                   Aplicación                       |
|                   Transporte	                     |
|                    Internet                        |
|                  Acceso a Red                      |


# Capa de Aplicación

Permite la interacción entre aplicaciones y la red.

Protocolos comunes


|Protocolo	  |Puerto	             |Función                      |
|-------------|--------------------|-----------------------------|
|HTTP	        |80	                 |Navegación web               |
|HTTPS	      |443	               |Web segura                   |
|FTP	        |21	                 |Transferencia de archivos    |
|SSH	        |22                  |Administración remota segura |
|DNS          |53                  |Resolución de nombres        |
|DHCP         |67/68	             |Asignación IP                |
|SMTP         |25	                 |Correo saliente              |
|POP3         |110	               |Recepción correo             |
|IMAP         |143	               |Sincronización correo        |



# Capa de Transporte

Responsable de la comunicación entre aplicaciones.

TCP

Transmission Control Protocol.

Características:

- Orientado a conexión.
- Confiable.
- Control de errores.
- Control de flujo.
- Garantiza entrega.

# Capa Internet

Responsable del direccionamiento y enrutamiento.

IP

Internet Protocol.

Funciones:

- Identificación de hosts.
- Direccionamiento.
- Enrutamiento.


# Capa de Acceso a Red

Se encarga de la transmisión física.

Tecnologías:

- Ethernet
- WiFi
- Fibra óptica
