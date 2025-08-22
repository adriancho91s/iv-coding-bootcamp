# Proyecto 19 | API REST de Películas, TV Shows y People

**📅 Created:** July 04, 2024 at 05:06 AM  
**📅 Updated:** July 05, 2024 at 04:44 AM  
**🔗 Original Link:** [View in Classroom](https://classroom.google.com/c/Njk1MDgxNzAyMTIx/a/Njk3NzY1ODExNDcw/details)  
**👤 Created by:** Adrián Fernando Gaitán Londoño
**🆔 Creator ID:** 100957882007157850038
**📊 Max Points:** N/A  

**📅 Due Date:** {'year': 2024, 'month': 7, 'day': 5}

---

## 📝 Description

Este documento establece los requisitos y las especificaciones para el desarrollo de una API REST que interactúa con la API de The Movie Database (TMDb). La API debe permitir listar películas, series de televisión (TV shows) y personas (actors, directors, etc.), con capacidades avanzadas de filtrado y paginación, así como obtener detalles específicos de cada entidad. Se deben seguir las mejores prácticas para asegurar que las claves secretas (API keys) no se expongan al cliente y se mantenga una alta seguridad.

1. Endpoints y Parámetros

1.1. Listar Películas
Método HTTP: GET
Ruta del Endpoint: `/api/movies`
Descripción: Lista películas con opciones de paginación y filtrado por región, idioma, género y términos de búsqueda.
Parámetros:
Query Parameters:
`page` (int) - Número de página para la paginación. Por defecto, `1`.
`region` (string) - Código de región para filtrar películas por ubicación geográfica.
`language` (string) - Código de idioma (ISO 639-1). Por defecto, `en-US`.
`query` (string) - Término de búsqueda para filtrar películas por título o descripción.
`genre` (string) - Identificador de género para filtrar películas por género.

1.2. Obtener Detalles de una Película
Método HTTP: GET
Ruta del Endpoint: `/api/movies/:id`
Descripción: Obtiene los detalles completos de una película específica.
Parámetros:
Path Parameter:
`:id` (string) - El identificador de la película en la base de datos de TMDb.

1.3. Listar TV Shows
Método HTTP: GET
Ruta del Endpoint: `/api/tv`
Descripción: Lista series de televisión (TV shows) con opciones de paginación y filtrado por región, idioma, género y términos de búsqueda.
Parámetros:
Query Parameters:
`page` (int) - Número de página para la paginación. Por defecto, `1`.
`region` (string) - Código de región para filtrar TV shows por ubicación geográfica.
`language` (string) - Código de idioma (ISO 639-1). Por defecto, `en-US`.
`query` (string) - Término de búsqueda para filtrar TV shows por título o descripción.
`genre` (string) - Identificador de género para filtrar TV shows por género.


1.4. Obtener Detalles de un TV Show
Método HTTP: GET
Ruta del Endpoint: `/api/tv/:id`
Descripción: Obtiene los detalles completos de un TV show específico.
Parámetros:
Path Parameter:
`:id` (string) - El identificador del TV show en la base de datos de TMDb.

1.5. Buscar Personas (People)
Método HTTP: GET
Ruta del Endpoint: `/api/people`
Descripción: Busca personas (actores, directores, etc.) en la base de datos de TMDb.
Parámetros:
Query Parameters:
`language` (string) - Código de idioma (ISO 639-1). Por defecto, `en-US`.
`include_adult` (boolean) - Incluir contenido para adultos en los resultados. Por defecto, `false`.
`page` (int) - Número de página para la paginación. Por defecto, `1`.
`query` (string) - Término de búsqueda para filtrar personas por nombre.

1.6. Obtener Detalles de una Persona
Método HTTP: GET
Ruta del Endpoint: `/api/people/:id`
Descripción: Obtiene los detalles completos de una persona específica.
Parámetros:
Path Parameter:
`:id` (string) - El identificador de la persona en la base de datos de TMDb.

1.7. Obtener Contenido Trending
Método HTTP: GET
Ruta del Endpoint: `/api/trending/:type`
Descripción: Obtiene contenido trending para películas, TV shows o personas.
Parámetros:
Path Parameter:
`:type` (string) - Tipo de contenido trending que se desea obtener. Valores posibles: `movie`, `tv`, `person`.
Query Parameters:
`time_window` required * (string) - Período de tiempo para el contenido trending. Valores posibles: `day`, `week`. Por defecto, `day`.

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

3.2. Pruebas
Postman Collection:
Crear y proporcionar una colección de Postman que contenga ejemplos de solicitudes y pruebas para todos los endpoints.
Asegurar que la colección de Postman sea fácil de usar para otros desarrolladores.

4. Consideraciones Adicionales
4.1. Buenas Prácticas REST

Estructura RESTful:
Seguir las mejores prácticas RESTful en el diseño y la implementación de los endpoints, asegurando que los métodos HTTP y los códigos de estado sean usados correctamente.

Este contrato define las especificaciones técnicas y los requisitos para el desarrollo de una API REST segura y funcional que interactúa con la API de TMDb. Es esencial seguir estas directrices para asegurar una implementación exitosa y un uso seguro de la API.



## 📋 Assignment Details

**Work Type:** ASSIGNMENT  
**State:** PUBLISHED  
**Assignment Mode:** ALL_STUDENTS

---

*Assignment ID: 697765811470*
