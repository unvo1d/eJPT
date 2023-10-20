# Herramienta `Chisel`

tags: #herramienta #tunelizacion #red #comando #pivoting 

## Descripción del Funcionamiento Interno
`Chisel` es una herramienta de línea de comandos rápida para crear túneles TCP seguros sobre HTTP. Utiliza la biblioteca `yamux` para la multiplexación de la conexión y `nhooyr.io/websocket` para el transporte sobre HTTP. `Chisel` puede ser utilizado para crear varios túneles a través de una sola conexión WebSocket.

## Uso
Se utiliza para tunelizar tráfico TCP a través de proxies HTTP, lo que puede ser útil para evadir firewalls o para conectar redes o sistemas de manera segura a través de Internet.

## Sintaxis
```bash
chisel server [options]
chisel client <server> [tunnel]...
```
`server` comando para iniciar el servidor chisel
`client`  comando para iniciar el cliente chisel
`server` la direccion del server chisel
`tunel` definiciones de tunel en el formato `local_address:remote_address`
## Ejemplos

### Iniciar servidor Chisel

```bash
chisel server --reverse
```
inicia un servidor chisel que permite conexiones reversas
### Crear un tunel 

```bash
chisel client http://server.example.com:8080 8080:localhost:80
```
Crea un tunel desde el puerto 8080 del cliente al puerto 80 del servidor
### Crear multiples tuneles 

```bash
chisel client http://server.example.com:8080 8080:localhost:80 8081:localhost:22
```
Crea dos tuneles, uno al puerto 80 y otro al puerto 22 del servidor local

### Especificar opciones del servidor

```bash
chisel server --port 8080 --key mykey --auth user:pass
```

Inicia un servidor chisel en el puerto 8080 con una clave y una autenticacion concretas