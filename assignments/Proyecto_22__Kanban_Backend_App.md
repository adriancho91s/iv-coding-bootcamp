# Proyecto 22 | Kanban Backend App

**📅 Created:** July 08, 2024 at 03:25 AM  
**📅 Updated:** July 08, 2024 at 03:43 AM  
**🔗 Original Link:** [View in Classroom](https://classroom.google.com/c/Njk1MDgxNzAyMTIx/a/Njk4MDg4MDMzNTIy/details)  
**👤 Created by:** Adrián Fernando Gaitán Londoño
**🆔 Creator ID:** 100957882007157850038
**📊 Max Points:** N/A  

**📅 Due Date:** {'year': 2024, 'month': 7, 'day': 8}

---

## 📝 Description

Desarrollar una aplicación web tipo tablero Kanban que permita a los usuarios crear, modificar y gestionar "cards" y "columns". La aplicación debe incorporar un sistema completo de autenticación y autorización para asegurar la privacidad y la seguridad de los datos de los usuarios.

Características de la Aplicación:

1. Gestión de Cards:
   - Los usuarios pueden crear "cards" con:
     - Título
     - Descripción en formato Markdown
     - Asignación a diferentes "columns" (estados)
   - Los usuarios pueden modificar y eliminar "cards".

2. Gestión de Columns:
   - Los usuarios pueden crear, modificar y eliminar "columns" para organizar las "cards".

3. Autenticación y Autorización:
   - Implementar un sistema que asegure que solo el propietario de los recursos pueda modificarlos.
   - Implementar un sistema de registro y perfil de usuario que permita a los usuarios modificar su información personal.

4. Perfil de Usuario:
   - Los usuarios deben poder registrarse y gestionar su perfil.
   - El perfil de usuario debe incluir campos básicos de información personal y opciones de edición.

Primera Fase del Proyecto

Objetivo de la Primera Fase
Desarrollar la API REST que permita realizar todas las operaciones mencionadas en las características de la aplicación.

Requisitos de la Primera Fase:

1. Cumplimiento de los Principios REST:
   - La API debe seguir los principios REST, asegurando una estructura consistente y entendible para la manipulación de recursos.

2. Manejo de Errores:
   - La API debe manejar errores de forma efectiva, proporcionando mensajes de error claros y adecuados códigos de estado HTTP.

3. Estándares de Seguridad:
   - Implementar medidas de seguridad para proteger la API de vulnerabilidades comunes como inyección de SQL, cross-site scripting (XSS) y ataques de fuerza bruta.
   - Asegurar que las contraseñas se almacenen de forma segura utilizando técnicas de hashing.

Restricciones Técnicas:

1. Sin Uso de ORMs:
   - La API debe interactuar directamente con la base de datos PostgreSQL sin utilizar Object-Relational Mappers (ORMs).

2. Autenticación y Autorización:
   - No se permite el uso de librerías de autenticación externas.
   - La autenticación debe implementarse usando JSON Web Tokens (JWT) o técnicas de hash para asegurar las contraseñas.
   - Las contraseñas no deben almacenarse en texto plano; deben ser hashadas utilizando un método seguro de hashing.

3. Protección de Endpoints:
   - Todos los endpoints de la API deben estar protegidos para que solo los usuarios autenticados puedan acceder y manipular los recursos.

Entregable de la Primera Fase:

1. **Código Fuente:**
   - El código completo de la API REST, siguiendo las mejores prácticas de codificación y arquitectura.
   - Documentación que describa la API, incluyendo cómo interactuar con los endpoints, manejar la autenticación y los posibles errores.

2. **Base de Datos:**
   - Esquema de la base de datos PostgreSQL con la estructura necesaria para soportar la aplicación.

3. **Instrucciones de Configuración y Ejecución:**
   - Instrucciones claras para configurar y ejecutar la API en un entorno de desarrollo y producción.


1. Funcionalidad Completa:
   - La API debe cumplir con todos los requisitos funcionales especificados para la primera fase.

2. Seguridad:
   - La API debe pasar las revisiones de seguridad internas y demostrar que las contraseñas y otros datos sensibles están protegidos adecuadamente.

3. Cumplimiento de Restricciones:
   - La API debe cumplir con todas las restricciones técnicas especificadas, incluyendo el no uso de ORMs y librerías de autenticación externas.

4. Documentación Clara y Completa:
   - La documentación debe ser detallada y clara, permitiendo a cualquier desarrollador entender y utilizar la API.



## 📋 Assignment Details

**Work Type:** ASSIGNMENT  
**State:** PUBLISHED  
**Assignment Mode:** ALL_STUDENTS

---

*Assignment ID: 698088033522*
