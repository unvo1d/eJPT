# Herramienta `joomscan`

tags: #herramienta #escaneo-enumeracion #activa #comando #web #joomla #cms 

## Descripción del Funcionamiento Interno
`joomscan` es una herramienta diseñada para detectar vulnerabilidades en sitios que utilizan el CMS Joomla. Identifica problemas en la configuración, componentes instalados y temas, ayudando a los administradores y auditores de seguridad a encontrar posibles riesgos en estos sitios.

## Uso
Se utiliza para escanear sitios Joomla en busca de vulnerabilidades conocidas y configuraciones incorrectas.

## Sintaxis
```bash
perl joomscan.pl --url <URL> [opciones]
```

## Ejemplos

### Verificacion basica
```bash
perl joomscan.pl --url www.example.com
```
### Enumeracion componentes
```bash
perl joomscan.pl --url www.example.com --enumerate-components
```
### Establecer cookie
```bash
perl joomscan.pl --url www.example.com --cookie "test=demo;"
```
### Establecer user agent
```bash
perl joomscan.pl --url www.example.com --user-agent "Mozilla/5.0"
```