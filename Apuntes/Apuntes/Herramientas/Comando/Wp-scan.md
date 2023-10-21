# Herramienta `wp-scan`

tags: #herramienta #escaneo-enumeracion #activa #comando #wordpress #web #cms

## Descripción del Funcionamiento Interno
`wp-scan` es una herramienta de escaneo de seguridad para WordPress que detecta vulnerabilidades conocidas en plugins, temas y la propia instalación de WordPress.

## Uso
Es utilizado por administradores de sitios web y evaluadores de seguridad para identificar problemas de seguridad en sitios WordPress.

## Sintaxis
```bash
wp-scan --url <URL> [opciones]
```

## Ejemplos


### Escaneo basico
```bash
wp-scan --url https://example.com
```
### Enumeracion de usuarios
```bash
wp-scan --url https://example.com --enumerate u
```

### Enumeracion de plugins
```bash
wp-scan --url https://example.com --enumerate p
```
### Enumeracion de temas
```bash
wp-scan --url https://example.com --enumerate t
```

### Escaneo agresivo 

```bash
wp-scan --url https://example.com --enumerate at
```

### Updatear base de datos
```bash
wp-scan --update
```
