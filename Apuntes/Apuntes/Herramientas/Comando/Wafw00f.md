# Herramienta `WAFW00F`

tags: #herramienta #information-gathering #activa #comando #waf

## Descripción del Funcionamiento Interno
`WAFW00F` es una herramienta de línea de comandos diseñada para identificar y detectar firewalls de aplicaciones web (WAF) en sitios web. Realiza una serie de pruebas y análisis heurísticos para determinar la presencia de un WAF y, si es posible, identificar el tipo de WAF utilizado.

## Uso
Se utiliza para la recolección pasiva y activa de información sobre la presencia y tipo de firewalls de aplicaciones web en un sitio, lo que puede ser útil para investigaciones de seguridad, análisis de vulnerabilidades y planificación de pruebas de penetración.

## Sintaxis
```bash
wafw00f <url> [opciones]
```

## Ejemplos

### Deteccion de WAF

```bash
wafw00f http.example.com
```

### Especificar una pagina particular

```bash
wafw00f http://example.com/pagina.html
```

### Guardar resultados

```bash
wafw00f http://example.com -o results.txt
```

### Especificar lista de agentes de usuario

```bash
wafw00f http://example.com --ua-file user-agents.txt
```

