# Reaver

Tags: #activo #herramienta #bruteforce #wireless #wps

## Descripción
Reaver es una herramienta de línea de comandos de código abierto que se utiliza para realizar ataques de fuerza bruta en routers con Wi-Fi Protected Setup (WPS) habilitado. Su objetivo principal es descifrar la clave precompartida WPA/WPA2 de una red Wi-Fi explotando el protocolo WPS. Reaver ha sido diseñado para ser robusto y práctico, y ha sido probado contra una amplia variedad de puntos de acceso y implementaciones de WPS&#8203;``【oaicite:3】``&#8203;.

## Funcionamiento Interno
Reaver lleva a cabo un ataque de fuerza bruta contra el número de PIN de configuración protegida de Wi-Fi (WPS) de un punto de acceso. Una vez que se encuentra el PIN de WPS, se puede recuperar la clave PSK de WPA y, alternativamente, se pueden reconfigurar las configuraciones inalámbricas del punto de acceso&#8203;``【oaicite:2】``&#8203;. Por defecto, cuando se detecta un estado bloqueado, Reaver verificará el estado cada 315 segundos (5 minutos y 15 segundos) y no continuará forzando los PIN hasta que el estado de WPS esté desbloqueado. Este chequeo puede ser incrementado o decrementado a cualquier valor entero no negativo, utilizando la opción `--lock-delay`&#8203;``【oaicite:1】``&#8203;.

## Uso
Para utilizar Reaver, es necesario poner el adaptador inalámbrico en modo monitor, identificar el BSSID del punto de acceso objetivo y luego ejecutar Reaver con las opciones deseadas. A continuación se muestra un ejemplo de uso de Reaver para atacar un punto de acceso específico, mostrando salida detallada:

```bash
root@kali:~# reaver -i wlan0mon -b E0:3F:49:6A:57:78 -v
```

### Opciones Comunes

- `-i, --interface=<wlan>`: Nombre de la interfaz en modo monitor a utilizar.
- `-b, --bssid=<mac>`: BSSID del punto de acceso objetivo.
- `-v, --verbose`: Mostrar advertencias no críticas.
- `-p, --pin=<wps pin>`: Utilizar el pin especificado.
- `-d, --delay=<seconds>`: Establecer el retardo entre intentos de pin.
- `-l, --lock-delay=<seconds>`: Establecer el tiempo de espera si el punto de acceso bloquea los intentos de pin.
- `-g, --max-attempts=<num>`: Salir después de un número especificado de intentos de pin.
- `-x, --fail-wait=<seconds>`: Establecer el tiempo de espera después de 10 fallos inesperados.
- `-A, --no-associate`: No asociarse con el punto de acceso (la asociación debe ser realizada por otra aplicación)​[2](https://www.kali.org/tools/reaver/)​.

