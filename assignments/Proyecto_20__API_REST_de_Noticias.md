# Proyecto 20 | API REST de Noticias

**📅 Created:** July 04, 2024 at 05:15 AM  
**📅 Updated:** July 05, 2024 at 04:44 AM  
**🔗 Original Link:** [View in Classroom](https://classroom.google.com/c/Njk1MDgxNzAyMTIx/a/Njk3NzY2MTYyODE1/details)  
**👤 Created by:** Adrián Fernando Gaitán Londoño
**🆔 Creator ID:** 100957882007157850038
**📊 Max Points:** N/A  

**📅 Due Date:** {'year': 2024, 'month': 7, 'day': 5}

---

## 📝 Description

Este contrato define los requisitos y especificaciones para el desarrollo de una API REST que interactúa con un proveedor de noticias (como Event Registry). La API permitirá obtener artículos, eventos destacados, detalles de artículos específicos y flujos de noticias en tiempo real. La API debe seguir las mejores prácticas RESTful y asegurar que las claves secretas (API keys) no se expongan al cliente. [https://www.newsapi.ai/documentation?tab=introduction](https://www.newsapi.ai/documentation?tab=introduction)

1. Endpoints y Parámetros
1.1. Obtener Artículos
Método HTTP: GET
Ruta del Endpoint: `/api/articles`
Descripción: Recupera una lista de artículos de noticias basados en los parámetros de búsqueda y filtrado proporcionados.
Parámetros:
Query Parameters:
`query` (string) - Término de búsqueda para filtrar artículos por palabra clave.
`category` (string) - Categoría de noticias para filtrar (por ejemplo, `technology`, `sports`).
`language` (string) - Código de idioma (ISO 639-1). Por defecto, `en`.
`page` (int) - Número de página para la paginación. Por defecto, `1`.
`pageSize` (int) - Número de artículos por página. Por defecto, `10`.
`fromDate` (string) - Fecha de inicio para filtrar artículos (`YYYY-MM-DD`).
`toDate` (string) - Fecha de finalización para filtrar artículos (`YYYY-MM-DD`).

1.2. Obtener Eventos Destacados (Breaking Events)
Método HTTP: GET
Ruta del Endpoint: `/api/breaking-events`
Descripción: Recupera una lista de eventos de última hora basados en los parámetros de búsqueda y filtrado proporcionados.
Parámetros:
Query Parameters:
`language` (string) - Código de idioma (ISO 639-1). Por defecto, `en`.
`region` (string) - Región geográfica para filtrar eventos.
`category` (string) - Categoría de eventos para filtrar (por ejemplo, `politics`, `health`).
`page` (int) - Número de página para la paginación. Por defecto, `1`.
`pageSize` (int) - Número de eventos por página. Por defecto, `10`.

1.3. Obtener Detalles de un Artículo
Método HTTP: GET
Ruta del Endpoint: `/api/articles/:id`
Descripción: Obtiene los detalles completos de un artículo específico.
Parámetros:
Path Parameter:
`:id` (string) - El identificador único del artículo.


2. Especificaciones de Seguridad
2.1. Manejo de Claves de API
Almacenamiento Seguro de Claves:
Las claves API deben almacenarse de forma segura en el servidor utilizando variables de entorno.
Las claves nunca deben ser expuestas al cliente ni ser parte de las respuestas de la API.

2.2. Manejo de Errores
Respuestas de Error:
Proporcionar respuestas detalladas y consistentes para los errores, evitando exponer información sensible.
Utilizar códigos de estado HTTP apropiados para indicar la naturaleza del error.

Registro de Errores:
Registrar todos los errores y excepciones para facilitar la auditoría y el monitoreo de la API.

3. Documentación y Pruebas
3.1. Documentación
Documentación API:
Proporcionar una documentación detallada y clara de los endpoints, parámetros y respuestas en la ruta principal de la API: `/api/`.
Utilizar herramientas como Swagger o OpenAPI para generar y mantener la documentación.

3.2. Pruebas
Postman Collection:
Crear y proporcionar una colección de Postman que contenga ejemplos de solicitudes y pruebas para todos los endpoints.
Asegurar que la colección de Postman esté bien documentada y fácil de usar para otros desarrolladores.

4. Consideraciones Adicionales
4.1. Buenas Prácticas REST
Estructura RESTful:
Seguir las mejores prácticas RESTful en el diseño y la implementación de los endpoints, asegurando que los métodos HTTP y los códigos de estado sean usados correctamente.

4.2. Monitoreo y Mantenimiento
Monitoreo de API:
Crear endpoint `/api/health`, que indique el estado de la API, si hay conexión con el servicio de [https://www.newsapi.ai/](https://www.newsapi.ai/)

Este contrato define las especificaciones técnicas y los requisitos para el desarrollo de una API REST segura y funcional que interactúa con un proveedor de noticias. Es esencial seguir estas directrices para asegurar una implementación exitosa y un uso seguro de la API.



## 📋 Assignment Details

**Work Type:** ASSIGNMENT  
**State:** PUBLISHED  
**Assignment Mode:** ALL_STUDENTS

---

*Assignment ID: 697766162815*
