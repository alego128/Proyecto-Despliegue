# Proyecto de Despliegue - UD4
Autor: Alejandro
Fecha: Febrero 2026

1. Infraestructura de Servidor y Transferencia
Servidor Web: Apache integrado en XAMPP.

Versión PHP: 8.x.

Gestión de Usuarios (SFTP/FTP):

dev_senior: Permisos totales para administración del sitio.

dev_junior: Permisos restringidos a la subcarpeta /assets.

2. Configuración de Red y DNS Local
Para simular el entorno de producción, se han configurado los siguientes subdominios mediante el archivo de hosts:

frontend.test -> Apuntando a 127.0.0.1.

backend.test -> Apuntando a 127.0.0.1.

db.test -> Apuntando a 127.0.0.1.

3. Flujo de Trabajo (Control de Versiones)
El despliegue sigue un ciclo de vida basado en Git:

Desarrollo: Los cambios se realizan en ramas locales (ej. fix-styles).

Merge: Una vez verificados, se fusionan a la rama master.

Despliegue: La transferencia de los commits finales se realiza mediante FileZilla Client al servidor configurado.