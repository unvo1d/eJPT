# Herramienta `dnsrecon`

tags: #herramienta #information-gathering #pasiva #comando #dns

## Descripción del Funcionamiento Interno
`dnsrecon` es una herramienta de línea de comandos diseñada para llevar a cabo análisis y recolección de datos DNS en los dominios. La herramienta incluye diversas opciones para especificar el tipo de información que se desea obtener, y puede llevar a cabo tareas como enumeración de subdominios, verificación de transferencias de zona, y búsqueda de registros DNS de diferentes tipos.

## Uso
Se utiliza para la recolección pasiva y activa de información sobre la configuración DNS de un dominio, lo que puede ser útil para investigaciones de OSINT (Open Source Intelligence), auditorías de seguridad y análisis de infraestructura de red.

## Sintaxis
```bash
dnsrecon -d <dominio> [opciones]
```

## Ejemplos 

### Enumeracion de subdominios

```bash
dnsrecon -d example.com -t brt
```

Mostrara una lista de subdominios encontrados para example.com
### Verificacion de transferencia de zona 

```bash
dnsrecon -d example.com -t axfr 
```

Verificara si las transferencias de zona estan permitidas y las mostrara si es posible

### Busqueda de Registros MX

```bash
dnsrecon -d example.com -t mx
```

Mostrara una lista de registros MX para example.com

### Busqueda de registros NS

```bash
dnsrecon -d example.com -t ns
```

Muestra la lista de registros de NS para example.com