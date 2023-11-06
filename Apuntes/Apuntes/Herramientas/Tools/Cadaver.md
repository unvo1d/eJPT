# `Cadaver`

tags: #herramienta #web #red #webdav #linux

## Descripción del Funcionamiento Interno
`Cadaver` es un cliente de línea de comandos para el protocolo WebDAV. Permite a los usuarios navegar por servidores WebDAV, realizar operaciones de transferencia de archivos, y ejecutar comandos de administración remota. Internamente, `Cadaver` utiliza la biblioteca `neon` para comunicarse con los servidores WebDAV, proporcionando soporte para operaciones básicas de HTTP y WebDAV, incluyendo la autenticación, la transferencia de archivos y la manipulación de recursos en el servidor.

## Uso
Se utiliza para interactuar con servidores WebDAV desde la línea de comandos, lo que puede ser útil para administradores de sistemas, desarrolladores y profesionales de la seguridad para gestionar recursos, subir o descargar archivos, y realizar pruebas de seguridad.

## Sintaxis
```bash
cadaver [options] [url]
```
- `[options]`: Opciones de configuración para `Cadaver`.
- `[url]`: URL del servidor WebDAV al que conectarse.

## Ejemplos

### Conectar a un Servidor WebDAV
```bash
cadaver http://webdav.example.com/
```
Este comando inicia `Cadaver` y se conecta al servidor WebDAV en `http://webdav.example.com/`.

### Subir un Archivo
Dentro de la interfaz de `Cadaver`:
```bash
put localfile.txt remotefile.txt
```
Sube `localfile.txt` del sistema local al servidor WebDAV, guardándolo como `remotefile.txt`.

### Descargar un Archivo
Dentro de la interfaz de `Cadaver`:
```bash
get remotefile.txt localfile.txt
```
Descarga `remotefile.txt` del servidor WebDAV al sistema local, guardándolo como `localfile.txt`.

### Listar Contenido del Directorio
Dentro de la interfaz de `Cadaver`:
```bash
ls
```
Muestra el contenido del directorio actual en el servidor WebDAV.

Recuerda utilizar `Cadaver` de manera ética y asegurarte de tener los permisos necesarios para interactuar con los servidores WebDAV.
