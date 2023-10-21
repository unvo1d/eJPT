# Herramienta `openssl s_client`

tags: #herramienta #escaneo-enumeracion #activa #comando #ssl #tls

## Descripción del Funcionamiento Interno
`openssl s_client` es una herramienta de línea de comandos que permite conectar con servidores SSL/TLS, obtener información sobre la configuración y los certificados del servidor.

## Uso
Se utiliza para la recolección activa de información sobre la configuración SSL/TLS de un servidor.

## Sintaxis
```bash
openssl s_client -connect <hostname:port> [opciones]
```

## Ejemplos

### Obtencion de info del certificado

```bash
openssl s_client -connect example.com:443
```

Se mostrara info y configuracion SSL del servidor example.com

