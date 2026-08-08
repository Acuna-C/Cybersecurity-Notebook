## 1. ¿Qué debo saber?
Protocolo que asigna dinámicamente direcciones IP, máscaras, gateways y servidores DNS a los clientes de la red.

---

## 2. Proceso DORA (Handshake de 4 Pasos)
1. **Discover:** El cliente envía un mensaje Broadcast preguntando "¿Hay algún servidor DHCP?".
2. **Offer:** El servidor DHCP responde ofertando una IP disponible.
3. **Request:** El cliente responde solicitando formalmente esa IP.
4. **Acknowledge (ACK):** El servidor confirma la asignación y le otorga el tiempo de concesión (Lease Time).

---

## 3. Ataques DHCP
* **DHCP Starvation:** Un atacante agota el estanque de IPs enviando miles de solicitudes con direcciones MAC falsas.
* **Rogue DHCP:** Un atacante monta un servidor DHCP no autorizado para repartir IPs con un falso Gateway y realizar un Man-In-The-Middle (MITM)
