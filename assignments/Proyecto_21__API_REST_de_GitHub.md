# Proyecto 21 | API REST de GitHub

**📅 Created:** July 03, 2024 at 11:03 PM  
**📅 Updated:** July 05, 2024 at 04:44 AM  
**🔗 Original Link:** [View in Classroom](https://classroom.google.com/c/Njk1MDgxNzAyMTIx/a/Njk3NzM2MjU0NDUx/details)  
**👤 Created by:** Adrián Fernando Gaitán Londoño
**🆔 Creator ID:** 100957882007157850038
**📊 Max Points:** N/A  

**📅 Due Date:** {'year': 2024, 'month': 7, 'day': 5}

---

## 📝 Description

Este documento describe el contrato para el desarrollo de una API REST que interactúa con la API de GitHub para obtener información pública del perfil de un usuario, incluidos sus repositorios. La API debe implementarse de manera segura, sin exponer las claves de acceso (API keys) utilizadas para interactuar con GitHub.

1. Endpoints y Parámetros

1.1. Obtener Información del Perfil del Usuario
Método HTTP: GET
Ruta del Endpoint: `/api/github/user/:username`
Descripción: Recupera información pública del perfil de un usuario de GitHub.
Parámetros:
Path Parameter:
`:username` (string) - El nombre de usuario de GitHub del que se desea obtener información.
Query Parameters (Opcionales):
`include_repos` (boolean) - Si se incluye, determina si se deben obtener detalles sobre los repositorios públicos del usuario. Por defecto, `false`.

Ejemplo de respuesta exitosa (200 OK):
```json
{
"username": "octocat",
"id": 583231,
"avatar_url": "[https://avatars.githubusercontent.com/u/583231?v=4",](https://avatars.githubusercontent.com/u/583231?v=4",)
"html_url": "[https://github.com/octocat",](https://github.com/octocat",)
"name": "The Octocat",
"company": "GitHub",
"location": "San Francisco",
"bio": "A mysterious character.",
"public_repos": 8,
"followers": 3934,
"following": 9,
"repos": [
{
"name": "Hello-World",
"html_url": "[https://github.com/octocat/Hello-World",](https://github.com/octocat/Hello-World",)
"description": "This your first repo!",
"updated_at": "2023-06-01T12:34:56Z"
},
...
]
}
```
Si `include_repos` es `true`, se incluirá un array con la información básica de los repositorios públicos del usuario.

Posibles Errores:
404 Not Found: El nombre de usuario proporcionado no existe.
400 Bad Request: El parámetro `username` no es válido.
500 Internal Server Error: Error del servidor al procesar la solicitud.

1.2. Listar Repositorios Públicos del Usuario

Método HTTP: GET
Ruta del Endpoint: `/api/github/user/:username/repos`
Descripción: Lista todos los repositorios públicos del usuario de GitHub especificado.
Parámetros:
Path Parameter:
`:username` (string) - El nombre de usuario de GitHub del que se desea obtener los repositorios públicos.
Query Parameters (Opcionales):
`sort` (string) - Criterio para ordenar los repositorios. Valores posibles: `created`, `updated`, `pushed`, `full_name`. Por defecto, `full_name`.
`direction` (string) - Dirección de la ordenación. Valores posibles: `asc`, `desc`. Por defecto, `asc`.

Ejemplo de respuesta Exitosa (200 OK):
```json
{
"repos": [
{
"name": "Hello-World",
"html_url": "[https://github.com/octocat/Hello-World",](https://github.com/octocat/Hello-World",)
"description": "This your first repo!",
"language": "JavaScript",
"created_at": "2020-01-01T12:34:56Z",
"updated_at": "2023-06-01T12:34:56Z",
"pushed_at": "2023-06-01T12:34:56Z"
},
...
]
}
```

Posibles Errores:
404 Not Found: El nombre de usuario proporcionado no existe.
400 Bad Request: El parámetro `username` no es válido.
500 Internal Server Error: Error del servidor al procesar la solicitud.

---

1.3. Obtener Información Detallada de un Repositorio
Método HTTP: GET
Ruta del Endpoint: `/api/github/user/:username/repos/:repo`
Descripción: Recupera información detallada sobre un repositorio público específico de un usuario de GitHub.
Parámetros:
Path Parameters:
`:username` (string) - El nombre de usuario de GitHub.
`:repo` (string) - El nombre del repositorio del que se desea obtener información.

Respuesta Exitosa (200 OK):
```json
{
"name": "Hello-World",
"full_name": "octocat/Hello-World",
"owner": {
"login": "octocat",
"id": 583231,
"avatar_url": "[https://avatars.githubusercontent.com/u/583231?v=4"](https://avatars.githubusercontent.com/u/583231?v=4")
},
"html_url": "[https://github.com/octocat/Hello-World",](https://github.com/octocat/Hello-World",)
"description": "This your first repo!",
"language": "JavaScript",
"created_at": "2020-01-01T12:34:56Z",
"updated_at": "2023-06-01T12:34:56Z",
"pushed_at": "2023-06-01T12:34:56Z",
"stargazers_count": 150,
"watchers_count": 150,
"forks_count": 30,
"open_issues_count": 5,
"license": {
"key": "mit",
"name": "MIT License"
}
}
```

Posibles Errores:
404 Not Found: El nombre de usuario o repositorio proporcionado no existe.
400 Bad Request: Los parámetros `username` o `repo` no son válidos.
500 Internal Server Error: Error del servidor al procesar la solicitud.

2. Especificaciones de Seguridad

2.1. Manejo de Claves de API

No Exponer Claves de API:
Las claves API para acceder a la API de GitHub deben almacenarse de forma segura en el servidor y nunca deben exponerse al cliente.
Utilizar variables de entorno (environment variables) para manejar las claves de API y cargarlas mediante configuraciones seguras en el servidor.

2.2. Validación de Solicitudes

Validación de Parámetros:
Validar todos los parámetros de entrada (tanto path parameters como query parameters).

2.3. Manejo de Errores

Respuestas de Error:
Proporcionar respuestas claras y detalladas para los errores, incluyendo códigos de estado HTTP y mensajes descriptivos.
No incluir información sensible en las respuestas de error.

1. Consideraciones Adicionales

3.1. Documentación

En la ruta principal de la API, `/api/`, proporcionar una documentación clara y detallada de los endpoints disponibles, los parámetros aceptados y las respuestas esperadas.

3.2. Testing

Crear una collection de Postman con las solicitudes de prueba para cada endpoint de la API y compartirlo.



## 📋 Assignment Details

**Work Type:** ASSIGNMENT  
**State:** PUBLISHED  
**Assignment Mode:** ALL_STUDENTS

---

*Assignment ID: 697736254451*
