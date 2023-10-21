# Herramienta `magescan`

tags: #herramienta #escaneo-enumeracion #activa #comando #web #magento #cms 

## Descripción del Funcionamiento Interno
`magescan` es una herramienta destinada a escanear sitios web que utilizan la plataforma Magento para evaluar la calidad y la seguridad del sitio, especialmente cuando no se tiene acceso directo al mismo. Por ejemplo, puede ser utilizado cuando se está entrevistando a un posible desarrollador o evaluando a un nuevo cliente, y se desea tener una idea de la calidad y seguridad del sitio que han desarrollado o están administrando&#8203;``【oaicite:5】``&#8203;&#8203;``【oaicite:4】``&#8203;.

## Uso
Se utiliza para ejecutar varios escaneos en un sitio web Magento especificado para recopilar información sobre la configuración del sitio, los módulos instalados, y otras características que pueden ser de interés desde un punto de vista de seguridad y calidad.

## Sintaxis
```bash
magescan.phar scan:all [--insecure|-k] [--show-modules] <url>
```
- `--insecure|-k`: Si se establece, los certificados SSL no serán validados.
- `--show-modules`: Lista todos los módulos buscados, no solo los encontrados.
- `<url>`: La URL del sitio Magento que se desea escanear​[3](https://www.kitploit.com/2018/03/magescan-scan-magento-site-for.html#:~:text=scan%3Aall%20%24%20magescan.phar%20scan%3Aall%20%5B,not%20just%20those%20found%20scan%3Acatalog)​​[4](https://www.buaq.net/go-637.html#:~:text=Usage%20%24%20magescan,SSL%20certificates%20won%27t%20be%20validated)​

## Ejemplos

### Todos los escaneos
```bash
magescan.phar scan:all store.example.com
```
### Formato de salida diferente
```bash
magescan.phar scan:all --format=json store.example.com
```

### Listar todos los modulos buscados(No solo los encontrados)
```bash
magescan.phar scan:all --show-modules store.example.com
```
