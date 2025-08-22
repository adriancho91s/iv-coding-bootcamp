# Proyecto 26 | API Rest CRUD con NestJS y Docker

**📅 Created:** July 15, 2024 at 07:34 AM  
**📅 Updated:** July 15, 2024 at 07:35 AM  
**🔗 Original Link:** [View in Classroom](https://classroom.google.com/c/Njk1MDgxNzAyMTIx/a/NzAwODU1OTU0ODEx/details)  
**👤 Created by:** Adrián Fernando Gaitán Londoño
**🆔 Creator ID:** 100957882007157850038
**📊 Max Points:** N/A  

**📅 Due Date:** {'year': 2024, 'month': 7, 'day': 15}

---

## 📝 Description

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



## 📋 Assignment Details

**Work Type:** ASSIGNMENT  
**State:** PUBLISHED  
**Assignment Mode:** ALL_STUDENTS

---

*Assignment ID: 700855954811*
