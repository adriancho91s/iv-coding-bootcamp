# Proyecto Final: Red Social

**📅 Posted:** July 14, 2024 at 02:51 PM  
**🔗 Original Link:** [View in Classroom](https://classroom.google.com/c/Njk1MDgxNzAyMTIx/p/NzAwODAwNDQyMjA0)  
**👤 Posted by:** Adrián Fernando Gaitán Londoño
**🆔 Creator ID:** 100957882007157850038

---

## 📝 Content

Proyecto Final: Red Social
El objetivo de este proyecto es reunir todo lo aprendido en el curso de programación Full Stack y aplicar todas las tecnologías vistas a lo largo del bootcamp para construir una red social.

Los participantes deben trabajar en equipo para diseñar y desarrollar una red social básica que cumpla con los siguientes requisitos funcionales y de diseño.

Funcionalidades Requeridas:

1. Registro y Autenticación de Usuarios:
Los usuarios deben poder crear una cuenta con una suscripción a la aplicación.
Verificar la disponibilidad del nombre de usuario (username) ya que debe ser único.
Permitir a los usuarios registrar datos personales como nombre, edad y género.
Opcional: permitir que los usuarios añadan una foto de perfil y de portada, descripción personal, lugar de estudios, lugar de trabajo, ubicación, y un enlace a su sitio personal.
2. Configuración de la Cuenta:
Permitir a los usuarios configurar el tema (aspecto visual) de la aplicación y garantizar que esta configuración persista en cualquier dispositivo.
3. Personalización del Perfil:
Los usuarios deben poder personalizar su perfil añadiendo una foto de perfil, una imagen de portada, una descripción, lugar de estudios, ubicación, un enlace personal, y lugar de trabajo.
4. Creación de Posts:
Permitir a los usuarios crear posts que incluyan texto, vídeo o imagen.
Los posts pueden ser públicos o visibles solo para seguidores.
Cada post debe permitir recibir reacciones y ser añadido a los favoritos por otros usuarios.
Mostrar la fecha de creación de cada post de manera agradable (usando una librería recomendada como [https://date-fns.org).](https://date-fns.org).)
5. Seguimiento de Usuarios:
Permitir a los usuarios encontrar y seguir a otros usuarios registrados en la aplicación.
Manejar solicitudes de seguimiento y notificaciones de estas solicitudes (en tiempo real).
6. Feed de Noticias:
Listar los posts de las cuentas seguidas en el feed principal (homepage).
Permitir acceso a los últimos posts del perfil de los usuarios seguidos.
7. Sistema de Chat:
Permitir la comunicación en tiempo real entre usuarios que se sigan mutuamente.
Mostrar dinámicamente notificaciones de mensajes recibidos.
8. Favoritos y Likes:
Permitir a los usuarios ver los posts que han guardado y los posts a los que les han dado like.
9. Perfil del Usuario:
Generar un perfil para cada usuario accesible mediante su @ en la URL.
Mostrar los posts publicados, los seguidores y las personas seguidas en el perfil del usuario.
10. Navbar:
Acceso rápido a notificaciones, mensajes, búsqueda de posts o amigos.
Permitir a cualquier usuario acceder a su configuración de perfil, ir a su perfil directamente o cerrar sesión (logout).
Vistas Requeridas:

1. Página de Registro y Login:
Formulario de registro con verificación de disponibilidad de username.
Formulario de login para acceder a la cuenta.
2. Página Principal (Feed):
Visualización de los posts de los usuarios seguidos.
Acceso rápido a la creación de nuevos posts (texto, imagen, vídeo).
3. Página de Perfil:
Visualización del perfil del usuario con su información personal y posts.
Opciones para editar el perfil.
4. Página de Configuración:
Configuración de la cuenta, tema de la aplicación y preferencias.
5. Sistema de Chat:
Interfaz para la comunicación en tiempo real entre usuarios que se siguen mutuamente.
6. Notificaciones:
Sistema de notificaciones para solicitudes de seguimiento, mensajes y reacciones a posts.
Tecnologías Requeridas:
Frontend: React.js, con Next.js, RTK (para el manejo de fetch).
Estilos: Tailwind CSS (opcional usar librerías de componentes UI como Shadcn UI y Radix).
Backend: NestJS, TypeOrm, Class Validators, Swagger.
Cloud: AWS.
Base de Datos: PostgreSQL.
Autenticación: JWT (JSON Web Tokens) o Cookie Based Authentication.
Real-time: Socket.io (para el chat y notificaciones en tiempo real).
Otros: Librerías recomendadas como date-fns para el manejo de fechas.
Planificación y Entregables:

1. Fase de Diseño:
Bocetos de las interfaces y flujo de usuario.
Definición de la arquitectura del sistema.
2. Fase de Desarrollo:
Implementación de funcionalidades básicas de registro y autenticación.
Desarrollo del feed principal y creación de posts.
Implementación del sistema de seguimiento y perfil de usuario.
Desarrollo del sistema de chat en tiempo real.
Integración de notificaciones y favoritos.
3. Entrega Final:
Presentación del proyecto final con demostración de todas las funcionalidades implementadas.
Ruta para el deployment:
[https://adriancho91.notion.site/AWS-Deployment-IV-Coding-Bootcamp-a5264f71cefe44878943076ed14e6c16](https://adriancho91.notion.site/AWS-Deployment-IV-Coding-Bootcamp-a5264f71cefe44878943076ed14e6c16)



---

*Announcement ID: 700800442204*
