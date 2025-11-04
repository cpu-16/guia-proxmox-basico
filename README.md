# Guía básica de virtualización con Proxmox VE

1. Acceso a la interfaz web de Proxmox

Para administrar Proxmox se utiliza una interfaz web, es decir, se entra desde el navegador (Chrome, Edge, Firefox, etc.).

1.1. IP y puerto de acceso

El administrador del laboratorio te proporcionará:

La IP privada del servidor Proxmox (por ejemplo: 172.25.205.161).

El puerto de administración de Proxmox (por defecto: 8006).

El acceso por Tailscale, para que puedas llegar a esa IP aunque Proxmox esté en otra red.

Una vez conectado a Tailscale en tu PC, abre tu navegador e introduce la dirección en la barra:

https://IP_DEL_PROXMOX:8006


Ejemplo real:

https://172.25.205.161:8006


Es normal que el navegador muestre un aviso de “No seguro” o “Certificado no válido”, porque Proxmox usa un certificado propio (self-signed). En este laboratorio lo aceptamos para poder continuar.

1.2. Pantalla de inicio de sesión

Al cargar la página verás la ventana “Proxmox VE Login” (como en la captura):

User name (Nombre de usuario): normalmente root u otro usuario que te haya creado el administrador.

Password (Contraseña): la que se te haya asignado.

Realm (Dominio de autenticación):

Lo habitual en un entorno pequeño es dejar: Linux PAM standard authentication.

En entornos más avanzados podrían existir otros “realms” (por ejemplo, un directorio LDAP o Active Directory), pero en este manual usaremos siempre el realm por defecto.

Language (Idioma): puedes elegir Español si está disponible o dejar English - English.

Opcionalmente puedes marcar “Save User name” para que el navegador recuerde el usuario.

Por último, pulsa el botón “Login” para entrar al panel de administración de Proxmox.
