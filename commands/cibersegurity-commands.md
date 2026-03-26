# Kali Linux & Pentesting Command Reference / Referencia de Comandos de Kali Linux y Pentesting

### 1. Network Reconnaissance

**Description:** Commands to gather information about hosts, domains, and networks.

| Description                                        | Commands            |
| -------------------------------------------------- | ------------------- |
| Perform host discovery and basic network scan      | `nmap -sn <target>` |
| Scan hosts and detect open ports                   | `nmap -sS <target>` |
| Aggressive scan including OS and service detection | `nmap -A <target>`  |
| Query DNS records                                  | `dig <domain>`      |
| Perform reverse DNS lookup                         | `nslookup <domain>` |
| Gather domain information                          | `whois <domain>`    |
| List active network connections                    | `netstat -tuln`     |
| Display routing table                              | `route -n`          |

---

### 2. Port Scanning

**Description:** Commands to identify open ports, services, and potential entry points.

| Description                | Commands                   |
| -------------------------- | -------------------------- |
| TCP SYN scan               | `nmap -sS <target>`        |
| TCP connect scan           | `nmap -sT <target>`        |
| UDP scan                   | `nmap -sU <target>`        |
| Scan a range of ports      | `nmap -p 1-65535 <target>` |
| Detect service versions    | `nmap -sV <target>`        |
| Scan multiple IP addresses | `nmap -iL targets.txt`     |

---

### 3. Service Enumeration

**Description:** Commands to enumerate specific services like HTTP, SMB, FTP, etc.

| Description                              | Commands                          |
| ---------------------------------------- | --------------------------------- |
| Scan for HTTP vulnerabilities            | `nikto -h <target>`               |
| Scan WordPress sites for vulnerabilities | `wpscan --url <target>`           |
| Scan SMB shares                          | `smbclient -L //<target>`         |
| Enumerate SNMP services                  | `snmpwalk -c public -v1 <target>` |
| Banner grabbing for service info         | `nc <target> <port>`              |

---

### 4. Vulnerability & Exploitation

**Description:** Commands for vulnerability assessment and exploitation.

| Description                   | Commands                                |
| ----------------------------- | --------------------------------------- |
| Launch Metasploit console     | `msfconsole`                            |
| Search exploits in Metasploit | `search <service>`                      |
| Use an exploit module         | `use exploit/<path>`                    |
| Set payload in Metasploit     | `set payload <payload>`                 |
| Exploit target                | `exploit`                               |
| Scan for vulnerabilities      | `openvas-start` / `openvas-check-setup` |

---

### 5. Passwords & Cracking

**Description:** Commands for brute-forcing, password recovery, and hash cracking.

| Description                  | Commands                                            |
| ---------------------------- | --------------------------------------------------- |
| Brute-force SSH or FTP login | `hydra -l <user> -P <password_list> ssh://<target>` |
| Crack password hashes        | `john --wordlist=<wordlist> <hashfile>`             |
| GPU-based hash cracking      | `hashcat -m <hash_type> <hashfile> <wordlist>`      |
| Generate rainbow tables      | `rcracki_mt <path_to_table> -h <hash>`              |

---

### 6. Wireless / Wi-Fi

**Description:** Commands for wireless network reconnaissance, monitoring, and attacks.

| Description              | Commands                                             |
| ------------------------ | ---------------------------------------------------- |
| Enable monitor mode      | `airmon-ng start <interface>`                        |
| Capture Wi-Fi traffic    | `airodump-ng <interface>`                            |
| Deauthenticate clients   | `aireplay-ng --deauth <number> -a <AP> <interface>`  |
| Crack WPA/WPA2 handshake | `aircrack-ng -w <wordlist> -b <BSSID> <capturefile>` |
| Check wireless networks  | `iwconfig`                                           |

---

### 7. Traffic Analysis & Sniffing

**Description:** Commands for packet capture, traffic inspection, and MITM attacks.

| Description                 | Commands                                            |
| --------------------------- | --------------------------------------------------- |
| Capture network packets     | `tcpdump -i <interface>`                            |
| Open Wireshark GUI          | `wireshark`                                         |
| Perform ARP spoofing / MITM | `ettercap -T -M arp:remote /<target1>/ /<target2>/` |
| Dump SSL/TLS traffic        | `ssldump -i <interface>`                            |
| Monitor network interfaces  | `ifconfig` or `ip addr`                             |

---

### 8. Social Engineering & Phishing

**Description:** Commands to create phishing campaigns, spoof emails, or capture credentials.

| Description                      | Commands                                                            |
| -------------------------------- | ------------------------------------------------------------------- |
| Start Social Engineering Toolkit | `setoolkit`                                                         |
| Generate phishing payload        | `setoolkit -> Social-Engineering Attacks -> Website Attack Vectors` |
| Start phishing server            | `python3 -m http.server <port>`                                     |
| Send spoof email                 | `sendmail -t < email_file>`                                         |

---

### 9. Malware & Forensics

**Description:** Commands for malware analysis and digital forensics.

| Description                 | Commands                                                 |
| --------------------------- | -------------------------------------------------------- |
| Analyze memory dump         | `volatility -f <memory_dump> --profile=<profile> pslist` |
| Recover deleted files       | `foremost -i <disk_image> -o <output_dir>`               |
| Extract firmware / binaries | `binwalk <file>`                                         |
| Search for strings in files | `strings <file>`                                         |
| Compute file hash           | `md5sum <file>` / `sha256sum <file>`                     |

---

### 10. Common Kali Tools

**Description:** Frequently used tools for general pentesting and information gathering.

| Description              | Commands                     |
| ------------------------ | ---------------------------- |
| Send raw network data    | `netcat -nv <target> <port>` |
| HTTP requests from CLI   | `curl <url>`                 |
| Download files           | `wget <url>`                 |
| Automate tasks with Bash | `bash <script.sh>`           |
| Reverse shell listener   | `nc -lvnp <port>`            |

---

### 11. Utilities & Scripting

**Description:** General-purpose Linux commands to facilitate pentesting workflows.

| Description                 | Commands                         |
| --------------------------- | -------------------------------- |
| List files and directories  | `ls -la`                         |
| Search for text in files    | `grep -r <pattern> <path>`       |
| Monitor real-time processes | `top` / `htop`                   |
| Archive and compress files  | `tar -cvf <archive.tar> <files>` |
| Execute commands remotely   | `ssh <user>@<host>`              |
| Schedule tasks              | `cron` or `crontab -e`           |

---

## Versión en Español

### 1. Reconocimiento de Red

**Descripción:** Comandos para recopilar información sobre hosts, dominios y redes.

| Descripción                                      | Comandos              |
| ------------------------------------------------ | --------------------- |
| Descubrimiento de hosts y escaneo básico         | `nmap -sn <objetivo>` |
| Escaneo de hosts y detección de puertos abiertos | `nmap -sS <objetivo>` |
| Escaneo agresivo incluyendo OS y servicios       | `nmap -A <objetivo>`  |
| Consultar registros DNS                          | `dig <dominio>`       |
| Consulta inversa de DNS                          | `nslookup <dominio>`  |
| Obtener información de dominio                   | `whois <dominio>`     |
| Listar conexiones de red activas                 | `netstat -tuln`       |
| Mostrar tabla de enrutamiento                    | `route -n`            |

---

### 2. Escaneo de Puertos

**Descripción:** Comandos para identificar puertos abiertos, servicios y posibles vectores de entrada.

| Descripción                       | Comandos                     |
| --------------------------------- | ---------------------------- |
| Escaneo TCP SYN                   | `nmap -sS <objetivo>`        |
| Escaneo TCP connect               | `nmap -sT <objetivo>`        |
| Escaneo UDP                       | `nmap -sU <objetivo>`        |
| Escaneo de rango de puertos       | `nmap -p 1-65535 <objetivo>` |
| Detección de versión de servicios | `nmap -sV <objetivo>`        |
| Escaneo de múltiples IP           | `nmap -iL targets.txt`       |

---

### 3. Enumeración de Servicios

**Descripción:** Comandos para enumerar servicios específicos como HTTP, SMB, FTP, etc.

| Descripción                           | Comandos                            |
| ------------------------------------- | ----------------------------------- |
| Escaneo de vulnerabilidades HTTP      | `nikto -h <objetivo>`               |
| Escaneo de vulnerabilidades WordPress | `wpscan --url <objetivo>`           |
| Escaneo de comparticiones SMB         | `smbclient -L //<objetivo>`         |
| Enumeración de servicios SNMP         | `snmpwalk -c public -v1 <objetivo>` |
| Banner grabbing de servicios          | `nc <objetivo> <puerto>`            |

---

### 4. Vulnerabilidades y Explotación

**Descripción:** Comandos para evaluación de vulnerabilidades y explotación.

| Descripción                   | Comandos                                |
| ----------------------------- | --------------------------------------- |
| Iniciar consola de Metasploit | `msfconsole`                            |
| Buscar exploits en Metasploit | `search <servicio>`                     |
| Usar un módulo exploit        | `use exploit/<ruta>`                    |
| Configurar payload            | `set payload <payload>`                 |
| Explotar objetivo             | `exploit`                               |
| Escanear vulnerabilidades     | `openvas-start` / `openvas-check-setup` |

---

### 5. Contraseñas y Cracking

**Descripción:** Comandos para fuerza bruta, recuperación de contraseñas y cracking de hashes.

| Descripción            | Comandos                                                     |
| ---------------------- | ------------------------------------------------------------ |
| Brute-force SSH o FTP  | `hydra -l <usuario> -P <lista_contraseñas> ssh://<objetivo>` |
| Cracking de hashes     | `john --wordlist=<wordlist> <hashfile>`                      |
| Cracking con GPU       | `hashcat -m <tipo_hash> <hashfile> <wordlist>`               |
| Generar rainbow tables | `rcracki_mt <ruta_tabla> -h <hash>`                          |

---

### 6. Wireless / Wi-Fi

**Descripción:** Comandos para reconocimiento, monitoreo y ataques en redes inalámbricas.

| Descripción                 | Comandos                                             |
| --------------------------- | ---------------------------------------------------- |
| Activar modo monitor        | `airmon-ng start <interfaz>`                         |
| Capturar tráfico Wi-Fi      | `airodump-ng <interfaz>`                             |
| Desautenticar clientes      | `aireplay-ng --deauth <numero> -a <AP> <interfaz>`   |
| Crackear handshake WPA/WPA2 | `aircrack-ng -w <wordlist> -b <BSSID> <capturefile>` |
| Revisar redes inalámbricas  | `iwconfig`                                           |

---

### 7. Análisis de Tráfico y Sniffing

**Descripción:** Comandos para captura de paquetes, inspección de tráfico y ataques MITM.

| Descripción                   | Comandos                                                |
| ----------------------------- | ------------------------------------------------------- |
| Captura de paquetes de red    | `tcpdump -i <interfaz>`                                 |
| Abrir GUI de Wireshark        | `wireshark`                                             |
| Spoofing ARP / MITM           | `ettercap -T -M arp:remote /<objetivo1>/ /<objetivo2>/` |
| Captura de tráfico SSL/TLS    | `ssldump -i <interfaz>`                                 |
| Monitorizar interfaces de red | `ifconfig` o `ip addr`                                  |

---

### 8. Ingeniería Social y Phishing

**Descripción:** Comandos para crear campañas de phishing o capturar credenciales.

| Descripción                        | Comandos                                                            |
| ---------------------------------- | ------------------------------------------------------------------- |
| Iniciar Social Engineering Toolkit | `setoolkit`                                                         |
| Generar payload de phishing        | `setoolkit -> Social-Engineering Attacks -> Website Attack Vectors` |
| Iniciar servidor phishing          | `python3 -m http.server <puerto>`                                   |
| Enviar email spoof                 | `sendmail -t < archivo_email>`                                      |

---

### 9. Malware y Forense

**Descripción:** Comandos para análisis de malware y forense digital.

| Descripción                   | Comandos                                                 |
| ----------------------------- | -------------------------------------------------------- |
| Analizar volcado de memoria   | `volatility -f <memory_dump> --profile=<profile> pslist` |
| Recuperar archivos eliminados | `foremost -i <imagen_disco> -o <output_dir>`             |
| Extraer firmware / binarios   | `binwalk <archivo>`                                      |
| Buscar strings en archivos    | `strings <archivo>`                                      |
| Calcular hash de archivo      | `md5sum <archivo>` / `sha256sum <archivo>`               |

---

### 10. Herramientas Comunes de Kali

**Descripción:** Herramientas frecuentes para pentesting general e información.

| Descripción                        | Comandos                         |
| ---------------------------------- | -------------------------------- |
| Enviar datos de red crudos         | `netcat -nv <objetivo> <puerto>` |
| Realizar peticiones HTTP desde CLI | `curl <url>`                     |
| Descargar archivos                 | `wget <url>`                     |
| Automatizar tareas con Bash        | `bash <script.sh>`               |
| Escucha reverse shell              | `nc -lvnp <puerto>`              |

---

### 11. Utilidades y Scripting

**Descripción:** Comandos generales de Linux para facilitar el pentesting.

| Descripción                         | Comandos                            |
| ----------------------------------- | ----------------------------------- |
| Listar archivos y directorios       | `ls -la`                            |
| Buscar texto en archivos            | `grep -r <patron> <ruta>`           |
| Monitorizar procesos en tiempo real | `top` / `htop`                      |
| Comprimir y archivar archivos       | `tar -cvf <archivo.tar> <archivos>` |
| Ejecutar comandos remotamente       | `ssh <usuario>@<host>`              |
| Programar tareas                    | `cron` o `crontab -e`               |

---

