# Herramienta `Hunter.io`

tags: #herramienta #information-gathering #pasiva #web #add-on #website

## Descripción del Funcionamiento Interno
`Hunter.io` es una plataforma en línea que proporciona servicios de búsqueda de direcciones de correo electrónico asociadas con un dominio específico. Utiliza una variedad de métodos para encontrar y verificar direcciones de correo electrónico, incluyendo la búsqueda en web, la verificación de patrones comunes de correo electrónico y la validación de la estructura de los correos encontrados.

## Uso
Se utiliza para la recolección pasiva de direcciones de correo electrónico asociadas con un dominio particular, lo que puede ser útil para investigaciones de OSINT (Open Source Intelligence) o campañas de phishing.

## Sintaxis
El uso principal de `Hunter.io` es a través de su interfaz web en [https://hunter.io](https://hunter.io), aunque también ofrece una API para la automatización de consultas.

- **Interfaz Web:**
   1. Accede a [https://hunter.io](https://hunter.io)
   2. Ingresa el dominio que deseas investigar.
   3. Presiona "Enter" o haz clic en "Find email addresses".

- **API:**
   La API de `Hunter.io` permite realizar consultas automatizadas y acceder a otras funciones del servicio. La documentación completa de la API se encuentra disponible en [https://hunter.io/api-documentation](https://hunter.io/api-documentation).

## Ejemplos

1. **Búsqueda de Correos Electrónicos en un Dominio Específico:**
   - Accede a [https://hunter.io](https://hunter.io)
   - Ingresa `example.com` en el campo de búsqueda.
   - Presiona "Enter" o haz clic en "Find email addresses".
   
   Resultado: Se mostrará una lista de direcciones de correo electrónico asociadas con `example.com`.

2. **Uso de la API para Buscar Correos Electrónicos:**
   Suponiendo que tienes una clave API de `Hunter.io`, puedes usar la siguiente sintaxis para buscar correos electrónicos:
   ```bash
   curl -X GET "https://api.hunter.io/v2/domain-search?domain=example.com&api_key=your_api_key"
