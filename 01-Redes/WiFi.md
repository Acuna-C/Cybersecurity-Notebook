# 📶 Wi-Fi & Seguridad Inalámbrica (IEEE 802.11)

## 1. ¿Qué debo saber?
* **SSID:** Nombre visible de la red Wi-Fi.
* **BSSID:** Dirección MAC del punto de acceso (Access Point).
* **4-Way Handshake (WPA2):** Proceso de autenticación de 4 pasos donde se valida la clave precompartida (PSK) sin enviarla en texto plano.

---

## 2. Evolución del Cifrado

| Estándar | Estado | Nivel de Seguridad |
| :---: | :---: | :--- |
| **WEP** | Obsoleto | Roto. Se rompe en minutos recolectando vectores de inicialización (IVs). |
| **WPA (TKIP)** | Obsoleto | Inseguro. vulnerable a ataques de inyección. |
| **WPA2 (CCMP/AES)** | Estándar actual | Seguro si la clave es robusta. Vulnerable a captura de Handshake + Cracking offline. |
| **WPA3 (SAE)** | Recomendado | Resistente a ataques de diccionario offline. |
