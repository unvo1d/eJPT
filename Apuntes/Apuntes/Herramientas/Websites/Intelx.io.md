# Herramienta `Intelx.io`

tags: #herramienta #information-gathering #pasiva #web #website

## Descripción del Funcionamiento Interno
`Intelx.io` es una plataforma en línea que proporciona servicios de búsqueda avanzada y análisis de datos en la web abierta y en la dark web. Permite a los usuarios realizar búsquedas en una amplia variedad de fuentes, incluyendo dominios, direcciones IP, hashes, y otros identificadores. `Intelx.io` indexa datos de diversas fuentes y proporciona herramientas para analizar y explorar los datos encontrados.

## Uso
Se utiliza para la recolección pasiva de información en investigaciones de OSINT (Open Source Intelligence), incluyendo la identificación de información relacionada con dominios, IP, o cualquier otro identificador en la web abierta y en la dark web.

## Sintaxis
El uso principal de `Intelx.io` es a través de su interfaz web en [https://intelx.io/](https://intelx.io/), aunque también ofrece una API para la automatización de consultas.

- **Interfaz Web:**
   1. Accede a [https://intelx.io/](https://intelx.io/)
   2. Ingresa el identificador que deseas investigar (por ejemplo, un dominio, una dirección IP, un hash, etc.).
   3. Presiona "Enter" o haz clic en "Search".

- **API:**
   La API de `Intelx.io` permite realizar consultas automatizadas y acceder a otras funciones del servicio. La documentación completa de la API se encuentra disponible en [https://intelx.io/documentation](https://intelx.io/documentation).

## Ejemplos

1. **Búsqueda de Información Relacionada con un Dominio:**
   - Accede a [https://intelx.io/](https://intelx.io/)
   - Ingresa `example.com` en el campo de búsqueda.
   - Presiona "Enter" o haz clic en "Search".
   
   Resultado: Se mostrará una lista de información relacionada con `example.com` incluyendo, posiblemente, subdominios, direcciones IP asociadas, y otros datos.

2. **Uso de la API para Buscar Información:**
   Suponiendo que tienes una clave API de `Intelx.io`, puedes usar la siguiente sintaxis para buscar información:
   ```bash
   curl -X GET "https://intelx.io/api?query=example.com&key=your_api_key"
