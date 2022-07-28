# Ejemplos de usos del modo multitienda

/\*\<!\[CDATA\[\*/\
div.rbtoc1597066537013 {padding: 0px;}\
div.rbtoc1597066537013 ul {list-style: disc;margin-left: 0px;}\
div.rbtoc1597066537013 li {margin-left: 0px;padding-left: 0px;}\
\
/\*]]>\*/

* [Ejemplos de usos del modo multitienda](ejemplos-de-usos-del-modo-multitienda.md#Ejemplosdeusosdelmodomultitienda-Ejemplosdeusosdelmodomultitienda)
  * [Gestionar un catálogo en modo multitienda](ejemplos-de-usos-del-modo-multitienda.md#Ejemplosdeusosdelmodomultitienda-Gestionaruncatálogoenmodomultitienda)
  * [Intercambio de datos entre las tiendas](ejemplos-de-usos-del-modo-multitienda.md#Ejemplosdeusosdelmodomultitienda-Intercambiodedatosentrelastiendas)
    * [Duplicar datos entre tiendas](ejemplos-de-usos-del-modo-multitienda.md#Ejemplosdeusosdelmodomultitienda-Duplicardatosentretiendas)
    * [Compartir datos entre las tiendas y los grupos de tiendas](ejemplos-de-usos-del-modo-multitienda.md#Ejemplosdeusosdelmodomultitienda-Compartirdatosentrelastiendasylosgruposdetiendas)
    * [Compartir productos y categorías](ejemplos-de-usos-del-modo-multitienda.md#Ejemplosdeusosdelmodomultitienda-Compartirproductosycategorías)
    * [Compartir clientes y grupos de clientes](ejemplos-de-usos-del-modo-multitienda.md#Ejemplosdeusosdelmodomultitienda-Compartirclientesygruposdeclientes)
    * [Utilizar un tema diferente para cada tienda o grupo de tiendas](ejemplos-de-usos-del-modo-multitienda.md#Ejemplosdeusosdelmodomultitienda-Utilizaruntemadiferenteparacadatiendaogrupodetiendas)
    * [Utilizar configuraciones específicas para cada tienda o grupo de tiendas](ejemplos-de-usos-del-modo-multitienda.md#Ejemplosdeusosdelmodomultitienda-Utilizarconfiguracionesespecíficasparacadatiendaogrupodetiendas)
  * [Gestionar las páginas CMS en modo multitienda](ejemplos-de-usos-del-modo-multitienda.md#Ejemplosdeusosdelmodomultitienda-GestionarlaspáginasCMSenmodomultitienda)
  * [Gestionar descuentos en modo multitienda](ejemplos-de-usos-del-modo-multitienda.md#Ejemplosdeusosdelmodomultitienda-Gestionardescuentosenmodomultitienda)
  * [Multitienda y Webservice](ejemplos-de-usos-del-modo-multitienda.md#Ejemplosdeusosdelmodomultitienda-MultitiendayWebservice)

## Gestionar un catálogo en modo multitienda <a href="#ejemplosdeusosdelmodomultitienda-gestionaruncatalogoenmodomultitienda" id="ejemplosdeusosdelmodomultitienda-gestionaruncatalogoenmodomultitienda"></a>

En modo multitienda, algunas páginas de administración de PrestaShop presentan un menú desplegable, titulado "Configuración para multitienda". Este menú te permite seleccionar el contexto para la acción que estás realizando: lo que te permite establecer la tienda o grupo de tiendas a las que se aplicará el cambio.

Por ejemplo, al crear un nuevo producto, la selección que realices en este menú determinará si el producto estará disponible para todas las tiendas, sólo para un grupo de tiendas, o en una sola tienda.

Durante la edición de un producto, PrestaShop muestra notificaciones para ayudarte a entender el alcance de los cambios. Por ejemplo, al modificar un producto en el contexto "Tienda A", la notificación mostrará el siguiente mensaje: "¡Advertencia! Si cambias el valor de los campos con una viñeta naranja, el valor será cambiado en todas las tiendas en donde se encuentre este producto", mostrando dicha viñeta de color naranja en todos los campos implicados, tales como "Tipo de producto", "Referencia", tamaño del paquete, etc.

Del mismo modo, si cambias un producto en el contexto "Todas las tiendas" o en el contexto de un grupo de tiendas, algunos campos serán desactivados: dado que esto tienen un impacto global, no podrás editarlo. Si realmente necesitas editar este contenido, cada campo tiene una casilla que puedes marcar para editar esos campos en todas las tiendas que se encuentren bajo este contexto.

Si modificas un campo desactivado, el producto es creado en todas las tiendas del contexto que todavía no tengan a éste en su propio catálogo. Asegúrate de comprobar el contexto antes de realizar esta acción.

## Intercambio de datos entre las tiendas <a href="#ejemplosdeusosdelmodomultitienda-intercambiodedatosentrelastiendas" id="ejemplosdeusosdelmodomultitienda-intercambiodedatosentrelastiendas"></a>

### Duplicar datos entre tiendas <a href="#ejemplosdeusosdelmodomultitienda-duplicardatosentretiendas" id="ejemplosdeusosdelmodomultitienda-duplicardatosentretiendas"></a>

Los datos duplicados en PrestaShop son establecidos durante la instalación de cualquier tienda individual, importando todos o algunos de los contenidos de una tienda existente a otra nueva. El contenido que puede ser importado es variado: productos, categorías, empleados, módulos, reglas de carrito, proveedores, etc. La importación de datos se realiza de una vez por todas: una vez la tienda ha sido creada, no puedes volver a importar datos de otra tienda - al menos no tan fácilmente.

### Compartir datos entre las tiendas y los grupos de tiendas <a href="#ejemplosdeusosdelmodomultitienda-compartirdatosentrelastiendasylosgruposdetiendas" id="ejemplosdeusosdelmodomultitienda-compartirdatosentrelastiendasylosgruposdetiendas"></a>

Las tiendas pueden compartir datos. Los datos compartidos se gestionan fundamentalmente entre las tiendas a nivel de grupo: uno de los aspectos más importantes a comprender en el modo multitienda de PrestaShop es que todas las tiendas dentro del mismo grupo de tiendas pueden compartir sus datos – o más concretamente, tres tipos de contenidos: clientes, cantidades disponibles, y pedidos. Una vez que el grupo de tiendas está configurado, el intercambio de datos entre las tiendas finaliza: aunque puedes cambiar la configuración para las cantidades de productos disponibles, no puedes cambiar la configuración de los clientes y los pedidos a partir del momento en que una de las tiendas de este grupo tenga un cliente o un pedido.

### Compartir productos y categorías <a href="#ejemplosdeusosdelmodomultitienda-compartirproductosycategorias" id="ejemplosdeusosdelmodomultitienda-compartirproductosycategorias"></a>

Al crear una nueva tienda dentro de un grupo, puedes hacer que todas o algunas de las categorías en la nueva tienda sean copias exactas de las categorías de otra tienda instalada en PrestaShop.

Al crear una categoría, para una tienda específica o para todas las tiendas instaladas, PrestaShop registra la categoría para todas las tiendas – simplemente se oculta en cualquier tienda en la que ésta no haya sido establecida.

Al asociar las nuevas tiendas, con una categoría determinada, cualquier cambio en esta categoría tendrá un impacto en todas las tiendas que están asociadas con ella, incluso si las tiendas pertenecen a grupos de tiendas diferentes. Puedes cambiar el contenido de la categoría de una sola vez para todas las tiendas, incluyendo sus productos.

### Compartir clientes y grupos de clientes <a href="#ejemplosdeusosdelmodomultitienda-compartirclientesygruposdeclientes" id="ejemplosdeusosdelmodomultitienda-compartirclientesygruposdeclientes"></a>

Como se indicó anteriormente, las tiendas dentro de un mismo grupo de tiendas pueden compartir clientes: todo lo que tienes que hacer es establecer la opción adecuada al momento de crear el grupo de tiendas.

Los grupos son menos detallados: si cambias uno de los grupos de clientes de manera predeterminada en una tienda, el cambio se aplicará a todas las tiendas, cualesquiera que sean sus grupos de tiendas.

Si quieres tener diferentes grupos de clientes para cada tienda, debes crear un nuevo grupo y utilizar el selector "Configuración multitienda para" con el fin de asociar el grupo a una tienda o a un grupo de tiendas.

### Utilizar un tema diferente para cada tienda o grupo de tiendas <a href="#ejemplosdeusosdelmodomultitienda-utilizaruntemadiferenteparacadatiendaogrupodetiendas" id="ejemplosdeusosdelmodomultitienda-utilizaruntemadiferenteparacadatiendaogrupodetiendas"></a>

Para instalar un tema en PrestaShop, debes utilizar el módulo "Importar / Exportar tema" e importar el archivo Zip perteneciente al tema. Una vez este archivo haya sido cargado, el módulo te hará algunas preguntas. En el modo multitienda, este también te preguntará si deseas activar el tema en todas las tiendas instaladas en Prestashop, solamente para algunos grupos de tiendas, o tan sólo para algunas tiendas especificas - con las tiendas actuales ya seleccionadas. El tema seguirá estando disponible para las tiendas no seleccionadas, pero estará desactivado.

Esta configuración puede ser modificada: una vez que el tema esté instalado en Prestashop, puedes utilizar la página "Temas" del menú "Preferencias" para cambiar el tema de la tienda actual, o del grupo de tiendas actual, dependiendo de cómo esté establecido el selector "Configuración multitienda para".

### Utilizar configuraciones específicas para cada tienda o grupo de tiendas <a href="#ejemplosdeusosdelmodomultitienda-utilizarconfiguracionesespecificasparacadatiendaogrupodetiendas" id="ejemplosdeusosdelmodomultitienda-utilizarconfiguracionesespecificasparacadatiendaogrupodetiendas"></a>

El selector "Configuración multitienda para" es la opción a la que debes dirigirte cuando quieras que tus modificaciones tengan un impacto sobre una tienda determinada o un conjunto de tiendas. Incluso debería ser la primera opción que revises al cargar la pantalla de administración, ya que Prestashop cambiará las opciones disponibles dependiendo del contexto en el que te encuentres: tienda, grupo de tiendas o todas las tiendas.

Esto hace posible:

* Utilizar un formato de imagen diferente para cada tienda / grupo de tiendas.
* Activar / configurar un módulo en base a una tienda.
* Posicionar / mostrar bloques en el front-office en base a una tienda.
* ...¡y mucho más!.

## Gestionar las páginas CMS en modo multitienda <a href="#ejemplosdeusosdelmodomultitienda-gestionarlaspaginascmsenmodomultitienda" id="ejemplosdeusosdelmodomultitienda-gestionarlaspaginascmsenmodomultitienda"></a>

Al visualizar el listado de páginas CMS en el contexto "Todas las tiendas", se muestran todas las páginas CMS de todas las tiendas. Del mismo modo, cuando se está en un contexto de grupo de tiendas, se muestran las páginas para todas las tiendas de ese grupo.

Cuando se crea una página en un contexto de grupo de tiendas, todas las tiendas existentes en ese grupo se muestran en esta página, aunque la página sea única: al modificar ésta para una tienda se modificará en todas las tiendas de ese grupo.\
En la página de creación, una sección aparece con una lista, indicando cuáles de éstas se verán afectadas.

## Gestionar descuentos en modo multitienda <a href="#ejemplosdeusosdelmodomultitienda-gestionardescuentosenmodomultitienda" id="ejemplosdeusosdelmodomultitienda-gestionardescuentosenmodomultitienda"></a>

Al crear reglas de carrito o reglas del catálogo en un contexto multitienda, una condición adicional estará disponible, con la que puedes elegir las tiendas en las que este descuento estará disponible.

## Multitienda y Webservice <a href="#ejemplosdeusosdelmodomultitienda-multitiendaywebservice" id="ejemplosdeusosdelmodomultitienda-multitiendaywebservice"></a>

El acceso al webservice también es altamente configurable, tanto a nivel de tienda como a nivel de grupo de tiendas. Al crear una clave de servicios web, puedes elegir asociar éste a todas las tiendas, a algunos grupos de tiendas, o a tiendas individuales.
