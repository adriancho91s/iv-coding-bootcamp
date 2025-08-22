# Proyecto 28 | Deployment en AWS EC2 de la API del Proyecto 26

**📅 Created:** July 16, 2024 at 08:21 AM  
**📅 Updated:** July 17, 2024 at 03:31 PM  
**🔗 Original Link:** [View in Classroom](https://classroom.google.com/c/Njk1MDgxNzAyMTIx/a/NzAwOTQ1MTk1NTU1/details)  
**👤 Created by:** Adrián Fernando Gaitán Londoño
**🆔 Creator ID:** 100957882007157850038
**📊 Max Points:** N/A  

**📅 Due Date:** {'year': 2024, 'month': 7, 'day': 17}

---

## 📝 Description

1. Introducción 
Condiciones para el deployment de la API del Proyecto 26 en una instancia de AWS EC2. El objetivo es desplegar una aplicación basada en NestJS utilizando Docker y Nginx para manejar el tráfico web. Este deployment no incluirá automatizaciones.

2. Alcance del Proyecto
- Tecnologías Utilizadas:
  - Backend: NestJS
  - Containerización: Docker
  - Web Server: Nginx
  - Cloud Platform: AWS EC2
- Componentes:
  - API Restful con NestJS
  - Contenedor Docker para la API
  - Configuración de Nginx como proxy inverso

3. Requisitos del Proyecto
- Requisitos Previos:
  - Creación y configuración de una cuenta AWS.
  - Instalación de AWS CLI en la máquina local.
  - Creación de una instancia EC2 con las configuraciones necesarias (tipo de instancia, VPC, seguridad).
- Requisitos de Software:
  - Node.js y npm instalados.
  - Docker y Docker Compose instalados.
  - Configuración de seguridad (grupos de seguridad, pares de llaves, etc.)

4. Tareas del Proyecto
Configuración de la Instancia EC2
1. Lanzamiento de la Instancia:
   - Seleccionar la región y lanzar una nueva instancia EC2.
   - Configurar el tipo de instancia, almacenamiento, y redes (VPC, subred).
   - Crear o usar un par de llaves existente para SSH.

5. Configuración de Seguridad:
   - Configurar grupos de seguridad para permitir tráfico HTTP/HTTPS y SSH.

Deployment de la API con Docker
6. Preparación del Ambiente:
   - Conectar a la instancia EC2 vía SSH.
   - Instalar Docker y Docker Compose en la instancia.

7. Configuración del Proyecto:
   - Crear un Dockerfile para la aplicación NestJS.
   - Crear un archivo `docker-compose.yml` para orquestar los servicios.
   - Construir y ejecutar los contenedores Docker.

Configuración de Nginx
8. Instalación de Nginx:
   - Instalar Nginx en la instancia EC2.
   - Configurar Nginx como proxy inverso para redirigir tráfico a los contenedores Docker.

9. Configuración SSL:
   - Instalar Certbot y obtener certificados SSL.
   - Configurar Nginx para utilizar SSL.

10. Entregables
- API del Proyecto 26 desplegada y funcionando en AWS EC2.
- Documentación del proceso de instalación y configuración.
- Archivos de configuración (`Dockerfile`, `docker-compose.yml`, configuración de Nginx).Apoyarse en documentación y/o video de su preferencia en caso de tener dificultades.



## 📋 Assignment Details

**Work Type:** ASSIGNMENT  
**State:** PUBLISHED  
**Assignment Mode:** ALL_STUDENTS

---

*Assignment ID: 700945195555*
