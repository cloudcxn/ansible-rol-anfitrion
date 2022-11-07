Rol de Ansible: Anfiftrión
==========================

Rol de Ansible para configurar el nombre del anfitrión a partir del serial
de la Raspberry Pi.

Ej: `raspberry-pi-a123`

Requerimientos
--------------

* Raspberry Pi con Raspbian basada en Debian Bullseye.
* Usuario al formatear la tarjeta SD de arranque: administrador
* SSH habilitado en la Raspberry Pi.

Variables del Rol
-----------------

| Variable | Descripción |
| -------- | ----------- |
| anfitrion_modelo | Modelo de la Raspberry Pi que servirá como el prefijo para el nombre del anfitrión. |

Ver los [valores por defecto](defaults/main.yml).

Dependencias
------------

Ninguna

Libro de Ejemplo
----------------

    - hosts: servidores
      roles:
         - { role: cloudcxn.anfitrion, anfitrion_modelo: "raspberry-pi-4" }

Licencia
--------

MIT.

Información del Autor
---------------------

El rol fue creado en noviembre del 2022 por Byron Quezada para
[Cloud CxN](https://www.cloudcxn.com).
