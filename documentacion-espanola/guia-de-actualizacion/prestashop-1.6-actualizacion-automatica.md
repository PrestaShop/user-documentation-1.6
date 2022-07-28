# PrestaShop 1.6 : Actualización automática

**Tabla de contenidos**\
****

/\*\<!\[CDATA\[\*/\
div.rbtoc1597066537537 {padding: 0px;}\
div.rbtoc1597066537537 ul {list-style: disc;margin-left: 0px;}\
div.rbtoc1597066537537 li {margin-left: 0px;padding-left: 0px;}\
\
/\*]]>\*/

* [Actualización automática](prestashop-1.6-actualizacion-automatica.md#Actualizaciónautomática-Actualizaciónautomática)
  * [Descarga e instalación del módulo 1-Click Upgrade](prestashop-1.6-actualizacion-automatica.md#Actualizaciónautomática-Descargaeinstalacióndelmódulo1-ClickUpgrade)
  * [La pantalla de configuración](prestashop-1.6-actualizacion-automatica.md#Actualizaciónautomática-Lapantalladeconfiguración)
    * [Bienvenido](prestashop-1.6-actualizacion-automatica.md#Actualizaciónautomática-Bienvenido)
    * [La lista de comprobación previa a la actualización](prestashop-1.6-actualizacion-automatica.md#Actualizaciónautomática-Lalistadecomprobaciónpreviaalaactualización)
    * [Comenzar actualización](prestashop-1.6-actualizacion-automatica.md#Actualizaciónautomática-Comenzaractualización)
    * [Comparación de versiones](prestashop-1.6-actualizacion-automatica.md#Actualizaciónautomática-Comparacióndeversiones)
    * [Deshacer](prestashop-1.6-actualizacion-automatica.md#Actualizaciónautomática-Deshacer)
    * [Opciones de copia de seguridad](prestashop-1.6-actualizacion-automatica.md#Actualizaciónautomática-Opcionesdecopiadeseguridad)
    * [Opciones de actualización](prestashop-1.6-actualizacion-automatica.md#Actualizaciónautomática-Opcionesdeactualización)
  * [El proceso de actualización](prestashop-1.6-actualizacion-automatica.md#Actualizaciónautomática-Elprocesodeactualización)
  * [Volviendo a la versión anterior: deshacer](prestashop-1.6-actualizacion-automatica.md#Actualizaciónautomática-Volviendoalaversiónanterior:deshacer)
  * [Volviendo a la versión anterior: restauración de su propia copia de seguridad](prestashop-1.6-actualizacion-automatica.md#Actualizaciónautomática-Volviendoalaversiónanterior:restauracióndesupropiacopiadeseguridad)

## Actualización automática <a href="#actualizacionautomatica-actualizacionautomatica" id="actualizacionautomatica-actualizacionautomatica"></a>

La herramienta de actualización automática de PrestaShop permite a los propietarios de tiendas hacer copias de seguridad y actualizar su sitio en pocos clics sin la necesidad de tener conocimientos técnicos.

El módulo 1-Click Upgrade debería de estar disponible de forma predeterminada en la página "Módulos" de su tienda (dentro de la categoría "Administración"): simplemente realizando un clic en el botón Instalar perteneciente a éste módulo, podrá utilizarlo para actualizar a la última versión de PrestaShop.

Nunca actualice su tienda online directamente. La herramienta de actualización automática puede fallar en algunas situaciones, y probablemente no podría volver a la versión anterior que tenía instalada.

La forma más segura de realizar este proceso es tener disponible una copia exacta de su tienda,  ya sea en el equipo local o en otra carpeta de su servidor web. Ésta deberá contener todos sus productos, categorías, temas, módulos, traducciones, ajustes personalizados, etc.

Realice una actualización de prueba sobre esa copia de su tienda. Una vez que la actualización se haya completado, navegue a través de las páginas del front office y back office de la tienda para asegurarse de que todo está tal y como esperaba. Si no es así, entonces la herramienta de actualización automática tiene un problema con su configuración, y debería utilizar el método manual de actualización, que ahora está obsoleto y requiere de más tiempo, pero que podría serle de ayuda en su situación.

### Descarga e instalación del módulo 1-Click Upgrade <a href="#actualizacionautomatica-descargaeinstalaciondelmodulo1-clickupgrade" id="actualizacionautomatica-descargaeinstalaciondelmodulo1-clickupgrade"></a>

Si el módulo 1-Click Upgrade no está disponible en su instalación de PrestaShop 1.4 o 1.5, puede descargarlo gratuitamente desde el sitio web de Complementos de PrestaShop (PrestaShop Addons).

Incluso si ya tiene instalado el módulo "1-Click upgrade", asegúrese de que está utilizando la última versión disponible:

* PrestaShop 1.4: Compruebe el número de versión en la pestaña "Módulos", a continuación comparelo con el número de versión que aparece en el sitio web de Complementos de PrestaShop (véase más abajo). Si los números son diferentes y la versión que tiene instalada es menor de la que está disponible en el sitio web de Complementos, descarguela y actualice el módulo.\

  * Para actualizar el módulo: desinstálelo y elimínelo desde el Panel de Administración de PrestaShop, a continuación, copie la carpeta "/autoupgrade" desde el archivo del módulo (que ha descargado desde el sitio web de Complementos) a la carpeta "/modules" de su instalación de PrestaShop. Por último, instale el módulo desde el Panel de Administración.
* PrestaShop 1.5 y versiones posteriores: PrestaShop se conectará automáticamente al sitio web de Complementos para comprobar si existen nuevas versiones de sus módulos. Si una nueva versión está disponible, se presentará un nuevo botón "¡Actualícelo! (Actualizar)" justo al lado del botón "Instalar / Desinstalar". Haga clic en él para que PrestaShop se encargue de descargar y actualizar el módulo por usted.

Tan sólo tiene que seguir los pasos que realiza habitualmente para instalar un módulo en PrestaShop:

1. Descargue el módulo 1-Click Upgrade desde PrestaShop Addons: [http://addons.prestashop.com/es/administracion-prestashop-modulo/5496-1-click-upgrade-autoupgrade.html](http://addons.prestashop.com/es/administracion-prestashop-modulo/5496-1-click-upgrade-autoupgrade.html). Guarde el archivo Zip en su escritorio.
2. En su Panel de Administración de PrestaShop, diríjase a la página "Módulos" del menú "Módulos".
3.  Haga clic en el botón "Añadir nuevo módulo", situado en la parte superior derecha de la lista de módulos disponibles.

    Si está actualizando desde la version 1.4, haga clic en el enlace "Añadir un nuevo módulo a partir de mi ordenador", situado en la parte superior izquierda.
4. En el formulario que se abre, haga clic en el botón "Seleccionar (Elegir un fichero)...", a continuación, busque y seleccione el archivo Zip del módulo que acaba de descargar.
5. Haga clic en el botón "Subir este módulo". PrestaShop pondrá el módulo en su servidor, lo descomprimirá, y colocará los archivos en la carpeta `/modules`.

El módulo estará ahora disponible en el listado de módulos, pero todavía tendrá que instalarlo:

1. En la pestaña "Módulos", encuentre el módulo 1-Click Upgrade: teclee "1-click upgrade" o "autoupgrade" en el cuadro de búsqueda de módulos (no lo haga en la búsqueda global en la parte superior). Un enlace directo al módulo debería aparecer a medida que escribe. Haga clic sobre dicho enlace.
2. PrestaShop a continuación, mostrará el módulo en el listado principal de módulos.
3. Haga clic en el botón "Instalar" del módulo.

El módulo está ahora preparado para que lo configure y lo utilice.

### La pantalla de configuración <a href="#actualizacionautomatica-lapantalladeconfiguracion" id="actualizacionautomatica-lapantalladeconfiguracion"></a>

La pantalla de configuración del módulo está disponible en el listado de "Módulos", haciendo clic en el botón o enlace "Configurar".

La pantalla de configuración también está disponible en:

* PrestaShop 1.4: bajo la pestaña "Herramientas", en la subpestaña "1-Click Upgrade".
* PrestaShop 1.5 y posterior: bajo los "Parámetros avanzados", en la página "1-Click Upgrade".

La pantalla de configuración le presenta una serie de secciones, proveyendo información, herramientas y ajustes.

#### Bienvenido <a href="#actualizacionautomatica-bienvenido" id="actualizacionautomatica-bienvenido"></a>

Esta pequeña sección sirve como recordatorio de que una actualización nunca es 100% segura, y por lo tanto usted debe asegurarse de que ha hecho una copia de seguridad completa de sus archivos y datos antes de realizar este proceso. De esta manera, si la actualización fallará, podría regresar al estado inicial de su tienda shop – aunque con un poco de trabajo volviendo a poner los archivos y datos en su lugar correspondiente.

Este proceso se explica en detalles en el capítulo "Cómo realizar y restaurar su propia copia de seguridad" de esta guía: [http://doc.prestashop.com/display/PS16/Making+and+restoring+your+own+backup](http://doc.prestashop.com/display/PS16/Making+and+restoring+your+own+backup).

![](<../../.gitbook/assets/23038081 (1).png>)

Tenga en cuenta que el módulo 1-Click Upgrade realiza una copia de seguridad propia, con el fin de permitir la reversión total de la actualización. Sin embargo, usted siempre debe realizar sus propias copias de seguridad.

#### La lista de comprobación previa a la actualización <a href="#actualizacionautomatica-lalistadecomprobacionpreviaalaactualizacion" id="actualizacionautomatica-lalistadecomprobacionpreviaalaactualizacion"></a>

La sección "comprobación pre-actualización" le proporciona información valiosa sobre la instalación actual de PrestaShop, y cómo ésta podría interactuar con la actualización automática.

![](<../../.gitbook/assets/23038082 (1).png>)

Deberá asegurarse de que todas las comprobaciones se validan antes de poder iniciar la actualización.

* **El módulo 1-click upgrade está actualizado (su versión actual es x.x)**. Indica si es necesario actualizar el propio módulo de actualización. Si acaba de instalarlo, hay pocas posibilidades de que tenga que actualizarlo.\
  Si no tiene la última versión del módulo, un botón aparece debajo de este campo, advirtiendo de que "Instale la última versión haciendo clic 'Añadir a partir de mi ordenador'". Al hacer clic será redirigido a la página "Módulos". Desde dicha página, haga clic sobre el enlace "Añadir módulo a partir de mi ordenador" para revelar el formulario  correspondiente tras la precarga de la página. Haga clic en el botón "Descargar este módulo" para iniciar la actualización del módulo. Finalmente, regrese a la página de configuración del módulo 1-Click Upgrade para continuar la realización de comprobaciones previas a la actualización.
* **El directorio raíz de su tienda debe tener permisos de escritura (permisos CHMOD apropiados)**. Indica si los permisos de lectura / escritura están correctamente establecidos. Si no lo estuvieran, tendrá que cambiarlos, utilizando un cliente FTP, como por ejemplo FileZilla.\
  &#x20;Consulte la sección "Compatibilidad y Configuración del Sistema" de la Guía de Introducción dentro del capítulo "Instalación de PrestaShop", para obtener una rápida explicación de cómo realizar un CHMOD.
* **La opción PHP "Modo seguro" debe estar deshabilitada**.
* **La opción PHP "allow\_url\_fopen" debe estar habilitada o CURL debe estar instalado**.
* **Debe poner su tienda en modo de mantenimiento**. Indica si su tienda está activa o en modo de mantenimiento. Recuerde poner su tienda en modo mantenimiento mientras se está realizando el proceso (copia de seguridad de archivos, copias de seguridad de base de datos, actualización automática, verificación), con el fin de evitar que los clientes puedan perder pedidos... y prevenirle a usted la perdida de clientes. El módulo puede desactivar su tienda por usted: Simplemente haga clic en el botón "Haga clic aquí para poner su tienda en mantenimiento". También puede optar por desactivar la tienda manualmente, utilizando la página de preferencias de la tienda:\

  * PrestaShop 1.4: activar/desactivar la tienda, en la pestaña principal "Preferencias".
  * PrestaShop 1.5 y superior: activar/desactivar la tienda, en la página "Mantenimiento", bajo el menú "Preferencias".
* **Debe deshabilitar las características de almacenamiento en caché de PrestaShop**. Indica si la caché de su tienda está activada o desactivada. Debe desactivarla durante todo el proceso. El módulo no lo hará por usted.\

  * PrestaShop 1.4: activar/desactivar la caché, en la página "Rendimiento", bajo la pestaña "Preferencias".
  * PrestaShop 1.5 y superior: activar/desactivar la caché, en la página "Rendimiento", bajo el menú "Parámetros avanzados".
* **El tiempo límite PHP tiene un valor muy alto o se encuentra desactivado completamente (Valor actual: xxx)**. La actualización automática puede ser un proceso largo, ya que se tiene que descargar este archivo desde [prestashop.com](http://prestashop.com), descromprimirlo en el servidor, reemplazar los archivos instalados actualmente, y lanzar la propia actualización en sí. Por tanto, el ajuste de este parámetro en  PHP podría estar establecido en un valor demasiado bajo, e interrumpir la actualización definitivamente en medio del proceso. En este campo, PrestaShop le ofrece una indicación del ajuste establecido en la configuración PHP. Idealmente, ésta debería indicar "desactivado".

Todos estos indicadores deben ser de color verde para que la actualización pueda realizarse. De lo contrario, el botón de actualización no aparecerá en pantalla.

Cuando su tienda está alojada en un servidor local ([`http://localhost`](http://localhost) o [`http://127.0.0.1`](http://127.0.0.1)), el módulo de actualización automática entiende que no se requiere el modo de mantenimiento, ya que nadie más que usted puede acceder al sitio. Por lo tanto, incluso auque usted no haya establecido su tienda en modo de mantenimiento, el módulo marcará esta comprobación como válida.

#### Comenzar actualización <a href="#actualizacionautomatica-comenzaractualizacion" id="actualizacionautomatica-comenzaractualizacion"></a>

En esta sección se compara su versión de PrestaShop con la última estable. Puede comprobar rápidamente si necesita actualizar o no. Si usted sabe que hay una nueva versión disponible más actual de la que se presenta, puede lanzar una comprobación de versión haciendo clic en el botón "Verificar si una nueva versión está disponible".

![](<../../.gitbook/assets/23038083 (1).png>)

Por defecto, la herramienta de actualización está configurada para actualizar su tienda a la próxima versión menor disponible. Esto significa que si usted utiliza una versión de la rama 1.4.x, ésta no le sugerirá la última versión 1.6.x disponible, sino que antes le ofrecerá actualiza a la última versión 1.4.x disponible. Por lo tanto, si desea actualizar desde una versión 1.4.x a la última versión 1.6.x, deberá hacer clic en el botón "Más opciones (modo Experto)". Tras realizar esta acción se abrirá una nueva sección, denominada "Más opciones (modo Experto)", donde puede elegir el canal de distribución desde el que desea actualizar.\
Esta opción también es muy útil si desea comprobar si hay una versión disponible que no esté considerada como  estable (por ejemplo, beta, RC o cualquier otra versión considerada inestable).

Antes de lanzar la actualización, debe asegurarse de que usted entiende completamente sus ajustes. Las secciones "Opciones de copia de seguridad" y "Opciones de actualización" se encuentran disponibles en la parte inferior de la página (y se describen más adelante en este capítulo).&#x20;

**Modo Experto**

Esta sección le permite determinar exactamente a qué versión desea actualizar su versión de PrestaShop actualmente instalada.

![](<../../.gitbook/assets/23038084 (1).png>)

Las opciones son:

* **Canal**. Elija el canal de distribución desde el que desea utilizar. Se le recomienda seleccionar "Lanzamiento de versiones menores", lo que significa "cualquier versión estable por encima de la actual". Las otras opciones son:\

  * **Lanzamiento de versiones mayores**. El próximo lanzamiento estable desde la última rama: dado que la rama actual es la 1.6.x, la herramienta de actualización usaría la última versión 1.6 (a partir de este escrito, v1.6.0).
  * **Lanzamiento de versiones menores**. _Esta es la configuración establecida de forma predeterminada._ Utiliza sólo la próxima versión estable dentro de la rama actual:  si usted tiene instalada la versión 1.4.2 de PrestaShop, se actualizará su tienda a la versión 1.4.9, incluso aunque la versión 1.6.2 esté disponible.
  * **Versiones candidatas a definitivas**. Las versiones RC (Release Candidate) son consideradas lo suficientemente estables como para poder ser probadas por la mayoría, pero no lo suficientemente estables como para ser lanzadas como una versión estable final. Utilícelas bajo su propio riesgo.
  * **Lanzamientos Beta**, **lanzamientos alpha**. Estas son versiones de desarrollo . Utilícelas bajo su propio riesgo.
  * **Lanzamientos Privados**. En algunas ocasiones, los desarrolladores de PrestaShop suben una versión de prueba privada. Si usted tiene la URL correcta y la clave hash, puede actualizar a esta versión fácilmente utilizando este canal. Si marca la casilla de verificación "Permitir actualizaciones mayores", usted indicará que sólo está interesado en las versiones mayores.
  * **Archivo local**. Para ser utilizada si ha descargado la versión a la que desea actualizar dentro de la carpeta local correcta, `/admin/autoupgrade/download`. Una vez que haya seleccionado archivo en el selector desplegable, indique el número de versión en el campo de texto (¡sea muy preciso!).
  * **Directorio local**. Para ser utilizada si se ha descargado y descomprimido la versión que desea actualizar dentro de la carpeta `/admin/autoupgrade/latest/prestashop`. Esta carpeta `/prestashop` debe provenir directamente del archivo que ha descargado.
* **rama**. Indica si hay alguna versión disponible en el canal seleccionado.
* **nombre**. El nombre de la última versión disponible en el canal seleccionado.
* **url**. La URL de la última versión en el canal seleccionado.
* **md5**. La suma de comprobación hash de la versión más reciente en el canal seleccionado.

#### Comparación de versiones <a href="#actualizacionautomatica-comparaciondeversiones" id="actualizacionautomatica-comparaciondeversiones"></a>

Para los más curiosos, esta sección enumera las diferencias entre la versión actual y la versión más reciente del canal seleccionado.&#x20;

![](<../../.gitbook/assets/23038085 (2).png>)

En el caso de haber realizado cambios directamente sobre los archivos principales de PrestaShop en lugar de haber utilizado las capacidades y técnicas override, esta lista puede ayudarle a saber si los cambios son seguros o no.\
&#x20;No obstante, recuerde que puede mejorar la vida útil de su código personalizado convirtiéndolos en archivos primordiales utlizando overriding. Al utilizar esta técnica su código personalizado no se verá afectado por las actualizaciones. Consulte la documentación destinada a desarrolladores para obtener más información.

#### Deshacer <a href="#actualizacionautomatica-deshacer" id="actualizacionautomatica-deshacer"></a>

Esta sección sólo aparece cuando se ha realizado al menos una actualización.

Veáse abajo para obtener más información.

#### Opciones de copia de seguridad <a href="#actualizacionautomatica-opcionesdecopiadeseguridad" id="actualizacionautomatica-opcionesdecopiadeseguridad"></a>

Estas opciones le permiten tener un cierto control sobre el proceso de copia de seguridad:

* **Copia de seguridad de mis archivos y base de datos**. Usted debe realizar una copia de seguridad, y el módulo se hará cargo este trabajo para que usted no tenga que hacerlo. Nunca debe desactivar esta opción, a menos que se le indique.
* **Copia de seguridad de mis imágenes**. Usted debe permitir que el módulo también se encargue de cuidar sus imágenes, para que cuando tenga que hacer una reinstalación desde cero, no tenga que volver a resubir sus archivos.&#x20;

![](<../../.gitbook/assets/23038086 (1).png>)

#### Opciones de actualización <a href="#actualizacionautomatica-opcionesdeactualizacion" id="actualizacionautomatica-opcionesdeactualizacion"></a>

Estas opciones le permiten tener un cierto control sobre el proceso de actualización:

* **Rendimiento del servidor**. Algunos hostings compartidos ofrecen un rendimiento deficiente, lo que podría dificultar el rendimiento del proceso de actualización, o incluso hacer que éste falle por completo. "Bajo" es seleccionado de manera predeterminada, pero si usted sabe que tiene un servidor potente, deberá seleccionar "Medio" o incluso "Alto".
* **Desactivar módulos no nativos**. Se recomienda elegir la opción "Sí" en esta opción, ya que algunos módulos podrían resultar ser un obstáculo al actualizar PrestaShop.
* **Actualizar el tema "predeterminado"**. El proceso de actualización sobrescribe el tema por defecto y lo sobreescribe por el de la última versión. Si ha realizado modificaciones en el tema directamente, puede protegerlas  seleccionando "No". ¡Recuerde que no se recomienda editar el tema predeterminado directamente!. Haga una copia del tema, y realice los cambios sobre esa copia, para evitar inconvenientes.
* **Actualizar los mensajes de correo electrónico predeterminados**. Una actualización podría traer nuevas plantillas de correo electrónico predeterminadas. Por defecto, la actualización reemplazará las ya existentes por las del archivo más reciente, y añadirá las nuevas plantillas. Si tiene plantillas personalizadas, se recomienda mantenerlas. Tendrá que personalizar las nuevas plantillas con el fin de ajustarlas al estilo general de su tienda.
* **Modo paso a paso**. _Sólamente disponible en modo Dev_. Si esta opción está habilitada, el módulo se detendrá en cada paso para pedirle una confirmación antes de realizar el proceso.
* **Mostrar errores PHP**. _Sólamente disponible en modo Dev_. Si esta opción está habilitada, el módulo mostrará los errores PHP, que podrían servirle de ayuda para descubrir los problemas del servidor que de otro modo permanecen ocultos a la vista.

![](<../../.gitbook/assets/23038087 (1).png>)

### El proceso de actualización <a href="#actualizacionautomatica-elprocesodeactualizacion" id="actualizacionautomatica-elprocesodeactualizacion"></a>

Una vez que todos los indicadores de la sección "Lista de comprobación pre-actualizacion" se encuentren con la marca de verificación de color verde, el botón de actualización aparece en la sección "Comenzar actualización", junto con la URL desde la que se descargará la nueva versión.

Haga clic en el botón "¡Comenzar actualización ahora!" para lanzar el proceso completo.

Una vez que se puso en marcha el proceso de actualización, la página de configuración general es sustituida por dos secciones: "Registro de actividad" y "Deshacer".

El registro de actividad le muestra un registro detallado de lo que el programa de actualización está haciendo en una pantalla por la que puede desplazarse:

* Archivos eliminados: Tan sólo los archivos de ejemplo son eliminados, tales como clases de anulación (override) vacías y controladores.
* Nombre del archivo de la copia de seguridad: el nombre sigue la forma `auto-backupfiles_V1.6.0.2_20140127-120310-798d3a69.zip`.
* Archivos añadidos al archivo de la copia de seguridad: todos los archivos restantes de la instalación actual incluidos en el archivo Zip.
* Tablas de bases de datos añadidas al archivo de la copia de seguridad: sus archivos son importantes, pero todo su catálogo se almacena en su base de datos, así que ésta es guardada en el mismo archivo.
* Archivos eliminados: mayormente módulos, controladores, clases, archivos CSS y archivos JavaScript. Ahora que todos los archivos se han guardado en el archivo de la copia de seguridad, ellos pueden ser eliminados de forma segura.
* Archivos copiados desde el nuevo archivo: todos los archivos existentes se sustituirán por los de la nueva versión.
* Archivos de traducción fusionados.
* Tablas de base datos creadas, eliminadas, alteradas y actualizadas.
* Directorios temporales vaciados: si es posible, el actualizador tratará de borrar el contenido de los directorios caché.

Un monton de archivos son mencionados durante el proceso. No es necesario que se detenga a leer todas las notificaciones que aparecen en pantalla, usted es libre de consultarlas tan sólamente en caso de error.

Sabrá que la actualización ha terminado cuando aparezca el siguiente mensaje en color verde "Actualización completa. Por favor, compruebe si su tema principal es funcional (trate de hacer una compra, compruebe el tema)", junto con la siguiente entrada de registro final: "Fin del proceso".\
La herramienta de actualización también indica que debe volver a habilitar su tienda, pero antes de hacerlo, deberá  comprobar que todo funciona en el back-office de su tienda : no hay errores, todos los productos y categorías están en su lugar con sus imágenes y archivos adjuntos correspondientes, etc. Hasta que no haya comprobado que todo está bien en su tienda, es mejor evitar que su tienda sea pública.

En la primera carga, las páginas podrían aparecer con un aspecto roto o desorganizado: debido a que su navegador web almacena en caché los archivos, probablemente esté haciendo uso de los viejos archivos CSS en lugar de los nuevos. No dude en recargar la página varias veces, o incluso vaciar la caché del navegador, con el fin de obtener la interfaz correctamente actualizada.

Al actualizar desde la versión 1.4 a la versión 1.6, sus menús no serán organizados de la misma forma en la que lo harían si realiza una instalación desde cero de la version 1.6.

Esto es debido a que las pestañas de PrestaShop 1.4 fueron reorganizadas dentro de menús en PrestaShop 1.6, y una gran cantidad de páginas fueron movidas y trasladadas con el fin de crear menús consistentes. Además, la herramienta de actualización asume que sus pestañas en PrestaShop 1.4 podrían haber sido personalizadas o movidas, ya sean por sí mismas o por la acción de un módulo. Por lo tanto, en lugar de eliminar la configuración existente, la herramienta de actualización toma las pestañas como las encuentra , y no las reorganiza en el orden predeterminado de los menús de PrestaShop 1.6.

Si desea cambiar el posicionamiento de las páginas dentro de un menú una vez que haya actualizado a la versión 1.6, diríjase a la página "Menus" bajo el menú "Administración", y comience a realizar los ajustes que considere necesario en las posiciones.

Una vez que se haya asegurado de que su instalación de PrestaShop está plenamente funcional, deberá volver a activar su tienda utilizando la opción disponible en la página "Mantenimiento" del menú "Preferencias", a continuación realice de nuevo una comprobación del front office de su tienda: buscar productos, ordenarlos, realizar el proceso de pedido de uno de ellos , etc.

**¿Está todo funcionando perfectamente?. ¡Enhorabuena, ha realizado el proceso de actualización de PrestaShop correctamente!**

JavaScript error

En algunas configuraciones de servidor, un mensaje de error puede aparecer, indicando lo siguiente "Javascript error (parseJSON) detected for action "upgradeNow". Starting restoration...", en español: "Error Javascript(parseJSON) detectado por acción..."upgradeNow". Empezando la restauración..."

&#x20;Siga estos pasos para resolver el error,:\


* Abra el archivo `php.ini` y habilite (descomentando) las extensiones MySQLi y MySQL PDO. Si no tiene acceso al archivo `php.ini`, póngase en contacto con su proveedor de alojamiento web.
*   Abra el archivo `/modules/autoupgrade/db/Db.php` y encuentre las siguientes líneas de código (alrededor de la línea 210):

    ```
    public static function getClass()
    {
        $class = 'MySQL';
        /*if (PHP_VERSION_ID >= 50200 && extension_loaded('pdo_mysql'))
            $class = 'DbPDO';
        else if (extension_loaded('mysqli'))
            $class = 'DbMySQLi';*/
        return $class;
    }
    ```

    Lo único que tiene que hacer es descomentar estas líneas (quitando los carácteres `/*` y `*/`, presentes en el bucle `if - else if`). El resultado final debe ser el siguiente:

    ```
    public static function getClass()
    {
        $class = 'MySQL';
        if (PHP_VERSION_ID >= 50200 && extension_loaded('pdo_mysql'))
            $class = 'DbPDO';
        else if (extension_loaded('mysqli'))
            $class = 'DbMySQLi';
        return $class;
    }
    ```

Después de haber hecho todo esto, inicie el proceso de actualización de nuevo.

### Volviendo a la versión anterior: deshacer <a href="#actualizacionautomatica-volviendoalaversionanterior-deshacer" id="actualizacionautomatica-volviendoalaversionanterior-deshacer"></a>

Lamentablemente, no todas las actualizaciones son exitosas – esta es la razón por la que **siempre**  debe hacer una copia de seguridad de todos sus archivos y datos, y por la que PrestaShop realiza una copia de seguridad adicional de dichos archivos y datos por sí mismo, con la que no siempre debería de contar. **Haga siempre su propia copia de seguridad primero**. Consúlte el capítulo "Cómo realizar y restaurar su propia copia de seguridad" de esta guía para obtener más información.

Los archivos de la copia de seguridad que realiza por sí mismo PrestaShop, son guardados en su servidor. Si resulta que la actualización ha ido mal, puede encontrar estos archivos en la sección "Deshacer" de la página de configuración del módulo 1-Click Upgrade.\
Los archivos de la copia de seguridad se crean tan pronto como se inicia el proceso de actualización, y están disponibles inmediatamente bajo la lista desplegable "Elija una copia de seguridad a restaurar".\
&#x20;Seleccione la más reciente. La fecha y la hora de la creación del archivo de copia de seguridad son añadidas junto con el nombre: `Vversion-date-hour-random`, por ejemplo "V1.4.9.0\_20120907-114024-f85f41a" de una copia de seguridad de una instalación perteneciente a PrestaShop 1.4.9, realizada el 7 de Septiembre de 2012, a las 11:40:24 de la mañana.

El botón "Deshacer" desencadena dos acciones:

* Toma los archivos de la última copia de seguridad, y los vuelve a instalar en lugar de los de la versión actual instalada.
* Toma los datos de la última copia de seguridad, y los vuelve a instalar a partir de la base de datos actual.

Seleccione el archivo de la copia de seguridad a la que desea volver y haga clic en el botón "Deshacer". Al igual que con el proceso de actualización, toda la interfaz desaparece para dejar solamente las secciones "Registro de actividad" y "Deshacer". Puede seguir el proceso de reversión desplazándose por el registro de actividad.\
Una vez que completado el proceso, recargue la página para comprobar que todo ha regresado a su lugar.

### Volviendo a la versión anterior: restauración de su propia copia de seguridad <a href="#actualizacionautomatica-volviendoalaversionanterior-restauraciondesupropiacopiadeseguridad" id="actualizacionautomatica-volviendoalaversionanterior-restauraciondesupropiacopiadeseguridad"></a>

Este proceso se explica con detalle en el capítulo "Cómo realizar y restaurar su propia copia de seguridad" de esta guía: [http://doc.prestashop.com/display/PS16/Making+and+restoring+your+own+backup](http://doc.prestashop.com/display/PS16/Making+and+restoring+your+own+backup).
