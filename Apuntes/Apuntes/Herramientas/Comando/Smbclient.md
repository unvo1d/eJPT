# Herramienta `smbclient`

tags: #herramienta #escaneo-enumeracion #activa #comando #smb #red

## Descripción del Funcionamiento Interno
`smbclient` es una herramienta de línea de comandos que permite a los usuarios acceder a recursos compartidos en servidores SMB/CIFS, similar a cómo lo haría un cliente de Windows. Permite explorar comparticiones, descargar, subir y eliminar archivos, entre otras operaciones.

## Uso
Utilizado para interactuar con servidores SMB/CIFS, lo que es útil para descubrir recursos compartidos y potenciales vectores de ataque en una red.

## Sintaxis
```bash
smbclient //[hostname]/[share] -U [username]
```

## Ejemplos

### Listar shares

```bash
smbclient -L //example.com -U username
```
### Conectarse a un share

```bash
smbclient //example.com/share -U username
```
### Descargar

```bash
smbclient //example.com/share -U username -c 'get filename'
```
### Subir 

```bash
smbclient //example.com/share -U username -c 'put filename'
```
### Ejecutar comando

```bash
smbclient //example.com/share -U username -c '!"command"'
```