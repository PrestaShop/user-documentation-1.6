# Instalación de PrestaShop en su ordenador

Es posible que desee instalar PrestaShop en su equipo local, ya sea con el fin de probarlo antes de invertir dinero en un servidor y en un nombre de dominio, o para personalizar su tienda localmente antes de subir sus modificaciones a otra instalación de PrestaShop que ya tenga instalada y funcionando en su alojamiento web.

La instalación de cualquier aplicación web a nivel local requiere primeramente de la instalación del entorno adecuado, esto es: el servidor web Apache, el intérprete del lenguaje PHP, el servidor de base de datos MySQL, e idealmente la herramienta phpMyAdmin. Este conjunto de herramientas es conocido con el acrónimo de   AMP: Apache+MySQL+PHP. Éste existe para muchos sistemas operativos, lo que proporciona la adición de otra letra al acrónimo: WAMP (Windows+Apache+MySQL+PHP), MAMP (Mac OS X+...) y LAMP (Linux+...).

## Elegir un paquete AMP <a href="#instalaciondeprestashopensuordenador-elegirunpaqueteamp" id="instalaciondeprestashopensuordenador-elegirunpaqueteamp"></a>

Tendría que sumergirse en un trabajo que requiere de formación bastante técnica para poder instalar todas las herramientas comentadas en la sección anterior; afortunadamente existen muchos paquetes pre-construidos que puede instalar fácilmente y que le proporcionan todo lo que necesita. Éstos no le impedirán tener que ahondar en la técnica, pero le serán de gran ayuda. Dado que todos los elementos empaquetados son de código abierto, estos instaladores son en la mayoría de ocasiones gratuitos. He aquí una selección de instaladores AMP gratuitos:

* EasyPHP: [http://www.easyphp.org/](http://www.easyphp.org/) (Windows)
* MAMP: [http://www.mamp.info/](http://www.mamp.info/) (Mac OS X)
* WampServer: [http://www.wampserver.com/es/](http://www.wampserver.com/es/) (Windows)
* XAMPP: [https://www.apachefriends.org/es/index.html](https://www.apachefriends.org/es/index.html) (Windows, Mac OS X, Linux, Solaris)

¡EasyPHP tiene un paquete especial todo en uno, que incluye una instalación lista para usar de PrestaShop 1.6! Es la forma más fácil de descubrir la nueva versión de PrestaShop, y para los desarrollos de temas y módulos por parte de los desarrolladores.

Descárguelo desde el siguiente enlace: [http://www.easyphp.org/prestashop.php](http://www.easyphp.org/prestashop.php)

Seleccione el paquete AMP con el que se sienta más cómodo, e inicie su ejecución.

Comprobación de que todo está funcionando perfectamente\
 <a href="#instalaciondeprestashopensuordenador-comprobaciondequetodoestafuncionandoperfectamente" id="instalaciondeprestashopensuordenador-comprobaciondequetodoestafuncionandoperfectamente"></a>
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Antes de continuar con este tutorial de instalación de  PrestaShop, asegúrese de que todos los componentes de su paquete AMP se encuentra trabajando de forma correcta:

*   **El servidor web debe estar en funcionamiento** . Usted debería ser capaz de acceder a éste a través de su navegador, escribiendo "127.0.0.1" en la barra de direcciones.

    [`http://127.0.0.1`](http://127.0.0.1) es el "localhost", que corresponde a "su ordenador": se trata de una dirección de bucle invertido que dirige el navegador a su servidor web local.\
    En realidad, [`http://127.0.0.1`](http://127.0.0.1) y [`http://localhost`](http://localhost) son la misma cosa: puede utilizar uno u otro indistintamente, ambos le dirigen a usted a la carpeta raíz de su servidor web local..

    Algunos servidores web podrían no ser capaces de inicializarse porque su puerto de conexión (normalmente, el puerto 80) están siendo  utilizados por otra aplicación.

    Esto sucede a menudo cuando se utiliza Skype. Para corregir este problema de que su servidor web local no pueda inicializarse, diríjase a la configuración avanzada de Skype (Herramientas > Opciones > Avanzadas > Conexiones) y desmarque la opción "Utilizar puertos 80 y 443 como alternativos". Reinicie Skype, e inicie de nuevo su servidor web local.
* **El servidor de la base de datos debe estar en funcionamiento**. MySQL es en donde todos los datos de PrestaShop se almacenan. El paquete AMP debería proporcionarle un indicador claro si MySQL está funcionando o no.
* **La herramienta phpMyAdmin debe ser accesible**. Se trata de la aplicación web que le ayuda a manejar los datos almacenados en MySQL. Su ubicación depende del paquere que elija: ésta puede ser encontrada en [`http://127.0.0.1/phpmyadmin`](http://127.0.0.1/phpmyadmin) (XAMPP, WampServer, MAMP), [`http://127.0.0.1/mysql`](http://127.0.0.1/mysql) (EasyPHP), o incluso en otra ubicación. Consulte la documentación del paquete – éste incluso podría proveerle de un botón phpMyAdmin que abriría la URL correcta en su navegador.

## Encontrar la carpeta raíz del servidor web local <a href="#instalaciondeprestashopensuordenador-encontrarlacarpetaraizdelservidorweblocal" id="instalaciondeprestashopensuordenador-encontrarlacarpetaraizdelservidorweblocal"></a>

Una vez que haya comprobado que el paquete está instalado correctamente y que todos sus servicios están en ejecución, necesitará encontrar la carpeta raíz de su servidor web local.

Esa es la carpeta local donde colocará los archivos de su aplicación, y puede ser comparada a la carpeta raíz de su servidor en línea, a excepción de que su contenido es accesible a través de la siguiente dirección [`http://127.0.0.1`](http://127.0.0.1).

&#x20;La ubicación real de esta carpeta en el equipo depende en gran medida del paquete AMP que utilice, y frecuentemente puede ser personalizada:

* EasyPHP: `C:\easyphp\www`
* MAMP: `/Applications/MAMP/htdocs/`
* WampServer: `C:\wamp\www`
* XAMPP: `C:\xampp\htdocs` o `/Applications/xampp/htdocs`

## Encontrar la información de usuario de MySQL <a href="#instalaciondeprestashopensuordenador-encontrarlainformaciondeusuariodemysql" id="instalaciondeprestashopensuordenador-encontrarlainformaciondeusuariodemysql"></a>

Por último, es necesario conocer el nombre de usuario y la contraseña root para MySQL, con el fin de instalar PrestaShop.

**La mayoría de los paquetes usan el nombre de usuario "root" con una contraseña vacía**, incluyendo EasyPHP, MAMP, WampServer y XAMPP.

Lea la documentación de su paquete.

## Nota final antes del tutorial de instalación <a href="#instalaciondeprestashopensuordenador-notafinalantesdeltutorialdeinstalacion" id="instalaciondeprestashopensuordenador-notafinalantesdeltutorialdeinstalacion"></a>

Una vez configurado correctamente, puede seguir en el resto de esta guía de introducción y comenzar la instalación de PrestaShop.

Al instalar PrestaShop a nivel local, tenga en cuenta que:

* Los archivos no deben ser cargados/subidos  a través de un cliente FTP (como Filezilla) a un servidor web: simplemente muévalos a la carpeta local correcta, como se indicó anteriormente.
* Usted no tiene que crear un nombre de dominio local: PrestaShop está disponible a través de la dirección bucle de retorno que se ha indicado anteriormente, la cual puede ser  [`http://localhost`](http://localhost) o [`http://127.0.0.1`](http://127.0.0.1) . Sí PrestaShop se encuentra disponible en esta dirección añada el nombre de su carpeta, por ejemplo, [`http://localhost/prestashop`](http://localhost/prestashop) o [`http://127.0.0.1/prestashop`](http://127.0.0.1/prestashop) si PrestaShop se encuentra en la subcarpeta `/prestashop/` de la carpeta raíz local. Al acceder a esta dirección, por primera vez, debería ser redirigido automáticamente al instalador de PrestaShop, ya sea en [`http://localhost/prestashop/install`](http://localhost/prestashop/install) o en [`http://127.0.0.1/prestashop/install`](http://127.0.0.1/prestashop/install).\


¿Ha leído todo? Ahora siga la guía clásica de instalación, comenzando directamente en la sección "Creación de una base de datos para su tienda": [Instalación de PrestaShop](instalacion-de-prestashop.md).
