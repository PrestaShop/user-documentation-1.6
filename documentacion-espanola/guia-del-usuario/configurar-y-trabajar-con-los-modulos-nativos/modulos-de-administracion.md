# Módulos de Administración

/\*\<!\[CDATA\[\*/\
div.rbtoc1597066520254 {padding: 0px;}\
div.rbtoc1597066520254 ul {list-style: disc;margin-left: 0px;}\
div.rbtoc1597066520254 li {margin-left: 0px;padding-left: 0px;}\
\
/\*]]>\*/

* [Módulos de Administración](modulos-de-administracion.md#MódulosdeAdministración-MódulosdeAdministración)
  * [1-Click Upgrade - AutoUpgrade](modulos-de-administracion.md#MódulosdeAdministración-1-ClickUpgrade-AutoUpgrade)
  * [Cumplimiento de la legislación europea](modulos-de-administracion.md#MódulosdeAdministración-Cumplimientodelalegislacióneuropea)
    * [Opciones de Etiqueta](modulos-de-administracion.md#MódulosdeAdministración-OpcionesdeEtiqueta)
    * [Características](modulos-de-administracion.md#MódulosdeAdministración-Características)
    * [Gestionar el contenido legal](modulos-de-administracion.md#MódulosdeAdministración-Gestionarelcontenidolegal)
    * [Inclusión del contenido del correo electrónico](modulos-de-administracion.md#MódulosdeAdministración-Inclusióndelcontenidodelcorreoelectrónico)
  * [Gestor de tareas Cron](modulos-de-administracion.md#MódulosdeAdministración-GestordetareasCron)
  * [Boletín de noticias](modulos-de-administracion.md#MódulosdeAdministración-Boletíndenoticias)
    * [Exportar suscriptores del Boletín de noticias](modulos-de-administracion.md#MódulosdeAdministración-ExportarsuscriptoresdelBoletíndenoticias)
    * [Exportar clientes](modulos-de-administracion.md#MódulosdeAdministración-Exportarclientes)
  * [Limpiador de Prestashop](modulos-de-administracion.md#MódulosdeAdministración-LimpiadordePrestashop)
  * [Alertas por correo](modulos-de-administracion.md#MódulosdeAdministración-Alertasporcorreo)
    * [Notificaciones de cliente](modulos-de-administracion.md#MódulosdeAdministración-Notificacionesdecliente)
    * [Notificaciones del comerciante](modulos-de-administracion.md#MódulosdeAdministración-Notificacionesdelcomerciante)
  * [Google Analytics API](modulos-de-administracion.md#MódulosdeAdministración-GoogleAnalyticsAPI)
  * [Marca de agua (filigrana)](modulos-de-administracion.md#MódulosdeAdministración-Marcadeagua\(filigrana\))
  * [Experiencia Comercial](modulos-de-administracion.md#MódulosdeAdministración-ExperienciaComercial)
  * [Diagramas NVD3](modulos-de-administracion.md#MódulosdeAdministración-DiagramasNVD3)
  * [Primeros pasos](modulos-de-administracion.md#MódulosdeAdministración-Primerospasos)
  * [Mostrar HTML simple](modulos-de-administracion.md#MódulosdeAdministración-MostrarHTMLsimple)

## 1-Click Upgrade - AutoUpgrade <a href="#modulosdeadministracion-1-clickupgrade-autoupgrade" id="modulosdeadministracion-1-clickupgrade-autoupgrade"></a>

Este módulo facilita en gran medida la actualización de PrestaShop a su última versión.

Véase el capítulo "Actualización automática" de la guía de Actualización de PrestaShop para conocer todos los detalles de este módulo: [http://doc.prestashop.com/display/PS16/Automatic+update](http://doc.prestashop.com/display/PS16/Automatic+update).

## Cumplimiento de la legislación europea <a href="#modulosdeadministracion-cumplimientodelalegislacioneuropea" id="modulosdeadministracion-cumplimientodelalegislacioneuropea"></a>

_Novedad en PrestaShop 1.6.1.0._

El módulo Cumplimiento de la legislación europea ayuda a los comerciantes a hacer que sus tiendas cumplan con las recientes y más restrictivas regulaciones de la UE.

Este es un módulo imprescindible para tiendas europeas.

La mayoría de sus opciones están destinadas a proporcionar más transparencia a los clientes finales, mediante:

* Etiquetas de precios más detalladas (precio por unidad, precio anterior, impuestos, tarifas de envío, plazos de entrega, peso del producto, etc.)
* Página del proceso de pago avanzada
* Contenido legal adjunto para correos electrónicos

No todas las opciones incluidas en este módulo serán útiles para todos los países, pero seguro que alguna de ellas te ayuda a que tu tienda cumpla con las leyes de comercio electrónico de la UE.\
La configuración predeterminada es la configuración recomendada; pero es libre de habilitar o deshabilitar las opciones como mejor te parezca.

### Opciones de Etiqueta <a href="#modulosdeadministracion-opcionesdeetiqueta" id="modulosdeadministracion-opcionesdeetiqueta"></a>

Asegúrate de traducir todos los campos de texto en todos los idiomas disponibles en tu tienda.

* **Etiqueta plazo de entrega (productos disponibles)**. Indica el plazo de de entrega estimado para tus productos en stock. Deja el campo vacío para deshabilitar la opción. El texto predeterminado es "Entrega: 1 a 3 semanas".
* **Etiqueta plazo de entrega (productos fuera de stock)**. Indica el plazo de de entrega estimado para tus productos fuera de stock. Deja el campo vacío para deshabilitar la opción. El texto predeterminado es "Entrega: 3 a 6 semanas".
* **Etiqueta Impuestos 'incl./excl.'**. Esta opción muestra si el impuesto está incluido en la página del producto (etiqueta "Impuestos incl. / excl.").&#x20;
* **Etiqueta 'Gastos de envío: impuestos excl.'**. Muestra si las tarifas de envío están incluidas, al lado del precio del producto ('Gastos de envío incluidos / excluidos').\
  Una vez habilitada, asegúrate de que la opción "Envío y pago" esté asociada a una página de CMS en la sección "Cumplimiento normativo legal", disponible más abajo en la pantalla de configuración. La etiqueta enlazará a este contenido.
* **Etiqueta de peso del producto**. Muestra el peso de un producto (cuando la información está disponible y el producto pesa más de 1 kg).
* **Precisión del peso del producto**. Te ayuda a seleccionar el nivel de precisión para la visualización del peso del producto (por ejemplo, 1 kg / 1,01 kg). El valor no puede ser negativo.
* **Términos de revocación dentro de la página ToS - Términos de Servicio (Terms of Service)**. Esta opción incluirá el contenido de los términos de revocación dentro de la página estática de Términos del Servicio (Terms of Service)..\
  Una vez habilitada, asegúrate de que la opción "Términos de revocación" esté asociada a una página de CMS en la sección "Cumplimiento normativo legal", disponible más abajo en la pantalla de configuración. La etiqueta enlazará a este contenido.
* **Revocación para productos virtuales**. Esta opción añade una casilla de verificación obligatoria al final del proceso de pago cuando el carrito contiene un producto virtual (ya sea un servicio o un bien digital). Utilízala para asegurarte de que el cliente es consciente de que pierde su derecho a cancelar una vez que la descarga de bienes digitales ha comenzado o una vez que el servicio se ha completado.
* &#x20;**Etiqueta precio 'Desde'**. Si un producto tiene combinaciones con diferentes precios, esta opción añade una etiqueta "Desde", antes del precio del producto en los listados de productos.
* **Texto arriba del carrito de compras**. Añade un texto personalizado encima del resumen del carrito de compras.
* **Texto bajo el carrito de compras**. Añade un texto personalizado que aparece bajo el resumen del carrito de compras..&#x20;

### Características <a href="#modulosdeadministracion-caracteristicas" id="modulosdeadministracion-caracteristicas"></a>

* **Activar característica 'Enviar a un amigo'**. Si está activada, el módulo "Enviar a un amigo" permite a los clientes enviar a un amigo un correo electrónico con un enlace a la página de un producto.\
  Esta opción asegura que cumples con la legislación local antes de habilitarla: los correos electrónicos enviados por esta característica se pueden considerar como correos electrónicos comerciales no solicitados.
* **Activar característica 'Reordenar'**. Esta opción permite a los clientes reordenar (volver a comprar un producto), realizando un simple clic desde su Historial de pedidos.\
  Desactiva esta opción si esta acción se considera como mercancías no solicitadas en tu legislación local.
* **Activar "Página del proceso de pago avanzada"**. Reemplaza el proceso estándar de pago con un cumplimiento más legal (basado en Europa, por supuesto). Esta opción solo funciona con la plantilla predeterminada de bootstrap u otras plantillas compatibles y con métodos de pago compatibles (muchos módulos ya han sido adaptados).\
  Una vez habilitada esta opción, la página del proceso pago avanzado muestra las siguientes secciones: métodos de pago, resumen de la dirección, aceptación de los Términos de Servicio (ToS), resumen del carrito y un botón "Pedido con obligación de pago".
* **Impuesto proporcional para el envío y embalaje**.  Cuando se activa esta opción, el impuesto para los gastos de envío y el embalaje se calcularán en proporción a los impuestos que se aplican a los productos incluidos en el carrito. Esto te permite definir un impuesto fijo, incluyendo los gastos de envío para cada transportista, mientras que la tasa de impuesto se calcula a partir de los impuestos del carrito promedio. Esta opción sustituye el comportamiento predeterminado en el que se define un gasto de envío excluido de impuestos, y lo sustituye por una regla de impuesto de envío fijo.\
  Cuando esté activado, asegúrate de que los gastos de envío los has establecido con impuestos incluidos

### Gestionar el contenido legal <a href="#modulosdeadministracion-gestionarelcontenidolegal" id="modulosdeadministracion-gestionarelcontenidolegal"></a>

Varias opciones de este módulo necesitan que el sistema "conozca" para qué se utilizan algunas de las páginas CMS. Si no existe una página disponible para asociarla con alguna de estas opciones, tendrás que crearla.

### Inclusión del contenido del correo electrónico  <a href="#modulosdeadministracion-inclusiondelcontenidodelcorreoelectronico" id="modulosdeadministracion-inclusiondelcontenidodelcorreoelectronico"></a>

Con esta interfaz, puedes elegir qué documentos debes incluir en la parte inferior de cualquiera de los correos electrónicos estándar enviados por la tienda; por ejemplo, el contenido textual de tu tienda puede incluirse en la parte inferior de todas las facturas enviadas.

El contenido se elige desde la sección de configuración "Gestionar contenido legal" de este módulo. Si ninguna opción está establecida, entonces no puedes seleccionar un contenido para enviar.

## Gestor de tareas Cron <a href="#modulosdeadministracion-gestordetareascron" id="modulosdeadministracion-gestordetareascron"></a>

Este módulo te proporciona una herramienta cron: puedes crear trabajos o tareas que  llamen a un determinado conjunto de direcciones URL seguras para tu tienda Prestashop, desencadenando así actualizaciones y otras tareas automatizadas.

## Boletín de noticias <a href="#modulosdeadministracion-boletindenoticias" id="modulosdeadministracion-boletindenoticias"></a>

Este módulo fue realizado para que puedas exportar un archivo CSV con las direcciones de correo electrónico de los clientes que se han registrado en tu tienda.

Tus clientes pueden darte sus direcciones de correo electrónico, ya sea introduciendo ésta en el bloque Newsletter localizado en la página de inicio, o bien marcando la casilla "Sí" para suscribirse al boletín de noticias cuando se registran en tu tienda. Necesitarás estas direcciones de correo electrónico para realizar funciones y actividades de marketing. Haz clic en "Configurar" para acceder a la página de configuración de este módulo.\
Tras el registro, tus clientes tienen dos opciones relacionadas con el boletín de noticias: La primera es suscribirse al boletín de noticias, la segunda recibir ofertas de tus asociados (si dicha opción fue seleccionada).

### Exportar suscriptores del Boletín de noticias <a href="#modulosdeadministracion-exportarsuscriptoresdelboletindenoticias" id="modulosdeadministracion-exportarsuscriptoresdelboletindenoticias"></a>

La primera sección te permite recoger todas las direcciones de correo electrónico registradas por el bloque de noticias de la página principal, haciendo clic en el botón "Exportar un fichero .CSV". Aparecerá una notificación, que te pedirá que hagas clic en un enlace para descargar el archivo que contiene las direcciones.

La información de este archivo se presenta en cuatro partes. El ID de cliente, la dirección de correo electrónico, el día de la inscripción, y la dirección IP. Si utilizas estos datos con un software como Microsoft Excel, puedes ordenar la información como desees.

### Exportar clientes <a href="#modulosdeadministracion-exportarclientes" id="modulosdeadministracion-exportarclientes"></a>

La segunda sección, denominada "Exportar clientes", te permite filtrar las direcciones de correo electrónico de tus clientes. A continuación, puedes filtrar los clientes, por sus países de origen seleccionando la opción "País del cliente" en el menú desplegable, y seleccionando posteriormente el país que quieras. El filtrado por países, es particularmente útil para el envío de boletines de noticias en el idioma del país seleccionado y para adaptar tus ofertas.

Puedes utilizar más filtros para exportar las direcciones de correo electrónico de tus clientes. Utiliza el campo "Suscritos al boletín de noticias", para seleccionar una de las tres siguientes opciones:

* **Todos los clientes**. Te permite seleccionar todas las direcciones de correo electrónico de los clientes que se han registrado en tu tienda. Es decir, tanto aquellos clientes que quieran recibir información por tu parte, como aquellos que no lo desean. Teniendo en cuenta este detalle, debes tener cuidado con el uso que hagas posteriormente con estos datos.
* **Suscritos**.Te permite seleccionar sólo a aquellos clientes que quieran recibir tu boletín de noticias.
* **No suscritos**. Te permite seleccionar sólo a aquellos clientes que no desean recibir tu boletín de noticias.

En el siguiente campo "Inscritos a publicidades", es donde puedes filtrar las direcciones de contacto, realizando un filtrado según la opción seleccionada por tus clientes a la hora de recibir ofertas de tus asociados. Al igual que en el campo anterior, tres opciones están disponibles:

* **Todos los clientes**. Te permite seleccionar todas las direcciones de correo electrónico de los clientes que se han registrado en tu tienda. Es decir, tanto aquellos clientes que quieran recibir información de sus asociados, como aquellos que no lo desean.
* **Suscritos**. Te permite seleccionar sólo a aquellos clientes que quieran recibir el boletín de tus asociados.
* **No suscritos**. Tepermite seleccionar sólo a aquellos clientes que no desean recibir el boletín de noticias de tus asociados.

Una vez que hayas filtrado las direcciones de correo electrónico para exportar, haz clic en "Exportar un fichero .CSV" para obtener todas las direcciones. Al igual que antes, una notificación en color verde te pedirá que hagas clic en un enlace para descargar el archivo. Este archivo contiene seis tipos de información: El ID de cliente, los apellidos del cliente, el nombre del cliente, la dirección de correo electrónico, el día de la inscripción, y la dirección IP. Toda esta información puede ser utilizada para enviar tus campañas de marketing.

## Limpiador de Prestashop <a href="#modulosdeadministracion-limpiadordeprestashop" id="modulosdeadministracion-limpiadordeprestashop"></a>

Este módulo te será de mucha utilidad cuando hayas terminado de explorar PrestaShop por primera vez, y te encuentres preparado para comenzar a añadir tu propio contenido: antes de nada deberás eliminar todos los datos de ejemplo no reales, que vienen incluidos al instalar Prestashop: productos, categorías, cliente, pedidos, etc.

La página de configuración consta de tres secciones:

* **Catálogo.** Esta acción eliminará todos los datos de tu catálogo actual, incluso los artículos que tu mismo hayas añadido. Haz clic en la opción "Sí", y a continuación. presiona el botón "Eliminar catálogo"  para iniciar el proceso.
* **Pedidos y clientes**. Esta acción eliminará todos los pedidos y clientes registrados actualmente, incluso los que tu mismo hayas añadido. Haz clic en la opción "Sí", y a continuación, presiona el botón "Eliminar pedidos y clientes" para iniciar el proceso.  **** &#x20;
* &#x20;**Limitaciones de la integridad funcional.** Esta acción comprobará tu base de datos y se asegurará de que todo está configurado correctamente, tratando de corregir lo que no lo esté. &#x20;
* **Limpieza de la base de datos**. Esto ayudará a reducir el espacio de almacenamiento y mejorará la eficiencia de acceso a disco.

**Ten mucho cuidado**: cualquier acción desencadenada por hacer clic en uno de estos botones es irreversible. Asegúrate de realizar una copia de seguridad de tu base de datos antes de utilizar algunos de estos botones.

## Alertas por correo <a href="#modulosdeadministracion-alertasporcorreo" id="modulosdeadministracion-alertasporcorreo"></a>

PrestaShop te permite recibir alertas por correo electrónico, y enviar notificaciones a tus clientes, en ciertas situaciones:

* A tus clientes: cuando un producto está fuera de stock.
* A ti: cuando un nuevo pedido se haya producido en tu tienda.
* A ti: cuando las unidades disponibles en stock de un producto se encuentran por debajo del umbral.
* A ti: cuando la cobertura de un producto está por debajo de un cierto número de días.

### Notificaciones de cliente <a href="#modulosdeadministracion-notificacionesdecliente" id="modulosdeadministracion-notificacionesdecliente"></a>

Sólo hay un ajuste de configuración en esta sección:

* **Disponibilidad del producto**. Cuando se habilita esta configuración, un campo aparecerá en la página del producto de tu tienda cuando éste se encuentre fuera de stock. Se invitará a tus clientes a que dejen sus datos de contacto para que puedan ser contactados cuando vuelvan a estar disponibles unidades de este producto para su venta.

### Notificaciones del comerciante <a href="#modulosdeadministracion-notificacionesdelcomerciante" id="modulosdeadministracion-notificacionesdelcomerciante"></a>

Hay varias opciones de configuración para las notificaciones a comerciantes:

* **Nuevo pedido**. Activa esta opción si deseas recibir una notificación cada vez que se produzca un nuevo pedido.&#x20;
* **Fuera de stock**. Activa esta opción y establece el campo "Umbral" con el valor en el que deseas ser alertado (de manera predeterminada es 3).
* **Advertencia de cobertura**. Activa esta opción y establece el campo "Cobertura" con el valor en el que deseas ser alertado (de manera predeterminada es 0).

Las Notificaciones del comerciante pueden ser enviadas a varias direcciones al mismo tiempo. Para ello, escriba en la opción denominada "Direcciones de e-mail", cada dirección de correo electrónico que recibirá la notificación (una dirección de correo electrónico por línea). Para desplazarse a la línea siguiente, pulse la tecla Enter de su teclado).

## Google Analytics API <a href="#modulosdeadministracion-googleanalyticsapi" id="modulosdeadministracion-googleanalyticsapi"></a>

Este módulo te permite vincular tu tienda PrestaShop con tu cuenta de Google Analytics.

En primer lugar, deberás elegir la versión de la API que deseas utilizar:

* La versión 1.3 requerirá que introduzcas los datos e-mail, contraseña y Perfil ID de tu cuenta en Google Analytics.
* La versión 3.0 requerirá que introduzcas los datos Client ID, Client Secret y Perfil ID de tu cuenta en Google Analytics.

Te recomendamos que utilice la versión 3.0, ya que la versión 1.3 se considera obsoleta y menos segura. Para poder trabajar con la versión 3.0, debes autorizar el acceso para OAuth siguiendo las siguientes instrucciones: [https://developers.google.com/analytics/devguides/config/mgmt/v3/mgmtAuthorization](https://developers.google.com/analytics/devguides/config/mgmt/v3/mgmtAuthorization)

## Marca de agua (filigrana) <a href="#modulosdeadministracion-marcadeagua-filigrana" id="modulosdeadministracion-marcadeagua-filigrana"></a>

Este módulo te permite añadir una marca de agua a las imágenes de tu tienda. Esta limita la circulación de tus imágenes en Internet. – y es de esperar que disuada a otros webmasters aprovecharse de ellas.

Si tienes la intención de exportar tus productos en Google Shopping, debes saber que en este servicio, no está permitido el uso de textos promocionales / logotipos y marcas de agua en las imágenes. Así que sólo podrás utilizar imágenes que no tengan una marca de agua o logo añadido.\
Puedes obtener toda la información sobre las políticas de Google Shopping en el siguiente enlace: [https://support.google.com/merchants/answer/2700371?hl=es\&ref\_topic=2701481](https://support.google.com/merchants/answer/2700371?hl=es\&ref\_topic=2701481)

La página de configuración te notifica de inmediato qué ajustes faltan por establecer.

* **Archivo de la filigrana (marca de agua)**. La imagen elegida debe estar en formato GIF.
* **Transparencia de la filigrana / marca de agua (0-100)**. 100 equivale a una imagen no transparente, lo que significa que tu logo será muy visible, y ocultará por completo la parte de la imagen donde éste se situé. El valor predeterminado, 60, es generalmente una buena elección.
* **Alineación X de la filigrana / marca de agua**. Selecciona dónde debe aparecer la marca de agua en cada una de tus imágenes. Este campo se refiere al eje horizontal.
* **Alineación Y de la filigrana / marca de agua**. Selecciona dónde debe aparecer la marca de agua en cada una de tus imágenes. Este campo se refiere al eje vertical.
* **Elija el tipo de imagen para proteger la filigrana / marca de agua**. El tipo de imágenes a las que se debe aplicar la marca de agua. Quizás sólo debas seleccionar las imágenes de mayor tamaño, ya que estas son las más propensas a ser robadas.

Una vez que hayas guardado tus ajustes, habrá finalizado la configuración de este módulo, pero comprobarás que las marcas de agua aún no han sido añadidas a las imágenes de tu tienda. Dirígete al menú "Preferencias", y abre la página "Imágenes". Haz clic en el botón "Regenerar miniaturas", situado en la parte inferior de la página. PrestaShop procesará todas tus imágenes (seleccionadas en la configuración), y tu marca de agua aparecerá en las imágenes que hayas seleccionado.

## Experiencia Comercial <a href="#modulosdeadministracion-experienciacomercial" id="modulosdeadministracion-experienciacomercial"></a>

Este módulo ha sido diseñado específicamente para ayudar a los usuarios de PrestaShop a realizar un seguimiento de su progreso como comerciantes, y comprobar cuánto ha ido creciendo y progresando en los días, meses y años desde que inició su tienda. Este módulo se encuentra instalado por defecto.

Para conseguir este objetivo hemos creado un sistema de medallas y puntos para monitorizar fácilmente tu progreso como minorista. Hemos desgranado el sistema en tres niveles, todos los cuales están integrados para triunfar en el mundo del e-commerce:

* **Funcionalidades**. Tu uso de las funcionalidades clave del comercio electrónico, tales como: Rendimiento del sitio, Tamaño del catálogo, Empleados y SEO.
* **Logros**. Tu cumplimiento de los objetivos específicos claves del comercio electrónico, como el Número de clientes, Pedidos, e Ingresos.
* **Internacional**. Seguimiento de tu presencia en mercados internacionales clave, tales como las Américas, Oceanía, Asia, Europa, África y El Magreb.

Cuanto más progrese tu tienda, más insignias y puntos obntendrás.\
No hay necesidad de entregar esta información, ni de rellenar ningún formulario. Sabemos lo ocupado que estás; así que todo se realiza automáticamente. Utiliza esta herramienta para impulsar tu negocio, ver tu progreso y reflexionar sobre tus grandes logros conseguidos.

## Diagramas NVD3 <a href="#modulosdeadministracion-diagramasnvd3" id="modulosdeadministracion-diagramasnvd3"></a>

NVD3 ([http://nvd3.org/](http://nvd3.org/)) es una librería Javascript que ha sido desarrollada específicamente para generar bellas gráficas utilizando D3.js ([http://d3js.org/](http://d3js.org/)), una librería JavaScript desarrollada para manipular documentos basados en datos.

Este módulo te permite utilizar el código de gráficas NVD3 para tu propio uso, proporcionándote útiles gráficas de datos.

## Primeros pasos <a href="#modulosdeadministracion-primerospasos" id="modulosdeadministracion-primerospasos"></a>

El módulo Primeros pasos, es el encargado de dar la bienvenida a los usuarios que utilizan por primera vez al back-office de PrestaShop: a través de una pequeña interfaz lúdica, se muestra al usuario cómo lanzar su tienda en pequeños y fáciles pasos.

## Mostrar HTML simple <a href="#modulosdeadministracion-mostrarhtmlsimple" id="modulosdeadministracion-mostrarhtmlsimple"></a>

Permite al sistema de estadísticas mostrar los datos en una cuadrícula o rejilla.
