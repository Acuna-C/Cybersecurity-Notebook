# 🧱 Modelo OSI (Open Systems Interconnection)

## 1. ¿Qué debo saber?
El Modelo OSI consta de 7 capas teóricas. La información baja por las capas del emisor (encapsulamiento) y sube por las del receptor (desencapsulamiento).

* **Capas y PDU (Unidad de Datos de Protocolo):**
  * **Capa 7 - Aplicación:** (Datos) HTTP, SSH, FTP, DNS.
  * **Capa 6 - Presentación:** (Datos) Formato, cifrado y compresión (TLS/SSL, ASCII, JPEG).
  * **Capa 5 - Sesión:** (Datos) Establece y mantiene sesiones entre aplicaciones (NetBIOS, RPC).
  * **Capa 4 - Transporte:** (Segmentos) Control de flujo y error (TCP, UDP).
  * **Capa 3 - Red:** (Paquetes) Direccionamiento lógico y enrutamiento (IP, ICMP, ARP).
  * **Capa 2 - Enlace de Datos:** (Tramas) Direccionamiento físico (MAC, Ethernet, Switches).
  * **Capa 1 - Física:** (Bits) Medio transmisor (Cables RJ45, Fibra, Señales Wi-Fi).

---

## 2. Ataques comunes por Capa
* **Capa 2:** ARP Poisoning, MAC Flooding, VLAN Hopping.
* **Capa 3:** IP Spoofing, Ping Flood (ICMP).
* **Capa 4:** SYN Flood (DoS en TCP).
* **Capa 7:** Inyecciones (SQLi), Phishing, Cross-Site Scripting (XSS).
