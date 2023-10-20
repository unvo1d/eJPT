---
tags: #Herramienta, #Information-Gathering, #Pasiva, #Web, #Red, #Comando
---
---

# Comando `host`


- Tags: #comando #herramienta  #information-gathering #pasiva #web #red
## Descripción del Funcionamiento Interno
El comando `host` es una utilidad simple de línea de comandos utilizada en sistemas Unix y Linux para realizar consultas DNS. Convierte nombres de dominio en direcciones IP y viceversa. Utiliza las bibliotecas de resolución del sistema para realizar las consultas, lo que significa que respeta el archivo `/etc/resolv.conf` y otras configuraciones del sistema.

## Uso
Se utiliza para obtener información DNS sobre un dominio, lo que puede incluir la dirección IP asociada, el servidor de nombres, el servidor de correo, entre otros. También es útil para descubrir subdominios y para el troubleshooting de problemas de red.

## Sintaxis
```bash
host [option] [name] [server]

'option' : modifica el comportamiento del comando
'name' : dominio o IP 
'server' : servidor DNS pa usar en la consulta 
```


## Ejemplos

1. **Consulta Básica:**
   ```bash
   host example.com

Devuelve ip asociada a example 

```

```host -t mx example.com

Devuelve los registros MX del dominio 
```

```host example.com 8.8.8.8

busca en el servidor DNS de google 
```

