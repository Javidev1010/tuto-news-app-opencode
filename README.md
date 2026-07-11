"""# News CLI - Lector de Noticias en Consola

El objetivo de esta aplicación es crear una herramienta de línea de comandos (CLI) en Python que permita a los usuarios consultar las últimas noticias globales utilizando la API de NewsAPI. La aplicación interactúa con el usuario mediante un menú en consola, permitiendo la búsqueda personalizada por temas e idiomas, además de ofrecer la posibilidad de guardar una configuración de búsqueda de noticias por defecto.

Al finalizar el desarrollo se debe permitir opcionalmente su empaquetado en un binario ejecutable.

---

## Opciones del Sistema

La aplicación desplegará un menú en consola como sigue:

1. Mostrar noticias default
2. Consultar nuevas noticias: Solicitará al usuario el tema que sera el parametro q y el idioma parametro language del api url
3. Establecer noticias por defecto: Permite registrar y almacenar de manera persistente un tema y un idioma específicos para que se consulte en el punto 1 del menu
4. Borrar configuración default
5. Salir

---

## Stack Tecnológico

- Lenguaje Python 3.10 o superior
- Gestión de Peticiones HTTP
- API de Datos: NewsAPI free
- Empaquetado: Generar un binario ejecutable

---

## Ejemplo de Petición HTTP

La aplicación se comunicará directamente con el endpoint /v2/everything de NewsAPI. Un ejemplo real del formato de URL es el siguiente:

https://newsapi.org/v2/everything?q=mundial2026&language=es&pageSize=5&apiKey=123abc

https://newsapi.org/v2/everything?q=sismo&language=es&pageSize=5&apiKey=123abc

donde q es el tema de interes y language el idioma
