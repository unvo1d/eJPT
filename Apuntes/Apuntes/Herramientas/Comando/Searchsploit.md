# Searchsploit

Tags: #activo #herramienta #explotación

## Descripción
Searchsploit es una herramienta de búsqueda de exploits desarrollada por Offensive Security, Unix Ninja y G0tmi1k. Permite a los usuarios realizar búsquedas detalladas offline a través de una copia local del repositorio Exploit Database. Esta capacidad es especialmente útil para evaluaciones de seguridad en redes segregadas o aisladas sin acceso a Internet. Es una herramienta de línea de comandos que se ejecuta en sistemas Unix y permite la búsqueda de exploits por término o términos relacionados con una vulnerabilidad particular.

## Funcionamiento Interno
Searchsploit opera mediante una interfaz de línea de comandos, permitiendo a los usuarios buscar exploits usando una o más palabras clave. La herramienta utiliza un operador AND, no un operador OR, lo que significa que cuantos más términos se usen, más se filtrarán los resultados. Además, Searchsploit puede buscar tanto en el título del exploit como en la ruta, aunque esta funcionalidad puede ser restringida a los títulos usando la opción `-t`. También proporciona una opción `--exclude` para eliminar resultados no deseados de la búsqueda, y los términos a excluir se pueden separar con una barra vertical (`|`) para excluir múltiples términos a la vez.

## Uso
Para hacer uso de Searchsploit, simplemente se deben agregar los términos de búsqueda deseados a la línea de comandos. A continuación, se presentan algunas opciones comunes y ejemplos de uso basados en la información recopilada:

### Opciones Comunes
- `-h`: Muestra todas las características y opciones disponibles.
- `-t`: Restringe la búsqueda solo a los títulos de los exploits.
- `--exclude`: Excluye resultados no deseados de la búsqueda.

### Ejemplos de Uso
```bash
searchsploit afd windows local
searchsploit -t oracle windows
searchsploit -p 39446
searchsploit linux kernel 3.2 --exclude=" (PoC)|/dos/"
searchsploit -s Apache Struts 2.0.0
searchsploit linux reverse password
```

- Para realizar una búsqueda básica, simplemente agregue cualquier número de términos de búsqueda que desee buscar​[1](https://blog.certcube.com/searchsploit-cheat-sheet/)​.
- Para restringir la búsqueda solo a los títulos de los exploits, use la opción `-t`​[1](https://blog.certcube.com/searchsploit-cheat-sheet/)​.
- Para excluir resultados no deseados, use la opción `--exclude` y separe los términos a excluir con una barra vertical (`|`)​[1](https://blog.certcube.com/searchsploit-cheat-sheet/)​.

# Ejemplos adicionales de uso de Searchsploit

```bash
searchsploit linux kernel --exclude="(PoC)|/dos/" | grep ' 3.2'  # Este comando proporciona una salida “más limpia” (ordenada por versión sin encabezados/pies de página)&#8203;``【oaicite:0】``&#8203;.
```

