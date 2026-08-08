# 🌐 Direccionamiento IPv4

## 1. ¿Qué debo saber?
Una dirección IPv4 tiene 32 bits divididos en 4 octetos (ej. `192.168.1.10`).

---

## 2. Clases de Direcciones IPv4

| Clase | Rango | Máscara por Defecto | Uso |
| :---: | :---: | :---: | :--- |
| **A** | `1.0.0.0` a `126.255.255.255` | `255.0.0.0` (`/8`) | Redes muy grandes. |
| **B** | `128.0.0.0` a `191.255.255.255` | `255.255.0.0` (`/16`) | Redes medianas. |
| **C** | `192.0.0.0` a `223.255.255.255` | `255.255.255.0` (`/24`) | Redes pequeñas / LANs. |

---

## 3. Rangos de Direcciones Privadas (RFC 1918)
Estas direcciones no son enrutables en Internet:
* **Clase A:** `10.0.0.0` a `10.255.255.255`
* **Clase B:** `172.16.0.0` a `172.31.255.255`
* **Clase C:** `192.168.0.0` a `192.168.255.255`

> **NAT (Network Address Translation):** Traduce múltiples IP privadas internas a una sola IP pública para navegar en Internet.
