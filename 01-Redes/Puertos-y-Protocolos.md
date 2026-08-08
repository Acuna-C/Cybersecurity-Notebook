# 📋 Torpedo: Puertos y Protocolos Críticos

| Puerto | Protocolo | Servicio | Estado / Comentario de Seguridad |
| :---: | :---: | :--- | :--- |
| **20/21** | TCP | FTP | **Inseguro.** Credenciales viajan en texto plano. |
| **22** | TCP | SSH / SFTP | **Seguro.** Cifrado. Reemplazo de Telnet/FTP. |
| **23** | TCP | Telnet | **Inseguro.** Acceso por consola sin cifrar. |
| **25** | TCP | SMTP | Envío de correos. Vulnerable a Enumeración de usuarios (VRFY/EXPN). |
| **53** | UDP/TCP | DNS | Puerto 53 UDP para consultas, TCP para transferencias de zona (AXFR). |
| **80** | TCP | HTTP | **Inseguro.** Tráfico web en texto plano. |
| **110** | TCP | POP3 | Recepción de correo (Sin cifrar). |
| **139 / 445**| TCP | NetBIOS / SMB | Compartir archivos en Windows. Vector histórico de exploits (ej. EternalBlue / WannaCry). |
| **143** | TCP | IMAP | Acceso a correo electrónico. |
| **389 / 636**| TCP | LDAP / LDAPS | Consulta de directorios (636 cifrado SSL/TLS). |
| **443** | TCP | HTTPS | **Seguro.** Tráfico Web cifrado con TLS/SSL. |
| **3389** | TCP | RDP | Escritorio remoto de Windows. Propenso a ataques de Fuerza Bruta o BlueKeep. |
