# 🏷️ VLANs & Enlace Troncal (Trunking)

## 1. ¿Qué debo saber?
* **VLAN (Virtual LAN):** Permite segmentar una red física en múltiples redes lógicas independientes en el Switch (Capa 2).
* **IEEE 802.1Q:** Estándar que añade una etiqueta (Tag) de 4 bytes a la trama Ethernet para identificar la VLAN a la que pertenece el tráfico.
* **Trunking (Puerto Troncal):** Enlace entre switches que transporta el tráfico de múltiples VLANs etiquetadas.

---

## 2. Riesgo de Seguridad
* **VLAN Hopping:** Ataque donde un dispositivo intenta enviar paquetes con etiquetas dobles (Double Tagging) o negociar un enlace troncal falso (vía DTP) para acceder a una VLAN restringida.
