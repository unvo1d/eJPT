# Herramienta `hydra`

tags: #herramienta #explotacion #comando #auth #brute-force

## Descripción del Funcionamiento Interno
`hydra` es una herramienta de fuerza bruta rápida para realizar ataques de diccionario sobre diferentes protocolos. Hydra puede realizar ataques de fuerza bruta para varios servicios de autenticación, incluyendo, pero no limitado a, FTP, HTTP(S)-FORM-GET, HTTP(S)-FORM-POST, HTTP(S)-GET, HTTP(S)-HEAD, HTTP-Proxy, ICQ, IMAP, IRC, LDAP, MS-SQL, MySQL, NNTP, Oracle Listener, Oracle SID, PC-Anywhere, PC-NFS, POP3, PostgreSQL, RDP, Rexec, Rlogin, Rsh, SIP, SMB(NT), SMTP, SMTP Enum, SNMP, SOCKS5, SSH(v1 and v2), Subversion, Teamspeak (TS2), Telnet, VMware-Auth, VNC y XMPP.

## Uso
Utilizada para realizar ataques de fuerza bruta en varios servicios y protocolos para identificar credenciales válidas.

## Sintaxis
```bash
hydra [-l LOGIN|-L FILE] [-p PASS|-P FILE] [OPTIONS] [PROTOCOL://]HOST[:PORT]
```

- `-l LOGIN`: Un nombre de usuario específico.
- `-L FILE`: Un archivo con una lista de nombres de usuario.
- `-p PASS`: Una contraseña específica.
- `-P FILE`: Un archivo con una lista de contraseñas.
- `OPTIONS`: Opciones adicionales como `-e nsr`, `-o` para la salida del archivo, `-t` para el número de tareas simultáneas, etc.
- `PROTOCOL://HOST[:PORT]`: Especifica el protocolo, el host y el puerto (opcional).

## Ejemplos

### SSH
```bash
hydra -l usuario -P /ruta/al/diccionario.txt ssh://192.168.1.1
```
### FTP
```bash
hydra -l usuario -P /ruta/al/diccionario.txt ftp://192.168.1.1
```
### HTTP-POST
```bash
hydra -l usuario -P /ruta/al/diccionario.txt http-post-form://192.168.1.1:80/login.php:usuario=^USER^&contrasena=^PASS^:F=Login incorrecto
```
### SMTP 
```bash
hydra -L /ruta/al/diccionario.txt -p cualquiercosa smtp://192.168.1.1
```

