# Actualizar y desinstalar Prestashop

**Tabla de contenidos**

* [Actualizar PrestaShop](actualizar-y-desinstalar-prestashop.md#ActualizarydesinstalarPrestashop-ActualizarPrestaShop)
* [Desinstalar PrestaShop](actualizar-y-desinstalar-prestashop.md#ActualizarydesinstalarPrestashop-DesinstalarPrestaShop)

## Actualizar PrestaShop <a href="#actualizarydesinstalarprestashop-actualizarprestashop" id="actualizarydesinstalarprestashop-actualizarprestashop"></a>

Nosotros hemos realizado una guía dedicada para este proceso: [Updating PrestaShop](http://doc.prestashop.com/display/PS15/Updating+PrestaShop).

## Desinstalar PrestaShop <a href="#actualizarydesinstalarprestashop-desinstalarprestashop" id="actualizarydesinstalarprestashop-desinstalarprestashop"></a>

PrestaShop es muy fácil de desinstalar:

1. Elimine todos los archivos y carpetas de PrestaShop de su servidor web, utilizando su cliente FTP.
2. Elimine todas las tablas `ps_` de la base de datos de PrestaShop, utilizando phpMyAdmin.

Usted perderá toda la información registrada en su tienda: clientes, pedidos, facturas, productos, etc.\
&#x20;Esta acción no se puede deshacer, a menos que tenga una copia de seguridad de todos sus datos.
