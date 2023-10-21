# Herramienta `sslyze`

tags: #herramienta #escaneo-enumeracion #activa #comando #ssl #tls

## Descripción del Funcionamiento Interno
`sslyze` es una herramienta de análisis de configuración SSL/TLS que puede evaluar servidores web, servidores de correo, servidores XMPP y otros. Realiza pruebas exhaustivas en las configuraciones SSL/TLS, analizando las versiones de protocolos soportadas, cifrados, certificados, y otras configuraciones relacionadas con SSL/TLS.

## Uso
Utilizado por administradores de sistemas y profesionales de seguridad para evaluar y mejorar la configuración SSL/TLS de servidores, y para descubrir posibles vulnerabilidades o malas configuraciones.

## Sintaxis
```bash
sslyze <opciones> <hostname:port>
```

## Ejemplos 

### Escaneo regular

```bash
sslyze --regular example.com:443
```

### Escaneo de certificados 
```bash
sslyze --certinfo_full example.com:443
```

### Escaneo de cifrados
```bash
sslyze --tlsv1 --hide_rejected_ciphers example.com:443
```
### Escaneo de renegociacion
```bash
sslyze --reneg example.com:443
```
### Escaneo de vulnerabilidad heartbleed
```bash
sslyze --heartbleed example.com:443
```
### Escaneo de resumen de versiones de protocolo

```bash
sslyze --sslv2 --sslv3 --tlsv1 --tlsv1_1 --tlsv1_2 example.com:443
```