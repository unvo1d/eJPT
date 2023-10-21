# Herramienta `linux-smart-enumeration`

tags: #herramienta #escaneo-enumeracion #activa  #comando #linux #escalada-de-privilegios

## Descripción del Funcionamiento Interno
`linux-smart-enumeration` (lse) es una herramienta diseñada para ayudar en la enumeración de sistemas Linux durante pruebas de penetración y competencias de Capture The Flag (CTF). El script tiene diferentes niveles de verbosidad, lo que permite controlar cuánta información se muestra. En el nivel de verbosidad predeterminado, se muestran los defectos de seguridad altamente importantes en el sistema.

## Uso
Lse proporciona información relevante sobre la seguridad del sistema Linux local, lo que puede ayudar en la escalación de privilegios.

## Sintaxis
```bash
./lse.sh [opciones]
```

- `-c`: Deshabilita el color.
- `-i`: Modo no interactivo.
- `-l LEVEL`: Nivel de verbosidad de la salida (0: muestra resultados altamente importantes; 1: muestra resultados interesantes; 2: muestra toda la información recopilada).
- `-s SELECTION`: Lista separada por comas de secciones o pruebas a ejecutar.
- `-e PATHS`: Lista separada por comas de rutas a excluir para realizar escaneos más rápidos.
- `-p SECONDS`: Tiempo que el monitor de procesos pasará observando procesos.
- `-S`: Sirve el script `lse.sh` en este host para que pueda ser recuperado desde un host remoto.

## Ejemplos


### Ejecucion directa 

```bash
bash <(wget -q -O - "https://github.com/diego-treitos/linux-smart-enumeration/releases/latest/download/lse.sh") -l2 -i

bash <(curl -s "https://github.com/diego-treitos/linux-smart-enumeration/releases/latest/download/lse.sh") -l1 -i

```

### Verbosidad

- **Nivel 0 (Predeterminado)**: Muestra información altamente importante que puede ser utilizada en una escalación de privilegios.
- **Nivel 1**: Muestra información interesante que puede ayudar en la escalación de privilegios.
- **Nivel 2**: Muestra toda la información recopilada sobre el sistema​[6](https://www.treitos.com/blog/2019/linux-smart-enumeration.html#:~:text=For%20that%20reason%20I%20ended,to%20see%20the%20different%20vulnerabilities)​.

