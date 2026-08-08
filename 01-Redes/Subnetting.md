# ✂️ Subnetting & CIDR

## 1. ¿Qué debo saber?
El subnetting es el proceso de dividir una red IP física en subredes lógicas más pequeñas.
* **CIDR (Classless Inter-Domain Routing):** Representa cuántos bits pertenecen a la red mediante una barra (ej. `/24`).

---

## 2. Tabla de Referencia Rápida (Cheat Sheet)

| CIDR | Máscara de Red | Hosts Totales | Hosts Útiles |
| :---: | :---: | :---: | :---: |
| **/30** | `255.255.255.252` | 4 | **2** (Usado en enlaces punto a punto) |
| **/29** | `255.255.255.248` | 8 | **6** |
| **/28** | `255.255.255.240` | 16 | **14** |
| **/27** | `255.255.255.224` | 32 | **30** |
| **/26** | `255.255.255.192` | 64 | **62** |
| **/25** | `255.255.255.128` | 128 | **126** |
| **/24** | `255.255.255.0` | 256 | **254** |

---

## 3. Regla de Oro
$$\text{Hosts útiles} = 2^{(32 - \text{CIDR})} - 2$$
*(Se restan 2 porque la primera IP es la dirección de Red y la última es el Broadcast).*
