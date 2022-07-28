# Facturas

Cada vez que un pedido de tu tienda es validado, una factura se envía al cliente. Puedes descargar las facturas de un solo pedido de la página del pedido. La página "Facturas" bajo el menú "Pedidos" te permite descargar una selección de facturas de pedidos anteriores en formato PDF, todas al mismo tiempo (en el mismo archivo PDF).

![](../../../.gitbook/assets/54268294.png)

Puedes obtener un archivo PDF conteniendo varias facturas en función de dos criterios principales:

* **Por fecha**. Muy útil cuando necesites imprimir todas las facturas de un mes o un trimestre determinado. Selecciona la fecha de inicio y fin, y haz clic en el botón "Generar PDF por fecha".
* **Por estado de pedido**. Indispensable cuando necesites imprimir con precisión pedidos que han sido cancelados, reembolsados o se encuentran pendientes. PrestaShop te indica el número de facturas vinculadas a cada estado entre paréntesis.

En ambos casos, las facturas se generan en un solo archivo PDF, cada uno con sus propias páginas. No se puede obtener un único archivo PDF para cada factura del período o estados determinados utilizando esta página.

Si deseas personalizar el aspecto de las facturas de tu tienda, debes cambiar sus archivos de plantilla.

Los archivos de la plantilla PDF se encuentran en la carpeta `/pdf`. Abre el archivo `invoice.tpl` y edítalo a tu gusto: éste es un archivo HTML con etiquetas Smarty.

## Opciones de factura <a href="#facturas-opcionesdefactura" id="facturas-opcionesdefactura"></a>

Puedes elegir si deseas o no poner las facturas a disposición de tus clientes tan pronto como se haga el pedido, así como el prefijo para todas las facturas y el número de factura que deseas que aparezca en la versión impresa de la factura. Esta función puede ayudarte a simplificar la gestión de tu cuenta.

![](../../../.gitbook/assets/54268297.png)

* **Activar las facturas**. Si deshabilitas esta opción, tu cliente no recibirá una factura después de su compra. Tendrás que encargarte tu personalmente de enviar la factura, si algún cliente te la solicita.
* **Activar el desglose de impuestos en la factura**. _Novedad en Prestashop 1.6_. Cuando se habilita esta opción, la factura lista todas las diferentes tasas de impuestos que fueron aplicadas al pedido, en lugar de tan sólo mostrar un porcentaje.
* **Activar imagen del producto**. _Novedad en PrestaShop 1.6.1._ Cuando se activa esta opción, se añadirá la imagen del producto junto al nombre del producto en la factura.\

* **Prefijo de las facturas**. De manera predeterminada, PrestaShop utiliza prefijos adaptados a cada idioma para tus facturas: "IN" en Inglés, "FA" en francés (de "factura"), "CU" en español (por "cuenta"), etc. Es posible que prefieras utilizar prefijos para cada idioma: "EN", "FR", "SP", etc. Por supuesto, también puedes optar por tener un prefijo único para cada idioma, o no utilizar ningún prefijo para ninguna de ellas.\
  &#x20;PrestaShop generará entonces los números de las facturas de acuerdo a tu configuración establecida: "# IN000001", "# FR000002", etc.
* **Número de factura**. Si tu empresa ya tiene pedidos y facturas antes de empezar a utilizar PrestaShop, puedes utilizar esta opción para iniciar tu sistema de facturación en un determinado número.
* **Texto legal libre**. _Novedad en PrestaShop 1.6.1.0_. Este campo te permite añadir contenido adicional a la factura, para casos en que la legislación local requiera que muestre información adicional. En la factura, aparecerá debajo del resumen de los métodos de pago. Por supuesto, puedes utilizar este texto libre para presentar cualquier texto que consideres necesario.
* **Texto en pie de página**. Puedes utilizar esta opción para tener un texto personalizado en la parte inferior de todas las facturas. El texto aparecerá en la factura debajo del nombre de la tienda.
* **Modelo de factura**. En función del tema, es posible que puedas utilizar más de un estilo de factura. Prueba esta opción con un pedido falso para elegir la que más te guste. Si sabes cómo codificar en HTML, puedes añadir tus propios modelos de factura o editar los ya existentes: éstas se encuentran en la carpeta `/pdf/` de tu instalación de PrestaShop.
* **Utilizar el disco como caché para facturas PDF**. Puedes optar por almacenar las facturas generadas en el disco del servidor en lugar de en la memoria caché del servidor. Esto preserva la memoria, pero enlentece la generación de archivos PDF. Utiliza esta opción con conocimiento de causa.

No olvides guardar los cambios realizados.

Cuando los clientes te piden sus facturas, puedes redirigirlos a la sección "Historial de pedidos" de sus cuentas de usuario, donde se incluyen todas sus facturas disponibles.
