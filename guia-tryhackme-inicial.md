--------- GUÍA TRYHACKME INICIAL ------------

-- ¿Que es TryHackMe?
Plataforma online para practicar hacking ético con laboratorios reales. Ideal para
principiantes y personas que se preparan para certificaciones como eJPT, CompTIA, etc.



-- ¿Como empezar?
1. Crea tu cuenta:
  [https://tryhackme.com]
2. Elige modo de conexión:
  AttackBox (web) o VPN (con Kali)
3. Comienza por estas salas:
    |  Sala  |  Nivel  |  Enlace  |
  |---------|--------|---------------|
  |  Introduction to Cyber Security  |  Muy Facil  |  [Ir](https://tryhackme.com/room.introoffensivesecurity)  |
  |  Pre Security  |  Básico  |  [Ir](https://tryhackme.com/room/introtonetworking)  |
  |  Linux Fundamentals  |  Fácil  |  [Ir](https://tryhackme.com/module/linux-fundamentals)  |
 
 

-- Salas recomendadas por nivel
  |  Nivel  |  Sala  |  Descripción  |
  |---------|--------|---------------|
  |  🟢  |  Introduction to Offensive Security  |  Fundamentos  |
  |  🟡  |  Linux Fundamentals  |  Linux desde cero  |
  |  🟡  |  Network Fundamentals  |  Redes  |
  |  🔵  |  Blue  |  Primer pentest  
  |  🔵  |  Vulnversity  |  Escaneo y explotación  |
  |  🔴  |  Ice  |  Explotación avanzada  |


-- Herramientas y comandos básicos
- NMAP:
  ```bash
  nmap -sC -sV -oN scan.txt <IP>
  ````

- GOBUSTER:
  ```bash
  gobuster dir -u http://<IP> -w /usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt
  ````
  
- HYDRA:
  ```bash
  hydra -l admin -P rockyou.txt ftp://<IP>
  ````

-NETCAT:
 ```bash
 nc <IP> <puerto>
 ````


 -- Consejos personales
 - Organiza cada máquina en carpetas
 - Documenta todo (puedes usar Obsidian, Notion)
 - No corras, repite y analiza
 - Participa en la comunidad
 - Prioriza aprender antes que resolver rápido


-- Recursos útiles
* HackTricks
* Exploit-DB
* Pentest Bookmarks
* Canales: The Cyber Mnetor, John Hammond, InfoSec Pat


  

