# Herramienta `Google Dorks`

tags: #herramienta #information-gathering #pasiva #web #busqueda

## Descripción del Funcionamiento Interno
`Google Dorks` no es una herramienta per se, sino una técnica de búsqueda avanzada que se utiliza en el motor de búsqueda de Google para encontrar información específica en sitios web. Consiste en utilizar operadores de búsqueda especiales que Google proporciona para filtrar los resultados de búsqueda y acceder a información que de otro modo podría ser difícil de encontrar.

## Uso
Se utiliza para la recolección pasiva de información sobre sitios web, servidores, archivos, directorios, o cualquier otro dato que pueda estar indexado por Google. Es especialmente útil para encontrar información sensible que haya sido expuesta accidentalmente en la web.

## Sintaxis
La sintaxis de `Google Dorks` consiste en operadores de búsqueda avanzados. Algunos de los operadores más comunes incluyen:

- `site:`: Restringe los resultados de búsqueda a un dominio específico.
- `filetype:`: Busca archivos de un tipo específico.
- `inurl:`: Busca palabras específicas en la URL.
- `intext:`: Busca palabras específicas en el texto de la página.

## Ejemplos

1. **Buscar archivos PDF en un sitio específico:**
   ```plaintext
   site:example.com filetype:pdf
   ```

2. **Buscar paginas con una URL especifica**

```
inurl:admin
```

3. **Buscar texto especifico en la pagina**
```
intext:"confidential"
```


4. **Combinar operadores** 

```
site:example.com intext:"email" filetype:txt
```