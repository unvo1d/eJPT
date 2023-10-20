# Herramienta `nmap`

tags: #herramienta #escaneo-enumeracion #activa #comando #red

## Descripción del Funcionamiento Interno
`nmap` es una herramienta de línea de comandos para exploración de redes y auditoría de seguridad. Realiza descubrimiento de hosts, escaneo de puertos, detección de servicios y versiones, y muchas otras tareas de análisis de red.

## Uso
Se utiliza para el escaneo activo y enumeración de redes, descubrimiento de hosts y servicios, y análisis de seguridad.

## Sintaxis
```bash
nmap [opciones] <objetivo>
```

## Flags mas usados

- `-sS`: Escaneo SYN.
- `-sT`: Escaneo TCP connect.
- `-sU`: Escaneo UDP.
- `-p`: Especifica rango de puertos.
- `-Pn`: No hacer ping, asume que el host está activo.
- `-F`: Escaneo rápido.
- `-T`: Controla la velocidad del escaneo (p. ej., `-T4` para un escaneo más rápido).
- `-oX`: Guarda la salida en formato XML.
- `-v`: Salida detallada (verbose).
- `-PE`: Escaneo ICMP Echo.
- `-A`: Escaneo agresivo.
- `-sC`: Ejecutar scripts por defecto de nmap.
- `-sV`: Detección de versión de servicios.
- `-sC -sV`: Combinación de detección de versión de servicios y ejecución de scripts por defecto.
- `--script`: Ejecuta un script específico o una categoría de scripts de la base de datos de scripts de nmap (e.g., `--script=vuln` para ejecutar scripts de vulnerabilidades).
- `-sN`: es utilizada para un escaneo TCP NULL. Este tipo de escaneo envía paquetes TCP con las banderas de control desactivadas. Es decir, todos los bits de las banderas (como SYN, ACK, FIN, etc.) están desactivados. Este tipo de escaneo puede ser útil para evadir ciertas detecciones de firewall o IDS (Sistema de Detección de Intrusiones), aunque no todos los sistemas operativos o dispositivos responden de manera predecible a estos paquetes.