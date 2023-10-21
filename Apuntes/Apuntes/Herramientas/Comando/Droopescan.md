# Herramienta `droopescan`

tags: #herramienta #escaneo-enumeracion #activa #cms #web #comando

## Descripción del Funcionamiento Interno
`droopescan` es una herramienta diseñada para acelerar la fase inicial de reconocimiento de un sitio web que utiliza alguno de los sistemas de gestión de contenido (CMS) específicos. Los CMS soportados varían en cuanto a las funcionalidades que `droopescan` puede explorar:
- **Drupal**: Identifica plugins y temas instalados, rutas de interés para un atacante (como el panel de login o el archivo de registro de cambios), y la versión de Drupal utilizada&#8203;``【oaicite:4】``&#8203;.
- **Joomla y WordPress**: Identifica rutas de interés para un atacante y la versión del sistema utilizado&#8203;``【oaicite:3】``&#8203;.
- **Moodle**: Reconoce plugins y temas instalados, y la versión del CMS en uso&#8203;``【oaicite:2】``&#8203;.
- **Silverstripe**: Identifica plugins y temas instalados, rutas de interés para un atacante, y la versión de Silverstripe utilizada&#8203;``【oaicite:1】``&#8203;.

## Uso
`droopescan` se utiliza para identificar problemas en sitios web basados en los CMS mencionados anteriormente. Es especialmente útil para la identificación de problemas en instalaciones de Drupal, SilverStripe y WordPress&#8203;``【oaicite:0】``&#8203;.

## Sintaxis
La sintaxis básica para el uso de `droopescan` es la siguiente:
```bash
droopescan scan {cms} -u {URL} [opciones]
```

`cms` el CMS que deseas escanear 

## Ejemplos

### Escaneo basico
```bash
droopescan scan drupal -u example.com
droopescan scan wordpress -u example.org
```
### Escaneo multiples URL
```bash
droopescan scan drupal -U list_of_urls.txt
droopescan scan silverstripe -U list_of_urls.txt
```
### Especificando el tipo de peticion
```bash
droopescan scan --number {NUMBER}
droopescan scan -n {NUMBER}
```
### Modo depuracion y silencio
```bash
droopescan scan --debug
droopescan scan --quiet
```