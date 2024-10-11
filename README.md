# Tarea-1.1---Acceso-a-APIs

Reporte sobre el Acceso a APIs utilizando POST con XAMPP, Postman y osTicket
Introducción
Este reporte detalla el proceso de acceso a APIs utilizando el método POST, centrándose en la configuración de un entorno de desarrollo local con XAMPP, la utilización de Postman como herramienta para realizar solicitudes y la integración con osTicket, un sistema de gestión de tickets.

Herramientas Utilizadas
XAMPP: Un paquete de software que incluye Apache, MySQL, PHP y Perl, que permite configurar un servidor local para desarrollar aplicaciones web.
Postman: Una herramienta de colaboración para API que permite a los desarrolladores realizar pruebas y documentar sus APIs de manera eficiente.
osTicket: Un sistema de soporte técnico de código abierto que permite gestionar solicitudes y tickets de usuarios.
Configuración del Entorno
Instalación de XAMPP:

Descargar e instalar XAMPP desde la página oficial.
Iniciar los módulos de Apache y MySQL desde el panel de control de XAMPP.
Instalación de osTicket:

Descargar osTicket y colocar los archivos en la carpeta htdocs de XAMPP.
Configurar la base de datos en MySQL y seguir las instrucciones de instalación de osTicket para conectar la aplicación a la base de datos.
Realización de Solicitudes POST con Postman
Configuración de Postman:

Abrir Postman y crear una nueva colección para organizar las solicitudes.
Definir el endpoint de la API de osTicket (por ejemplo, http://localhost/osTicket/api/tickets).
Ejemplo de Solicitud POST:

Seleccionar el método POST.
Configurar la URL del endpoint correspondiente.
En la pestaña "Body", elegir el formato JSON y proporcionar la estructura necesaria, por ejemplo:
json

{
    "name": "John Doe",
    "email": "john.doe@example.com",
    "subject": "Issue with ticket system",
    "message": "I am unable to access my account."
}
Autenticación:

Si la API de osTicket requiere autenticación, agregar los encabezados necesarios en la sección de "Headers" (por ejemplo, Authorization: Bearer {token}).
Enviar la Solicitud:

Hacer clic en "Send" para enviar la solicitud POST y revisar la respuesta en la parte inferior de Postman.
Manejo de Respuestas
Analizar la respuesta JSON devuelta por osTicket. Debe incluir un código de estado HTTP (200, 201, etc.) y, en caso de éxito, detalles sobre el ticket creado.
Implementar manejo de errores en caso de recibir un código de error (por ejemplo, 400 o 500).
Conclusiones
El uso del método POST en combinación con XAMPP, Postman y osTicket permite a los desarrolladores interactuar eficazmente con el sistema de gestión de tickets. La configuración del entorno local y la utilización de herramientas adecuadas facilita el proceso de prueba y desarrollo, asegurando que las integraciones sean efectivas y sin problemas.
