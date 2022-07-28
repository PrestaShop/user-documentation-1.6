# Informaciones diversas

**Tabla de contenidos**\
****

/\*\<!\[CDATA\[\*/\
div.rbtoc1597066504955 {padding: 0px;}\
div.rbtoc1597066504955 ul {list-style: disc;margin-left: 0px;}\
div.rbtoc1597066504955 li {margin-left: 0px;padding-left: 0px;}\
\
/\*]]>\*/

* [Informaciones diversas](informaciones-diversas.md#Informacionesdiversas-Informacionesdiversas)
  * [¡Mantenga una versión de prueba a mano!](informaciones-diversas.md#Informacionesdiversas-¡Mantengaunaversióndepruebaamano!)
  * [Comprobación de la librería GD](informaciones-diversas.md#Informacionesdiversas-ComprobacióndelalibreríaGD)
  * [Activar PHP5](informaciones-diversas.md#Informacionesdiversas-ActivarPHP5)
    * [1&1](informaciones-diversas.md#Informacionesdiversas-1&1)
    * [Free.fr](informaciones-diversas.md#Informacionesdiversas-Free.fr)
    * [OVH](informaciones-diversas.md#Informacionesdiversas-OVH)
    * [GoDaddy](informaciones-diversas.md#Informacionesdiversas-GoDaddy)
    * [Lunarpages alojamiento compartido](informaciones-diversas.md#Informacionesdiversas-Lunarpagesalojamientocompartido)

## Informaciones diversas <a href="#informacionesdiversas-informacionesdiversas" id="informacionesdiversas-informacionesdiversas"></a>

### ¡Mantenga una versión de prueba a mano! <a href="#informacionesdiversas-mantengaunaversiondepruebaamano" id="informacionesdiversas-mantengaunaversiondepruebaamano"></a>

Después de instalar y configurar su tienda de la manera en que mejor se adapte a sus necesidades, le recomendamos **encarecidamente** que instale una versión de prueba en su ordenador o en otro lugar de su servidor de alojamiento, antes de abrir oficialmente su tienda al público, utilizando [WAMP](http://en.wikipedia.org/wiki/Comparison\_of\_WAMPs) para Windows, [MAMP](http://en.wikipedia.org/wiki/MAMP) para Mac, [LAMP](http://en.wikipedia.org/wiki/LAMP\_\(software\_bundle) para Linux, o [XAMPP](http://www.apachefriends.org/en/xampp.html) para cualquiera de esas plataformas.

Esta segunda instancia le será de utilidad como un entorno de pre-producción en la que poder llevar a cabo todas las futuras modificaciones que vaya a realizar en su tienda, sin afectar a la versión que se encuentra en línea. De esta manera, si se produce un error en este entorno de prueba, su tienda real no se vería afectada.

Tras haber confirmado que su versión de prueba funciona como debería, copiar la versión de prueba sobre la versión online. Es mejor hacer este proceso en horas no pico, y estableciendo su tienda en Modo de Mantenimiento temporalmente desde el back-office de Prestashop.

### Comprobación de la librería GD <a href="#informacionesdiversas-comprobaciondelalibreriagd" id="informacionesdiversas-comprobaciondelalibreriagd"></a>

La [librería GD](http://www.boutell.com/gd/) permite a PrestaShop editar las imágenes que suba, incluyendo el cambio de tamaño de éstas.

En una instalación por defecto de PHP, la librería GD debería estar activa, pero si encuentra que este no es el caso para su instalación, las instrucciones para Windows son las siguientes:

1. En el directorio raíz de la carpeta de PHP, abra el archivo `php.ini`.
2. Descomente la línea `extension=php_gd2.dll` (situada en la parte media del archivo, entre una larga lista de extensiones) borrando el carácter ";" en el inicio de la línea.\
   Reinicie los servicios de PHP.

Si no tiene acceso al archivo `php.ini` (que es lo que ocurre generalmente al tener contratado un  alojamiento compartido), póngase en contacto con su proveedor de alojamiento.&#x20;

### Activar PHP5 <a href="#informacionesdiversas-activarphp5" id="informacionesdiversas-activarphp5"></a>

A menudo, los servidores dedicados o compartidos tienen tanto PHP 4 como PHP 5 disponibles, pero sólo PHP4 se activa de forma predeterminada.

Para instalar PrestaShop, PHP 5 debe ser activado. Si intenta ejecutar PrestaShop utilizando PHP 4, recibirá numerosos errores, incluyendo este mensaje:&#x20;

```
Parse error: parse error, unexpected T_STATIC, expecting T_OLD_FUNCTION or T_FUNCTION or T_VAR or '}' in [php file] on line X.
```

Por favor, no dude en publicar en PrestaShop's [Forge](http://forge.prestashop.com/), un informe concerniente al aviso de error que recibe al ejecutar PrestaShop en su servicio de hosting. Los iremos añadiendo a esta guía en cuanto los recibamos.

&#x20;A continuación se presenta un listado de procedimientos que tendrá que realizar, en algunos proveedores de hosting...&#x20;

#### 1&1 <a href="#informacionesdiversas-1-and-1" id="informacionesdiversas-1-and-1"></a>

Añada esta línea a su archivo `.htaccess`:

```
AddType x-mapp-php5 .php
```

Para la reescritura de URL, añada las siguientes líneas:

```
Options +FollowSymLinks
RewriteEngine On
```

#### [Free.fr](http://free.fr) <a href="#informacionesdiversas-free.fr" id="informacionesdiversas-free.fr"></a>

Añada esta línea a su archivo `.htaccess`:

```
php 1
```

#### OVH <a href="#informacionesdiversas-ovh" id="informacionesdiversas-ovh"></a>

Añada esta línea a su archivo `.htaccess`:

```
SetEnv PHP_VER 5
```

Para desactivar registros globales:

```
SetEnv REGISTER_GLOBALS 0
```

#### GoDaddy <a href="#informacionesdiversas-godaddy" id="informacionesdiversas-godaddy"></a>

Para conocer su versión de PHP:

1. Inicie sesión.
2. En la sección Productos, haga clic en Web Hosting.
3. Junto a la cuenta de alojamiento que desea utilizar, haga clic en Iniciar.

En la sección Servidor, puede ver la versión de PHP.

Para cambiar su versión de PHP:

1. En el menú Contenido, seleccione Lenguajes de programación.
2. Seleccione la versión de PHP que desee utilizar y, a continuación, haga clic en Continuar.
3. Haga clic en Actualizar.

Los cambios pueden tardar hasta 24 horas en completarse.

#### Lunarpages alojamiento compartido <a href="#informacionesdiversas-lunarpagesalojamientocompartido" id="informacionesdiversas-lunarpagesalojamientocompartido"></a>

1. Acceda al cPanel. Éste debería estar ubicado en [http://www.(su\_dominio).(com/net/org/etc)/cpanel](http://www.\(su\_dominio\).\(com/net/org/etc\)/cpanel)
2. Introduzca el nombre de usuario y contraseña de su cuenta en el cuadro que aparece.
3. Aparecerá una nueva página. Diríjase a la última fila de iconos en la página y haga clic en el icono titulado "Enable/Disable PHP 5 (Activar / Desactivar PHP 5)"
4. Aparecerá una nueva página. Haga clic en "Add PHP 5 To Your Account! (Añadir PHP 5 a su cuenta!)".

Su petición de cambio será presentada. Por favor sea paciente, este cambio puede tomar hasta 24 horas para que sea procesado por el servidor de hosting.
