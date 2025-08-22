# Trabajo desde Casa

**📅 Posted:** July 14, 2024 at 02:32 PM  
**🔗 Original Link:** [View in Classroom](https://classroom.google.com/c/Njk1MDgxNzAyMTIx/p/NzAwNzk5MzIzNzQx)  
**👤 Posted by:** Adrián Fernando Gaitán Londoño
**🆔 Creator ID:** 100957882007157850038

---

## 📝 Content

Trabajo desde Casa

DTOs, Patrón Repositorio y Servicios | Clase 4 | NestJS de 0 a 100
- Duración: 18 min
- Publicación: Jan 4, 2023
- [Ver video]([https://www.youtube.com/watch?v=_sVnRC3mIko&list=PLergODdA95kfcSoXqZZ-IDImO6YaQLYlG&index=6)](https://www.youtube.com/watch?v=_sVnRC3mIko&list=PLergODdA95kfcSoXqZZ-IDImO6YaQLYlG&index=6))

Error Handlers y Controladores | Clase 5 | NestJS de 0 a 100
- Duración: 24 min
- Publicación: Jan 10, 2023
- [Ver video]([https://www.youtube.com/watch?v=7uX7c-9iObM&list=PLergODdA95kfcSoXqZZ-IDImO6YaQLYlG&index=7)](https://www.youtube.com/watch?v=7uX7c-9iObM&list=PLergODdA95kfcSoXqZZ-IDImO6YaQLYlG&index=7))

Relaciones con Query Builder | Clase 6 | NestJS de 0 a 100
- Duración: 21 min
- Publicación: Feb 10, 2023
- [Ver video]([https://www.youtube.com/watch?v=pXYAwYq9gfw&list=PLergODdA95kfcSoXqZZ-IDImO6YaQLYlG&index=8)](https://www.youtube.com/watch?v=pXYAwYq9gfw&list=PLergODdA95kfcSoXqZZ-IDImO6YaQLYlG&index=8))

Autenticación de Usuarios + Tip de TypeScript | Clase 7 | NestJS de 0 a 100
- Duración: 49 min
- Publicación: Feb 15, 2023
- [Ver video]([https://www.youtube.com/watch?v=NBR2AoHfKSo&list=PLergODdA95kfcSoXqZZ-IDImO6YaQLYlG&index=9)](https://www.youtube.com/watch?v=NBR2AoHfKSo&list=PLergODdA95kfcSoXqZZ-IDImO6YaQLYlG&index=9))

Autorización con Guards y Decoradores | Clase 8 | NestJS de 0 a 100
- Duración: 28 min
- Publicación: Feb 24, 2023
- [Ver video]([https://www.youtube.com/watch?v=-3eLNfSsLIs&list=PLergODdA95kfcSoXqZZ-IDImO6YaQLYlG&index=10)](https://www.youtube.com/watch?v=-3eLNfSsLIs&list=PLergODdA95kfcSoXqZZ-IDImO6YaQLYlG&index=10))

Manejo de Roles y Niveles de Acceso | Clase 9 | NestJS de 0 a 100
- Duración: 29 min
- Publicación: Mar 3, 2023
- [Ver video]([https://www.youtube.com/watch?v=0KQ8uSiaxhE&list=PLergODdA95kfcSoXqZZ-IDImO6YaQLYlG&index=11)](https://www.youtube.com/watch?v=0KQ8uSiaxhE&list=PLergODdA95kfcSoXqZZ-IDImO6YaQLYlG&index=11))

Terminando Módulo de Tareas | Clase 10 | NestJS de 0 a 100
- Duración: 46 min
- Publicación: Mar 10, 2023
- [Ver video]([https://www.youtube.com/watch?v=arGKgITnbZg&list=PLergODdA95kfcSoXqZZ-IDImO6YaQLYlG&index=12)](https://www.youtube.com/watch?v=arGKgITnbZg&list=PLergODdA95kfcSoXqZZ-IDImO6YaQLYlG&index=12))

Documentación con Swagger y OpenAPI | Clase 11 | NestJS de 0 a 100
- Duración: 28 min
- Publicación: Mar 14, 2023
- [Ver video]([https://www.youtube.com/watch?v=lXIk5Tq8khQ&list=PLergODdA95kfcSoXqZZ-IDImO6YaQLYlG&index=13)](https://www.youtube.com/watch?v=lXIk5Tq8khQ&list=PLergODdA95kfcSoXqZZ-IDImO6YaQLYlG&index=13))

Modulo HTTP + Axios | Clase 11 | NestJS de 0 a 100
- Duración: 13 min
- Publicacion: Mar 16, 2023
- [ver video]([https://www.youtube.com/watch?v=oCshaXZTMJw&list=PLergODdA95kfcSoXqZZ-IDImO6YaQLYlG&index=15)](https://www.youtube.com/watch?v=oCshaXZTMJw&list=PLergODdA95kfcSoXqZZ-IDImO6YaQLYlG&index=15))

Proyecto: API Rest CRUD con NestJS y Docker
Crear una API Rest CRUD que involucre usuarios y una lista de tareas. Los usuarios pueden tener muchas tareas, pero una tarea solo puede tener un usuario. La tarea debe tener campos como título, descripción, duración, y estado (`ENUM('pending', 'inProgress', 'done')`). El usuario debe tener como mínimo: username, password, y role.

Endpoints Requeridos:
1. Usuarios:
Crear usuario (solo admin, si no el usuario debe registrarse)
Editar usuario (solo a sí mismo, o con rol admin)
Eliminar usuario (solo a sí mismo, o con rol admin)
Obtener todos los usuarios (solo admin)
Login (cualquier usuario con credenciales)
Register (cualquier usuario que quiera crear una cuenta)


2. Tareas:
Crear tarea (autenticado)
Editar tarea (autenticado)
Eliminar tarea (autenticado)
Obtener todas las tareas (rol admin)


Requisitos Adicionales:
Validaciones para todos los campos.
Incorporación de documentación con Swagger.
Usar TypeOrm, Postgres.
Configuración de la aplicación con Docker para que se ejecute con `docker-compose up`.


Pasos para Dockerizar la API:
1. Preparar el ambiente: Instalar Docker y configurar para ejecutar contenedores.
2. Crear un Dockerfile (Imagen de la API).
3. Conectar API a contendor de Postgres.
4. Construir la imagen de Docker.
5. Correr el contenedor.
6. Escribir un archivo `docker-compose.yml`:
Definir el servicio de la API.
Configurar el mapeo de puertos.
Definir el volumen para montar el código de la API.
7. Verificar que la API está corriendo: Acceder a `[http://localhost:{PORT}`.PORT](http://localhost:{PORT}`.PORT) : definido por cada ingeniero.


Recurso Recomendado:
[El mejor programa para administrar base de datos SQL y NoSQL - Datagrip]([https://www.youtube.com/watch?v=Qn4o75UqeQk)](https://www.youtube.com/watch?v=Qn4o75UqeQk))



---

*Announcement ID: 700799323741*
