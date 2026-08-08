# 🤝 Modelo TCP/IP & Protocolos de Transporte

## 1. ¿Qué debo saber?
* [cite_start]**TCP (Transmission Control Protocol):** Orientado a conexión, confiable, garantiza orden y entrega de paquetes[cite: 67].
* [cite_start]**UDP (User Datagram Protocol):** Sin conexión, sin garantías de entrega, ligero y rápido (usado en Streaming, VoIP, DNS)[cite: 67].

---

## 2. Handshake de 3 Vías (3-Way Handshake)
[cite_start]Para abrir una conexión TCP válida entre Cliente y Servidor[cite: 67]:
1. **Cliente $\rightarrow$ Servidor:** `SYN` (Sincronización).
2. **Servidor $\rightarrow$ Cliente:** `SYN-ACK` (Aceptación y Sincronización).
3. **Cliente $\rightarrow$ Servidor:** `ACK` (Confirmación final).

---

## 3. Banderas (Flags) TCP Críticas
* **SYN:** Inicia una conexión.
* **ACK:** Confirma la recepción de datos o paquetes.
* **FIN:** Cierre elegante de la conexión.
* **RST:** Reinicio forzado inmediato de la conexión.
* **PSH:** Pide procesar los datos de inmediato sin esperar a llenar el búfer.
* **URG:** Indica que los datos son urgentes.
