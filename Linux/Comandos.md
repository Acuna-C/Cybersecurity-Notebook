# 🐧 Comandos Linux

## 1. Navegación y Gestión de Archivos


| Comando | Uso |
| :---: | :---: |
| pwd | Muestra la ruta del directorio actual |
| ls -la | Lista todos los archivos y carpetas (incluidos ocultos) con permisos y detalles |
| cd | Cambia al directorio especificado (cd .. sube un nivel). |
| mkdir <nombre> | Crea una nueva carpeta |
| cp <origen> <destino>|Copia un archivo o directorio (cp -r para carpetas)|
| mv <origen> <destino>|Mueve o renombra un archivo o directorio|
| rm <archivo>|Elimina un archivo (rm -rf <carpeta> elimina una carpeta y su contenido)|
---

## 2. Lectura y Búsqueda


| Comando | Uso |
| :---: | :---: |
| cat <archivo> | Muestra todo el contenido de un archivo en pantalla |
| head -n 10 <archivo> | Muestra las primeras 10 líneas de un archivo |
| tail -n 10 <archivo> | Muestra las últimas 10 líneas de un archivo (tail -f lo sigue en tiempo real) |
| grep "<texto>" <archivo> | Busca una palabra o patrón dentro de un archivo |
| find <ruta> -name "<nombre>"|Busca archivos o carpetas por nombre|

---

## 3. Redes y Diagnóstico


| Comando | Uso |
| :---: | :---: |
| ip a / ip addr | Muestra las interfaces de red y sus direcciones IP |
| ping -c 4 <ip_o_dominio> | Envía paquetes para verificar conectividad con un host |
| ss -tuln / netstat -tuln | Lista los puertos abiertos y servicios a la escucha |
| curl -I <url>|Obtiene las cabeceras HTTP de un sitio web|

---

## 4. Permisos y Sistema


| Comando | Uso |
| :---: | :---: |
| chown <usuario>:<grupo> <archivo> | Cambia el propietario de un archivo |
| sudo <comando> |Ejecuta un comando con privilegios de superusuario (root) |
| htop / top |Muestra los procesos en tiempo real y el uso de CPU/RAM |
| ps aux | Lista todos los procesos activos en el sistema |


---

## 5. Permisos chmod

| chmod | signo | uso |
| :---: | :---: | :---: |
| chmod | + | Añade los permisos especificados |
| chmod | - | Remueve los permisos especificados |
| chmod | = | Establece exactamente los permisos dados (sobrescribe los anteriores) |

---
| chmod  | Letra | uso |
| :---: | :---: | :---: |
| chmod | u | (user): El usuario propietario del archivo |
| chmod | g | (group): El grupo de usuarios al que pertenece el archivo |
| chmod | o | (others): Cualquier otro usuario del sistema |
| chmod | a | (all): Todos los anteriores (u + g + o). |
| chmod | r | (read): Leer/ver el contenido |
| chmod | w | (write): Modificar/escribir |
| chmod | x | (execute): Ejecutar como programa o entrar a un directorio |
| chmod | s | (setuid / setgid): Ejecuta el archivo con los privilegios del dueño o grupo |
| chmod | t | (sticky bit): Evita que usuarios borren archivos de otros en carpetas compartidas |



## 6. Valores Octales (Notación Numérica)

En lugar de letras, se pueden sumar valores numéricos para combinar permisos:

| Numero | Accion |
| :---: | :---: |
|4| Lectura (r)|
|2| Escritura (w)|
|1| Ejecución (x)|
|0| Sin permisos (-)|

Ejemplo: 4 + 2 + 1 = 7 (Permisos totales: rwx).

Comando: chmod 755 archivo (Propietario: 7 rwx, Grupo: 5 r-x, Otros: 5 r-x).




---


## Ejemplos claros de cómo usar u, g, o y a:


| Ejmplo | Accion |
| :---: | :---: |
|chmod u+x script.sh| Significado: Le da permiso de ejecución (+x) únicamente al propietario (u) del archivo. El grupo y los demás usuarios no podrán ejecutarlo|
|chmod g+w documento.txt| Significado: Le da permiso de escritura (+w) al grupo (g) asignado al archivo. Útil para trabajar en equipo sobre un mismo documento|
|chmod o-r secreto.txt| Significado: Le quita el permiso de lectura (-r) a los demás usuarios (o). Solo el dueño y los miembros del grupo podrán leerlo|
|chmod a+r leeme.txt|Significado: Le da permiso de lectura (+r) a todos los usuarios (a: usuario, grupo y otros)|
|chmod u+rw,g+r,o-rwx reporte.pdf (Combinado)|Significado: Otorga lectura y escritura al dueño (u+rw), solo lectura al grupo (g+r), y quita todos los permisos a los demás (o-rwx)|
