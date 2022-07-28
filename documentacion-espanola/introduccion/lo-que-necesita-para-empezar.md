# Lo que necesita para empezar

**Tabla de contenidos**\
****

/\*\<!\[CDATA\[\*/\
div.rbtoc1597066503842 {padding: 0px;}\
div.rbtoc1597066503842 ul {list-style: disc;margin-left: 0px;}\
div.rbtoc1597066503842 li {margin-left: 0px;padding-left: 0px;}\
\
/\*]]>\*/

* [Lo que necesitará para empezar](lo-que-necesita-para-empezar.md#Loquenecesitaparaempezar-Loquenecesitaráparaempezar)
  * [Instrucciones rápidas de puesta en marcha.](lo-que-necesita-para-empezar.md#Loquenecesitaparaempezar-Instruccionesrápidasdepuestaenmarcha.)
  * [Instrucciones detalladas de puesta en marcha.](lo-que-necesita-para-empezar.md#Loquenecesitaparaempezar-Instruccionesdetalladasdepuestaenmarcha.)
    * [Registrando un nombre de dominio](lo-que-necesita-para-empezar.md#Loquenecesitaparaempezar-Registrandounnombrededominio)
    * [Encontrar un hosting (alojamiento)](lo-que-necesita-para-empezar.md#Loquenecesitaparaempezar-Encontrarunhosting\(alojamiento\))
    * [Requerimientos Técnicos](lo-que-necesita-para-empezar.md#Loquenecesitaparaempezar-RequerimientosTécnicos)
    * [Herramientas](lo-que-necesita-para-empezar.md#Loquenecesitaparaempezar-Herramientas)
    * [Estableciendo una planificación](lo-que-necesita-para-empezar.md#Loquenecesitaparaempezar-Estableciendounaplanificación)
    * [Instalando PrestaShop](lo-que-necesita-para-empezar.md#Loquenecesitaparaempezar-InstalandoPrestaShop)

## Lo que necesitará para empezar <a href="#loquenecesitaparaempezar-loquenecesitaraparaempezar" id="loquenecesitaparaempezar-loquenecesitaraparaempezar"></a>

### Instrucciones rápidas de puesta en marcha. <a href="#loquenecesitaparaempezar-instruccionesrapidasdepuestaenmarcha." id="loquenecesitaparaempezar-instruccionesrapidasdepuestaenmarcha."></a>

Aquí hay una lista reducida de lo que necesita para comenzar con la instalación de PrestaShop 1.6. No se preocupe si encuentra lagunas en algun apartado; encontrará instrucciones detalladas en las secciones que siguen a esta.

* Requerimientos del Sistema:
  * PHP 5.2 o superior.
    * Ajustes adecuados: `allow_url_fopen` establecido en ON, `register_globals` establecido en OFF, `magic_quotes_*` establecido en OFF, `safe_mode` establecido en OFF (todo ello en el archivo `php.ini`), `file_max_upload_size` establecido en "16M".
    * Extensiones PHP útiles: PDO\_MySQL, cURL, SimpleXML, mcrypt, GD, OpenSSL, DOM, SOAP (todo ello en el archivo `php.ini`).
    * Herramientas de Servidor útiles: cron/crontab, Memcached.
  * MySQL 5.0 o superior.
  * Mejor si:\

    * El hosting es Unix/Linux.
    * El servidor corre Apache Web Server 1.3 o superior o bien nginx Web Server.
      * Ajustes para el módulo Apache: `mod_rewrite` activado (enabled), `mod_security` desactivado (disabled), `mod_auth_basic` desactivado.
    * Al menos 64 Mb de RAM dedicados a PHP.
* Códigos de acceso (cuentas de acceso) a su servidor mediante protocolo FTP y a su base de datos MySQL.\

  * Estos deberían ser suministrador por el Administrador de su hosting (alojamiento para la tienda) si no está realizando una instalación local (en su propio ordenador).
* Cualquier editor de textos (N del T: un editor excelente es Notepad Plus, gratuito).
* Cualquier cliente FTP (N del T: use un programa de FTP que guarde las contraseñas encriptadas, tal como WinSCP, gratuito).
* Cualquier navegador moderno (si decide usar Internet Explorer, asegúrese de que sea la versión 8 o superior).

También necesitará saber la URL gracias a la cual su tienda (o tiendas) van a estar visibles en internet (también llamado nombre de dominio).

Compruebe la página oficial de requerimientos del sistema: [http://www.prestashop.com/en/system-requirements](http://www.prestashop.com/en/system-requirements).

Una vez su instalación esté en marcha, puede usar la Guía de Instalación: [http://doc.prestashop.com/display/PS16/Installing+PrestaShop](http://doc.prestashop.com/display/PS16/Installing+PrestaShop).

### Instrucciones detalladas de puesta en marcha. <a href="#loquenecesitaparaempezar-instruccionesdetalladasdepuestaenmarcha." id="loquenecesitaparaempezar-instruccionesdetalladasdepuestaenmarcha."></a>

PrestaShop es una aplicación web (webapp): necesita ser instalada en un Servidor Web (webserver) para funcionar correctamente, y necesita un nombre de dominio para que sus visitantes puedan acceder a su tienda.

#### Registrando un nombre de dominio <a href="#loquenecesitaparaempezar-registrandounnombrededominio" id="loquenecesitaparaempezar-registrandounnombrededominio"></a>

Antes de descargar o instalar nada, necesitará proveer de un lugar adecuado a su tienda online Prestashop. Esto se compone de dos partes: un nombre de dominio y un servidor web (un dominio y un hosting). Un dominio es el identificador online para su sitio web como por ejemplo [`example.com`](http://example.com) o bien [`myonlineshop.net`](http://myonlineshop.net). Es la fachada pública de su servidor web, y por lo tanto, de su tienda online.

Necesitará comprar un nombre de dominio (un dominio) para su tienda. Podría ser interesante comprarlo al mismo tiempo y a la misma empresa en donde estará su alojamiento (hosting): muchas empresas de alojameinto ofrecen el dominio de forma grauita con cada nueva cuenta de cliente. Podría ser gratuito durante un año, o mientras usted sea cliente de ese proveedor. Esto hace más fácil obtener el "paquete completo" (hosting+dominio) en un solo proceso.

Tenga en cuenta que podrían surgir problemas con los dominios suministrados por su proveedor de hosting: si no está satisfecho con el servicio, podría querer cambiar a uno mejor... y esto implica mover no sólo los archivos y la base de datos, sino también (normalmente) el nombre de dominio al nuevo proveedor.

Los archivos y base de datos son fáciles de trasladar pero, dependiendo del proveedor, usted podría tener problemas intentando quedarse con su nombre de dominio. A pesar de que ellos han comprado el dominio para usted cuando usted contrató el servicio completo, técnicamente el dominio les pertenece y podrían incluso prohibirle trasladarlo a otro proveedores o hacerle pagar por él. Y dado que el dominio es su marca y la forma de acceder a su tienda, usted deberá conocer y cumplir las reglas del proveedor de alojamiento para evitar males mayores.

Esto es por lo que se recomienda adquirir su nombre de dominio en un Registrador Independiente (vea: [http://en.wikipedia.org/wiki/Domain\_name\_registrar](http://en.wikipedia.org/wiki/Domain\_name\_registrar)). Técnicamente, usted nunca comprará un nombre de dominio, solo lo "alquilará", normalmente a cambio de un pago anual. Esto le dá el derecho a usar ese nombre de dominio; pero tan pronto como deje de pagarlo, no podrá seguir usándolo y cualquier otro podría obtener el derecho de uso para sí mismo. Así que quizá sea mejor pagar por el dominio además de pagar por el hosting, de forma que podría mover este último a otro proveedor de alojamiento sin cargos adicionales; sólo cambie los DNSs de su nombre de dominio y en menos de 24 horas ese cambio se habrá propagado por toda la red volviendo a estar operativa de nuevo su tienda.

Si finalmente se decide a adquirir su nombre de dominio en un Registrador Independiente, aquí hay algunos en los que puede confiar:

* Gandi: [http://en.gandi.net/](http://en.gandi.net/)
* Namecheap: [http://www.namecheap.com/](http://www.namecheap.com/)
* PairNIC: [https://www.pairnic.com/](https://www.pairnic.com/)

Hay muchos más. Consultelo entre sus amistades!

#### Encontrar un hosting (alojamiento) <a href="#loquenecesitaparaempezar-encontrarunhosting-alojamiento" id="loquenecesitaparaempezar-encontrarunhosting-alojamiento"></a>

Ahora que ya tiene un nombre de domonio, necesitará adecuarlo a Prestashop. Esto significa que los archivos de Prestashop necesitan residir en un Servidor Web (webserver). Podría tener su propio servidor web pero quizá la mejor opcion sea confiar el alojamiento a un Proveedor de Servicios de Hosting (see: [http://en.wikipedia.org/wiki/Internet\_hosting\_service](http://en.wikipedia.org/wiki/Internet\_hosting\_service)), el cual le ofrecerá un alojamiento online adecuado a cambio de una cantidad mensual o anual variable.

Antes de comenzar una tienda online, necesitará selecciona un Proveedor de Hosting. Ciertamente, cualquier Proveedor de Hosting puede ofrecerle soluciones adecuadas para su tienda, pero solo unos pocos Proveedores de Hosting ofrecen servidores optimizados para Prestashop:=

* 1&1 en todos paises: [1&1](http://www.prestashop.com/es/ecommerce-hosting/1and1)
* InMotion Hosting en todos los paises, excepto en Francia y España: [InMotion](http://www.inmotionhosting.com/prestashop-hosting)\
  \


Échele un vistazo a nuestros [Partners de Hosting](http://www.prestashop.com/en/ecommerce-hosting)!

Cuando escoja su alojamiento, recuerde un requerimiento crítico: deberá ofrecerle soporte para PHP 5.2 (o superior), que es el lenguaje de programación en el está escrito Prestashop; y también MySQL 5 (o superior), que es el tipo de base de datos en el qeu Prestashop almacena todos sus datos. Hay algunos otros requerimientos: compruebe la sección "Requerimientos Técnicos" un poco más abajo.

PrestaBox

PrestaShop puede alojar su negocio online en sus propios Servidores in-house: nuestro servicio PrestaBox ha sido para liberar a los Responsables de Tienda de cualesquiera complicaciones técnicas, tales como instalar o actualizar Prestashop.

Por favor, consulte nuestra web PrestaBox para más detalles sobre nuestro servicio de alojamiento seguro y de precio bajo. Está altamente recomendado para Resposnables de Tienda con poca o ninguna experiencia en Internet o informática.

Puede conocer PrestaBox en esta url: [http://www.prestabox.com/](http://www.prestabox.com/)

#### Requerimientos Técnicos <a href="#loquenecesitaparaempezar-requerimientostecnicos" id="loquenecesitaparaempezar-requerimientostecnicos"></a>

PrestaShop es una aplicación que corre (se ejecuta) en un servidor web, y está programada usando el lenguaje de programación PHP. Adicionalmente, almacena sus datos en un servidor de bases de datos MySQL.

PHP es un lenguaje de programación de código abierto (open-source), principalmente usado para aplicaciones web. Creado en 1995, se ha convertido el en lenguaje de programación más usado por los desarrolladores web. Usa una sintaxis muy similar al lenguaje de programación C, siendo muy fácil de aprender para un desarrollador.

MySQL is un sistema de gestión de bases de datos, de código abierto (open-source). También creado en 1995, se ha convertido en el sistema de bases de datos más usado por desarrolladores web. Está basado en el lenguaje SQL, el lenguaje de bases de datos más extendido en la actualidad.

Independientemente del servicio de hosting (alojamiento) que usted elija, debería contar con estos componentes instalados en el servidor web:

* **Sistema**: Unix, Linux o Windows. Se recomienda encarecidamente el sistema Unix.
* **Servidor Web:** Apache Web server 1.3 o superior.
* **PHP 5.2 o superior**. Debería poder activar PHP 5 (pregunte a su proveedor de alojamiento).
* **MySQL 5.0 o superior**.
* Al menos 64 Mb de RAM en su servidor web (128 Mb es lo más adecuado, pero en general, cuanta más, mejor!).

PrestaShop puede también trabajar en un Servidor Web Microsoft IIS Web Server 6.0 o superior, y nginx 1.0 o superior.

Dispone de más información para Administradores de sistemas en la [Guía del Administrador de Sistemas](http://doc.prestashop.com/display/PS15/System+Administrator+Guide). Asegúrese de leerla (RTFM!)

#### Herramientas <a href="#loquenecesitaparaempezar-herramientas" id="loquenecesitaparaempezar-herramientas"></a>

Necesitará dos herramientas básicas: un editor de textos para poder editar archivos de texto, y un cliente (programa) de FTP, para poder transferir archivos desde su ordenador local a su servidor web y viceversa.

**Editor de Textos**

Aquí tiene unos cuantos editores de texto confiables y bien conocidos:

* Windows:
  * Notepad++: [http://notepad-plus-plus.org/](http://notepad-plus-plus.org/)
  * UltraEdit: [http://www.ultraedit.com/](http://www.ultraedit.com/)
  * Crimson Editor: [http://www.crimsoneditor.com/](http://www.crimsoneditor.com/)
* OS X:
  * Textmate: [http://macromates.com/](http://macromates.com/)
  * Coda: [http://www.panic.com/coda/](http://www.panic.com/coda/)
  * Smultron: [http://www.peterborgapps.com/smultron/](http://www.peterborgapps.com/smultron/)
* Unix/Linux:
  * Vim: [http://www.vim.org/](http://www.vim.org/)
  * Emacs: [http://www.gnu.org/software/emacs/](http://www.gnu.org/software/emacs/)

No use un procesador de texto del tipo Microsoft Word o Write de OpenOffice o LibreOffice. (N del T: insertan código oculto que puede estropear sus archivos de Prestashop)

**Cliente FTP**

FTP es el acrónimo para "File Transfer Protocol" (protocolo de transferencia de ficheros), que es la forma estándar de transferir archivos desde su ordenador local a un servidor web.

En esta guia, nosotros usamos Filezilla, que es un excelente (y gratuito) programa de FTP para Windows, Mac OS X y Linux. Puede descargarlo desde [http://filezilla-project.org/](http://filezilla-project.org/) y comenzar su instalación. Nota: no descargue FileZilla Server, solo FileZilla Client!

Una vez FilleZilla está instalado, necesitará configurarlo con los datos de su conexión FTP a su wervidor web, los cuales le habrán sido enviados por su empresa de alojamiento. Si no es así, pídaselos de nuevo (o revise la carpeta de spam de su email!).

Básicamente, los datos que necesita son:

* **Un hostname** (nombre del servidor ftp; usualmente algo como ftp.sudominio.com) o una **dirección IP:** será la forma de localizar su espacio web en el servidor donde se alojará su tienda.
* **Un nombre de usuario:** es el identificador de su cuenta de hosting, el cual es único para usted.
* **Una contraseña:** lo cual es una medida de seguridad básica.

Ejecute FileZilla, y abra la herramienta Gestor de Sitios. Puede hacerlo de tres formas distintas:

* Presione las teclas Ctrl-S,
* Haga click en el icono "Abrir el gestor de sitios", arriba, a la izquierda en la barra de menúes e iconos del programa,
* Abra el menú "Archivo" y seleccione la opción "Gestor de Sitios".

Hecho esto, se abrirá una ventana.

Para añadir su espacio en el servidor web al Gestor de Sitios:

1. Haga click en el botón "Nuevo Sitio". Se crea una nueva entrada en la lista de sitios. Déle un nombre que le resulte fácil de reconocer.
2. En el lado derecho, en la pestaña "General", inserte los parámetros que su proveedor de alojamiento le ha enviado (nombre del servidore, usuario y contraseña). No debería tener que cambiar el resto de parámetros por defecto, a menos que se lo indique su proveedor de alojamiento.
3. Una vez todos los campos han sido correctamente insertados, haga click en el boton "conectar". Esto guardará los datos de su nuevo sitio en la lista, y le permitirá acceder (login) a su cuenta en el servidor web, de forma que pueda estar seguro de que todo funciona correctamente.

Si FileZilla no se adapta a lo que necesita, aquí tiene otros programas de FTP muy conocidos:

* Windows:
  * CoreFTP: [http://www.coreftp.com/](http://www.coreftp.com/)
  * WinSCP: [http://winscp.net/](http://winscp.net/) (N del T: use solo este programa; es el único que guarda los datos de acceso a su servidor web encriptados; si su ordenador se vé infectado por troyanos, éstos no podrán leer esos datos ni acceder a su servidor web con ellos)
  * SmartFTP: [http://www.smartftp.com/](http://www.smartftp.com/)
* Mac OS X:
  * Cyberduck: [http://cyberduck.ch/](http://cyberduck.ch/)
  * Transmit: [http://www.panic.com/transmit/](http://www.panic.com/transmit/)
  * Fetch: [http://fetchsoftworks.com/fetch/](http://fetchsoftworks.com/fetch/)
* Unix/Linux:
  * gFTP: [http://gftp.seul.org/](http://gftp.seul.org/)
  * kasablanca: [http://kasablanca.berlios.de/](http://kasablanca.berlios.de/)
  * NcFTP: [http://www.ncftp.com/ncftp/](http://www.ncftp.com/ncftp/)

#### Estableciendo una planificación <a href="#loquenecesitaparaempezar-estableciendounaplanificacion" id="loquenecesitaparaempezar-estableciendounaplanificacion"></a>

Ahora debe decidir donde quiere alojar su tienda PrestaShop. Hay cuatro posibilidades relativas a su nombre de dominio (a su dominio):

* En la raiz del dominio: [http://www.ejemplo.com/](http://www.example.com/)
* En una carpeta: [http://www.ejemplo.com/tienda/](http://www.example.com/shop/)
* En un subdominio: [http://tienda.ejemplo.com/](http://store.example.com/)
* En una carpeta de un subdominio: [http://moda.ejemplo.com/boutique/](http://clothes.example.com/boutique/)

Tenga en cuenta que gracias a la característica "Multitienda", puede tener tantas tiendas como necesite con una única instalación de PrestaShop 1.6, cada una de ellas con su propio dominio específico si es necesario. Debería tenerlo en cuenta cuando decida qué hacer finalmente.\
&#x20;Independientemente de lo que decida, la tienda por defecto estará siempre donde la instalación de Prestashop se haya realizado físicamente.

#### Instalando PrestaShop <a href="#loquenecesitaparaempezar-instalandoprestashop" id="loquenecesitaparaempezar-instalandoprestashop"></a>

Finalmente, ahora que todos los datos están en su lugar, puede usar la guia de instalación: [http://doc.prestashop.com/display/PS16/Installing+PrestaShop](http://doc.prestashop.com/display/PS16/Installing+PrestaShop).
