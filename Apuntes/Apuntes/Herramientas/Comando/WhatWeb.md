# Herramienta `WhatWeb`

tags: #herramienta #information-gathering #pasiva #web #comando

## Descripción del Funcionamiento Interno
`WhatWeb` es una herramienta de línea de comandos que identifica las tecnologías utilizadas en sitios web, incluyendo el nombre del sistema operativo, el tipo de servidor web, los sistemas de gestión de contenido (CMS), los scripts, las cookies y mucho más. Utiliza plugins y técnicas de fingerprinting (huellas dactilares) para identificar las tecnologías, examinando el contenido de la página, las respuestas del servidor y otros datos.

## Uso
`WhatWeb` se utiliza para la recolección de información pasiva sobre las tecnologías utilizadas en un sitio web, lo cual puede ser útil para entender la estructura y las posibles vulnerabilidades de un sitio antes de realizar pruebas de penetración.

## Sintaxis
```bash
whatweb [options] [URLs]

'options' : para modificar el comportamiento del comando
```

## Ejemplos

```bash
whatweb example.com

'-v' Verbose 
```


```
whatweb -o results.txt example.com

'-o' guardar output en archivo
```


```
whatweb example.com example.org

'analisis de multiples sitios'
 ```



