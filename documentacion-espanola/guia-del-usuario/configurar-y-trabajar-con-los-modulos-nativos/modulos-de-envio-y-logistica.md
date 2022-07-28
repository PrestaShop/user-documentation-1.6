# Módulos de Envío y Logística

## Estimación de los gastos de envío <a href="#modulosdeenvioylogistica-estimaciondelosgastosdeenvio" id="modulosdeenvioylogistica-estimaciondelosgastosdeenvio"></a>

Este módulo permite al cliente comparar las tarifas de envío de los distintos transportistas  antes de continuar con el proceso de compra.

Este módulo es muy sencillo: sólo tienes que instalarlo para mostrar esta opción en el front-office de tu tienda.

Debes haber establecido todas las tarifas de envío de los distintos transportistas disponibles en tu tienda. Este proceso se realiza en la página "Transportistas", donde deberás indicar los costes y rangos para todas las zonas geográficas donde realices envíos.

La página de configuración del módulo sólo tiene una opción , "¿Cómo actualizar la lista de transportistas?". Esta opción te permite mostrar un transportista solamente cuando toda la información está establecida, o en cualquier momento.

## Estimación de la entrega <a href="#modulosdeenvioylogistica-estimaciondelaentrega" id="modulosdeenvioylogistica-estimaciondelaentrega"></a>

Este módulo muestra una fecha aproximada de entrega durante el proceso de compra.

La página de configuración tiene dos secciones:

* **Configuración del transportista**. El módulo se basa en las indicaciones de tus transportistas. Por tanto, debes añadir las reglas para cada uno de sus transportistas, haciendo clic en el enlace "Añadir una nueva regla de transportista".
* **Ajustes**:
  * **Tiempo suplementario cuando un producto no está disponible**. Calcula el tiempo que podría tomar a tu equipo reponer el stock de los productos. Esto sólo es útil si el cliente quiere pedir productos que no están disponibles (la opción para esto se encuentra en la página de preferencias "Productos", en la sección "Stock de productos").
  * **Tiempo suplementario para la preparación del pedido**. Calcula el tiempo que podría tomar a tu equipo preparar un pedido.
  * **Opción para la preparación**. Si tu equipo también trabaja y envía productos los fines de semana, indícalo, ya que el módulo tiene esto en cuenta.
  * **Formato de la fecha**. El formato en que se muestra la fecha probable de entrega. Esta utiliza el formato de la función de PHP `date()` cada letra tiene un significado, como se explica en el enlace indicado. El parámetro predeterminado, "l j F Y", significa que la fecha se mostrará en el formato "Sábado, 21 de enero de 2012". Hay muchos otros carácteres que puedes utilizar para establecer el formato de fecha como mejor te parezca: véase [http://php.net/manual/es/function.date.php](http://php.net/manual/es/function.date.php).

Añadir una nueva regla de transportista es bastante sencillo:

* **Transportista**. Selecciona el transportista para el que deseas añadir la regla. Si el transportista deseado no se encuentra en la lista, deberás crearlo primero desde la página Transporte > Transportistas.
* **Entrega prevista entre**. Establece el marco de tiempo en el que el transportista elegido se compromete a entregar los productos. Tienes que obtener esta información del propio transportista.
* **Opciones de entrega**. Algunas empresas de transporte también realizan entregas los fines de semana. Asegúrate de indicarlo de ser así.

Debes crear tantas reglas de transporte como sea necesario.

## Fedex (fedexcarrier) <a href="#modulosdeenvioylogistica-fedex-fedexcarrier" id="modulosdeenvioylogistica-fedex-fedexcarrier"></a>

Ofrece a tus clientes, los diferentes métodos de entrega disponibles con Fedex.

## Globkurier <a href="#modulosdeenvioylogistica-globkurier" id="modulosdeenvioylogistica-globkurier"></a>

**Disponible solamente en Polonia.**

![](<../../../.gitbook/assets/23036725 (1).png>)

[GlobKurier.pl](http://globkurier.pl) es uno de los líderes nacionales en la entrega de los envíos. Proporcionamos servicios nacionales e internacionales a más de 200 países. Nuestras principales ventajas son los precios competitivos, velocidad y seguridad. Con [GlobKurier.pl](http://globkurier.pl) puedes estar seguro de que tus envíos siempre llegan a tiempo.

## GoInterpay <a href="#modulosdeenvioylogistica-gointerpay" id="modulosdeenvioylogistica-gointerpay"></a>

![](<../../../.gitbook/assets/23038228 (1).png>)

Dispón de más de 200 métodos de pago y envío con  una sencilla integración.

## Kiala Advanced (Sólo titulares de contratos Kiala) <a href="#modulosdeenvioylogistica-kialaadvanced-solotitularesdecontratoskiala" id="modulosdeenvioylogistica-kialaadvanced-solotitularesdecontratoskiala"></a>

El módulo de Kiala te permite proponer una opción de entrega de paquetes en un punto de recogida Kiala como una alternativa a la entrega domiciliaria. Los puntos de entrega Kiala están ampliamente disponibles en Francia, y también en otros países europeos.

Debes tener una cuenta en Kiala para poder utilizar este módulo. Puedes llegar al formulario de inscripción desde el siguiente enlace: [http://www.kiala.com/](http://www.kiala.com/).\
A continuación, configura el módulo con tu información personal y de tu tienda en el formulario de la sección "Estado del módulo Kiala".\
&#x20;La sección "Ajustes de país" te permite indicar en qué países deseas que la entrega Kiala esté disponible para tus clientes.\
&#x20;Por último, la sección "Kiala opciones avanzadas", añade algunas opciones más:

* **Carpeta de exportación**. La carpeta local en el que el módulo guardará tu exportación, que contiene una gran cantidad de información útil.
* **Prefijo para el pedido y número de paquete**. Puedes tener un prefijo específico para tu tienda, lo que hace que esto se vea más personalizado de cara a tus clientes.
* **¿Exportar en cada pedido?**. Puedes preferir tener varios archivos de exportación específicos del pedido en lugar de uno grande.
* **¿Criterio de seguimiento del paquete?**. ¿El paquete debe ser seguido en función del cliente o en función del pedido? Si no estás seguro, mantén el valor "por pedido".

Una vez que la configuración ha sido establecida, tus clientes podrán ver que la opción "Kiala" aparece en el front-office de la tienda como parte de los métodos de entrega disponibles.

## Mondial Relay <a href="#modulosdeenvioylogistica-mondialrelay" id="modulosdeenvioylogistica-mondialrelay"></a>

Este módulo te permite mostrar los precios para la entrega en los puntos Mondial Relay. Este servicio está disponible en Francia, Luxemburgo, España y Bélgica.

Debes tener una cuenta en Mondial Relay para poder utilizar este servicio. Puedes llegar al formulario de inscripción desde el siguiente enlace: [http://www.mondialrelay.com/](http://www.mondialrelay.com/).\
A continuación, configura el módulo, haz clic en el icono "Detalles de la cuenta" e introduce la información necesaria, proporcionada por Mondial Relay: Webservice Enseigne, Code marque (Código de marca), Webservice Key (Clave del webservice), Etiquette's Language (Idioma de etiqueta) y Weight Coefficient (Coeficiente de peso). El Idioma de etiqueta (Etiquette's Language), sólo puede utilizar los idiomas que están activados en tu tienda; puedes activar más idiomas desde la página "Idiomas", bajo el menú "Localización". Haz clic en "Actualizar ajustes" para conecta tu tienda al servicio web Mondial Relay, y a partir de aquí, sigue las instrucciones del módulo que aparecen en las pantallas "Envío" y "Ajustes avanzados".

Una vez que la configuración ha sido establecida, tus clientes podrán ver que la opción "Mondial Relay" aparece en el front-office de la tienda como parte de los métodos de entrega disponibles.

## So Colissimo <a href="#modulosdeenvioylogistica-socolissimo" id="modulosdeenvioylogistica-socolissimo"></a>

Este módulo te permite mostrar tarifas para las entregas a través de SoColissimo, un servicio de La Poste, el servicio postal histórico de Francia. Este servicio está disponible principalmente en Francia.

Debes tener una cuenta en SoColissimo para poder utilizar este módulo. Puedes obtener una cuenta llamando a La Poste desde un teléfono francés, utilizando este número: **3634**.\
A continuación, configura el módulo con tu información SoColissimo: ID So, key (clave de cifrado), preparation time (tiempo de preparación), overcost (sobrecoste), URL So, Fancybox, Supervision y Supervision URL.\
La documentación completa está disponible (en francés) en formato PDF, bajo el enlace "Documentación" en la página de configuración de este módulo.

Para finalizar la instalación, copia / pega las dos URL finales en tu back-office de SoColissimo.

Una vez que la configuración ha sido establecida, tus clientes podrán ver que la opción "SoColissimo" aparece en el front-office de la tienda como parte de los métodos de entrega disponibles.

## TNT Express France <a href="#modulosdeenvioylogistica-tntexpressfrance" id="modulosdeenvioylogistica-tntexpressfrance"></a>

**Disponible solamente en Francia.**

Este módulo te permite mostrar tarifas para las entregas a través del servicio de correo urgente TNT. Este servicio está disponible en todo el mundo.

Debes tener una cuenta en TNT para poder utilizar este módulo. Puedes llegar al formulario de inscripción desde el siguiente enlace: [http://www.tnt.com](http://www.tnt.com).\
&#x20;A continuación, configura el módulo con tu Id en TNT, tu contraseña y tu número de cuenta, desde la pestaña "Configuración de la cuenta".\
A partir de aquí, continúa la configuración del módulo utilizando las pestaña  "Ajustes de envío" y "Configuración del servicio". Esta última pestaña te permite especificar detalladamente el  servicio de entrega que deseas que esté disponible para tus clientes, así como cualquier cargo adicional que puedas necesitar en función del peso del paquete.

Una vez que la configuración ha sido establecida, tus clientes podrán ver que la opción "TNT Express France" aparece en el front-office de la tienda como parte de los métodos de entrega disponibles.

## Tracking - Front office <a href="#modulosdeenvioylogistica-tracking-frontoffice" id="modulosdeenvioylogistica-tracking-frontoffice"></a>

Este módulo completa PrestaShop con una función de programa de afiliados integrado, que permite a los afiliados acceder a sus propias estadísticas.

La herramienta de programa de afiliados se encuentra en la página "Programa de afiliados", bajo el menú "Estadísticas". Una vez que hayas instalado el módulo "Tracking - Front office", estos afiliados pueden acceder a sus estadísticas, dirigiéndose al enlace: [http://www.ejemplo.com/modules/trackingfront/stats.php](http://www.example.com/modules/trackingfront/stats.php).

Para crear un nuevo afiliado, haz clic en el botón "Añadir nuevo", y en el formulario de creación, añade el nombre de usuario y la contraseña del afiliado, a continuación, especifica la cuota que recibes por clic, por pedido y por porcentaje de ventas.

Haz clic en el encabezado de la sección "Ayuda" para ver instrucciones sobre cómo configurar las direcciones URL referenciales.

La "Información técnica - Modo Experto" te permite utilizar expresiones regulares en lugar de URLs de texto sin formato.

## UPS <a href="#modulosdeenvioylogistica-ups" id="modulosdeenvioylogistica-ups"></a>

Ofrece a tus clientes, los diferentes métodos de entrega disponibles con UPS .

## USPS <a href="#modulosdeenvioylogistica-usps" id="modulosdeenvioylogistica-usps"></a>

Calcula las tarifas de envío del Servicio Postal de los Estados Unidos para el envío nacional dentro de los EE.UU.
