# `Evil-WinRM`

tags: #herramienta #windows #escalada-de-privilegios #red #activedirectory #ad 

## Descripción del Funcionamiento Interno
`Evil-WinRM` es una herramienta diseñada específicamente para la explotación de servidores Windows que tienen el servicio Windows Remote Management (WinRM) habilitado y configurado. Esta herramienta proporciona una interfaz de línea de comandos que facilita la interacción con el servidor, permitiendo la ejecución de comandos y scripts, transferencia de archivos, y varias otras funciones útiles durante una evaluación de seguridad o un pentest. Internamente, `Evil-WinRM` utiliza la biblioteca `WinRM` de Ruby para comunicarse con el servidor remoto, y proporciona una variedad de funcionalidades para explotar vulnerabilidades y elevar privilegios.

## Uso
`Evil-WinRM` se utiliza principalmente para interactuar con servidores Windows que tienen el servicio WinRM habilitado, lo cual es común en entornos de Active Directory. Permite a los atacantes o pentesters ejecutar comandos, transferir archivos, y realizar otras acciones en el servidor remoto con facilidad.

## Sintaxis
```bash
evil-winrm -i <ip/direccion_del_servidor> -u <usuario> -p <contraseña>
```
- `-i`: Especifica la dirección IP o nombre del servidor.
- `-u`: Nombre de usuario para la autenticación.
- `-p`: Contraseña para la autenticación.

## Ejemplos

### Conectar a un Servidor Remoto
```bash
evil-winrm -i 192.168.1.10 -u Administrator -p 'Password123!'
```
Este comando establece una conexión con el servidor en `192.168.1.10` utilizando las credenciales del usuario `Administrator`.

### Ejecutar un Comando Remoto
Una vez conectado:
```bash
*Evil-WinRM* PS C:\Users\Administrator\Documents> whoami
```
Ejecuta el comando `whoami` en el servidor remoto.

### Transferir un Archivo al Servidor Remoto
Una vez conectado:
```bash
*Evil-WinRM* PS C:\Users\Administrator\Documents> upload C:\path\to\local\file.txt C:\path\to\remote\destination\file.txt
```
Transfiere un archivo desde la máquina local al servidor remoto.


