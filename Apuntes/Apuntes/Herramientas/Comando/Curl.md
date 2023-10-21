# Herramienta `curl`

tags: #herramienta #escaneo-enumeracion #activa #comando #web 

## Descripción del Funcionamiento Interno
`curl` es una herramienta de línea de comandos para transferir datos con URL sintaxis, soportando DICT, FILE, FTP, FTPS, Gopher, HTTP, HTTPS, IMAP, IMAPS, LDAP, LDAPS, POP3, POP3S, RTMP, RTSP, SCP, SFTP, SMB, SMBS, SMTP, SMTPS, Telnet y TFTP.

## Uso
Utilizado para hacer solicitudes HTTP/HTTPS, descargar o subir archivos, y explorar la respuesta de servidores web.

## Sintaxis
```bash
curl [opciones] <URL>
```

## Ejemplos

### Peticion GET
```bash
curl http://example.com
```
### Peticion POST 
```bash
curl -d "param1=value1&param2=value2" -X POST http://example.com/resource
```
### Custom Header
```bash
curl -H "X-MyHeader: 123" http://example.com
```
### Auth basica 
```bash
curl --user username:password http://example.com
```
### Seguir redirects
```bash
curl -L http://example.com
```
### Mostrar headers de response
```bash
curl -I http://example.com
```