# Herramienta `Sublist3r`

tags: #herramienta #information-gathering #pasiva #comando #subdominios

## Descripción del Funcionamiento Interno
`Sublist3r` es una herramienta de línea de comandos diseñada para enumerar subdominios de sitios web mediante el uso de múltiples fuentes como motores de búsqueda, y servicios de recolección de datos DNS.

## Uso
Se utiliza para la recolección pasiva de información sobre subdominios asociados con un dominio principal.

## Sintaxis
```bash
sublist3r -d <dominio> [opciones]
```

## Ejemplos

### Enumeracion de subdominios

```bash
sublist3r -d example.com
```


### Opciones 

- `-e`: Especifica los motores de búsqueda para la enumeración.
- `-o`: Especifica un archivo de salida para guardar los resultados.
- `-v`: Habilita la salida detallada (verbose).
- `--threads`: Especifica el número de hilos (threads) a us

```bash
sublist3r -d example.com -e google,bing -o output.txt
```
