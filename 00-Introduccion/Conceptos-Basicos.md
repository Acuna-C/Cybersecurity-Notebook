# Conceptos Básicos de Redes y Ciberseguridad

## ¿Qué es una Red?
 
Una red es un conjunto de dispositivos conectados entre sí que intercambian información y recursos.
 
### Ejemplos de dispositivos

- Computadores
- Servidores
- Switches
- Routers
- Impresoras
- Smartphones


### Tipos de red
 
| Tipo | Descripción |
|--------|------------|
| PAN | Red personal |
| LAN | Red local |
| MAN | Red metropolitana |
| WAN | Red de área amplia |
| WLAN | Red inalámbrica |

---

# ¿Qué es Internet?
 
Internet es una red mundial compuesta por millones de dispositivos conectados mediante el conjunto de protocolos TCP/IP.

Características:

- Descentralizada
- Escalable
- Global
- Basada en estándares
 
---
 
# Host

Un host es cualquier dispositivo conectado a una red con capacidad para enviar y recibir datos.
 
Ejemplos:

- PC
- Laptop
- Servidor
- Smartphone
- Cámara IP

---

# Dirección IP
 
Una dirección IP identifica de forma lógica a un dispositivo dentro de una red.

Ejemplo IPv4:

192.168.1.10

Ejemplo IPv6:

2001:db8::1

---


# Dirección MAC

Una dirección MAC es un identificador físico único asignado a una interfaz de red.

Ejemplo:

00:1A:2B:3C:4D:5E

Características:

- 48 bits
- Única por fabricante
- Opera en Capa 2

---

# Router

Dispositivo que conecta diferentes redes y dirige los paquetes de datos.

Funciones:

- Enrutamiento
- Conexión a Internet
- NAT
- Seguridad básica

---

# Switch

Dispositivo que conecta equipos dentro de una misma red.

Funciones:

- Aprender direcciones MAC
- Reenviar tráfico eficientemente
- Segmentar dominios de colisión

---

# Hub

Dispositivo antiguo que replica el tráfico a todos los puertos.

Desventajas:

- Bajo rendimiento
- Sin inteligencia de red
- Poco seguro

---

# Cliente y Servidor

## Cliente

Equipo que solicita servicios.

Ejemplo:

- Navegador web

## Servidor

Equipo que entrega servicios.

Ejemplos:

- Servidor Web
- Servidor DNS
- Servidor DHCP

---

# Paquete

Unidad de información transmitida a través de una red.

Un paquete contiene:

- Dirección origen
- Dirección destino
- Datos
- Información de control

---

# Puerto

Número lógico utilizado para identificar servicios o aplicaciones.


Ejemplos:

| Puerto | Servicio |
|----------|----------|
| 22 | SSH |
| 53 | DNS |
| 80 | HTTP |
| 443 | HTTPS |

---

# Protocolo

Conjunto de reglas que permiten la comunicación entre dispositivos.

Ejemplos:

- TCP
- UDP
- HTTP
- HTTPS
- DNS
- DHCP

---

# Ancho de Banda

Cantidad máxima de datos que pueden transmitirse en un tiempo determinado.

Medidas comunes:

- Mbps
- Gbps
- Tbps

---

# Latencia

Tiempo que tarda un paquete en viajar desde el origen hasta el destino.

Generalmente se mide en:

- Milisegundos (ms)


---

# DNS

Domain Name System.

Convierte nombres de dominio en direcciones IP.

Ejemplo:

google.com → 142.250.x.x

---

# DHCP

Dynamic Host Configuration Protocol.

Asigna automáticamente:

- Dirección IP
- Máscara de red
- Gateway
- DNS

---

# Gateway

Puerta de enlace utilizada para salir de una red local hacia otras redes.

Ejemplo:

192.168.1.1

---

# VPN

Virtual Private Network.

Permite crear una conexión segura y cifrada a través de Internet.

Beneficios:

- Privacidad
- Protección de datos
- Acceso remoto seguro

---

# Firewall

Sistema de seguridad que controla el tráfico de red.

Funciones:

- Permitir conexiones
- Bloquear conexiones
- Registrar eventos

Ejemplos:

- Windows Firewall
- pfSense
- Fortinet
- Palo Alto

---

# Malware

Software diseñado para dañar o comprometer sistemas.

Tipos:

- Virus
- Gusanos
- Troyanos
- Spyware
- Ransomware

---

# Vulnerabilidad

Debilidad que puede ser explotada por una amenaza.

Ejemplos:

- Software desactualizado
- Contraseñas débiles
- Mala configuración

---

# Amenaza

Cualquier evento o actor capaz de explotar una vulnerabilidad.

Ejemplos:

- Hackers
- Malware
- Desastres naturales
- Error humano

---

# Riesgo

Probabilidad de que una amenaza explote una vulnerabilidad generando un impacto negativo.

Fórmula conceptual:

Riesgo = Amenaza × Vulnerabilidad × Impacto

---

# Autenticación

Proceso para verificar la identidad de un usuario.

Factores:

### Algo que sé

- Contraseña
- PIN
 
### Algo que tengo

- Token
- Smartphone

### Algo que soy

- Huella digital
- Reconocimiento facial

---

# Principio de Mínimo Privilegio

Un usuario debe tener solamente los permisos necesarios para realizar su trabajo.

Beneficios:

- Reduce riesgos
- Limita ataques
- Mejora la seguridad

---

# Copia de Seguridad (Backup)

Proceso de creación de copias de datos para su recuperación ante incidentes.

Regla 3-2-1:

- 3 copias de los datos
- 2 medios distintos
- 1 copia fuera del sitio

---

# Conceptos Clave para Recordar

✅ IP identifica dispositivos.

✅ MAC identifica interfaces físicas.

✅ DNS traduce nombres a IP.

✅ DHCP asigna configuraciones automáticamente.

✅ Router conecta redes.

✅ Switch conecta dispositivos.

✅ Firewall filtra tráfico.

✅ Vulnerabilidad ≠ Amenaza.

✅ Riesgo = Amenaza + Vulnerabilidad + Impacto.

✅ La seguridad empieza por los principios básicos.
