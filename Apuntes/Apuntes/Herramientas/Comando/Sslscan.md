# Herramienta `sslscan`

tags: #herramienta #escaneo-enumeracion #activa #comando #ssl #tls

## Descripción del Funcionamiento Interno
`sslscan` es una herramienta de línea de comandos que permite explorar la configuración SSL/TLS de un servidor para identificar posibles problemas o inseguridades.

## Uso
Se utiliza para la recolección activa de información sobre la configuración SSL/TLS de un servidor.

## Sintaxis
```bash
sslscan <hostname:port> [opciones]
```

## Ejemplos

### Escaneo basico

```bash
sslscan example.com:443
```

### Muestra solo cifras y protocolos que el servidor acepta

```bash 
sslscan --no-failed example.com
```

