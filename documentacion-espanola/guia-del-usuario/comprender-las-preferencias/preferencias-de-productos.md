# Preferencias de Productos

Esta página contiene algunas preferencias relativas a cómo tus productos son gestionados y mostrados por PrestaShop.

## Preferencias generales <a href="#preferenciasdeproductos-preferenciasgenerales" id="preferenciasdeproductos-preferenciasgenerales"></a>

![](../../../.gitbook/assets/54887085.png)

* **Modo catálogo**. La activación del Modo Catálogo convierte a tu tienda en un simple escaparate de productos, sin posibilidad de comprar productos.
* **Límite para el comparador de productos.** Esta opción permite establecer el número máximo de productos que pueden ser comparados.
* **Número de días en los que el producto es considerado una "novedad"**. Cuando añades un producto a tu tienda, este es considerado nuevo y será visible tanto en el bloque "Novedades" como en la página "Nuevos productos". El campo te permite especificar el número de días que el producto permanecerá visible en el bloque y en la página. Con esta funcionalidad, tu decides cómo mostrar y actualizar las novedades de tu tienda. La página "Nuevos productos" es generalmente la más visitada por tus clientes habituales.
* **Redireccionar después de añadir un producto al carrito**. Puedes redireccionar al cliente a la página anterior, o al resumen del carrito.
* **Tamaño máximo para la descripción corta**. Tu producto tiene dos descripciones: una "descripción corta" y otra normal. La descripción corta, aparece en los buscadores, y en la sección descripción de tu producto. De manera predeterminada, está limitada a 400 caracteres, pero esta opción te permite cambiar este límite. 0 significa que la descripción corta, no está limitada.
* **Aplicar descuentos por cantidad basados en**. Esta configuración indica la base en la que Prestashop debe basarse para aplicar descuentos: por producto, o por combinación (que puede presentar múltiples productos).
* **Forzar la actualización de URL amigables**. De manera predeterminada, la URL amigable de la página de un producto es generada a partir del nombre del producto, y ésta continuará siendo la misma aunque cambies el nombre del producto – con la finalidad de que tus productos estén bien referenciados, sus URL's deben ser estables. Al activar esta opción, PrestaShop actualizará la URL amigable cada vez que cambies el nombre del producto o el título de la página.

![](../../../.gitbook/assets/54887088.png)

## Preferencias de Paginación <a href="#preferenciasdeproductos-preferenciasdepaginacion" id="preferenciasdeproductos-preferenciasdepaginacion"></a>

* **Productos por página**. Indica cuántos productos se mostrarán en las páginas de tus categorías.
* **Ordenar productos por**. Indica el orden de los productos en las categorías de tu tienda. 6 opciones están disponibles:\

  * **Nombre del producto**. Muestra tus productos por orden alfabético.
  * **Precio del producto**. Muestra tus productos conforme a sus precios.
  * **Fecha de creación**. Muestra tus productos de acuerdo a la fecha en la que fueron añadidos a tu tienda.
  * **Fecha de modificación**. Cuando se edita un producto, su fecha de modificación cambia. Esta opción hace que tus productos aparezcan en el orden de la fecha de modificación.
  * **Posición dentro de la categoría**. Muestra tus productos tal como ellos fueron posicionados en las categorías de su catálogo. La posición de los productos puede ser modificada en el catálogo de tu tienda usando las flechas de posición. De esta manera, podrás mostrar primero los productos más interesantes para tus clientes.
  * **Fabricante**. Muestra tus productos en orden alfabético de los nombres de sus fabricantes.
  * **Cantidad de producto**. Muestra tus productos en base a su cantidad disponible.
  * **Referencia del producto**. Muestra tus productos en función de su número de referencia.
* **Método de ordenación predeterminada**. Las opciones anteriores pueden ser ordenadas de forma ascendente o descendente.![](../../../.gitbook/assets/54887092.png)

## Preferencias de la página del producto <a href="#preferenciasdeproductos-preferenciasdelapaginadelproducto" id="preferenciasdeproductos-preferenciasdelapaginadelproducto"></a>

* **Mostrar las cantidades disponibles en la página de producto**. Al habilitar esta funcionalidad, los visitantes pueden ver las cantidades en stock disponibles de cada producto. La visualización de esta información se puede utilizar para estimular las ventas en el caso de que la cantidad en stock sea baja. Las cantidades mostradas dependerán de los atributos y combinaciones seleccionadas.
* **Mostrar número de productos disponibles si su cantidad es inferior a**. Puedes optar por mostrar una alerta cuando el stock disponible restante de un producto se encuentre por debajo de un cierto nivel. Esta opción es particularmente útil para promocionar compras. Tanto el texto como el posicionamiento de la alerta dependerán del tema que estés utilizando; en el tema predeterminado, ésta muestra el mensaje "Advertencia: ¡Últimas unidades en stock!", debajo del campo "Cantidad".
* **Activar JqZoom (lupa) en lugar de Fancybox en la página de producto**. De manera predeterminada, al hacer clic con el botón derecho del ratón, se mostrará una versión más grande de la imagen del producto. Si activas esta funcionalidad, los visitantes seguirán teniendo la posibilidad de hacer clic sobre las imágenes para visualizarlas a un mayor tamaño pero en este caso también se producirá una ampliación de la zona de la imagen por donde pase el ratón.
* **Mostrar productos con atributos no disponibles en la página de producto**. Tus productos pueden estar compuestos de combinaciones o atributos diferentes: color, tamaño, capacidad, etc. Los atributos pueden ser editados desde la página "Atributos" en el menú "Catálogo". Consulta el capítulo titulado "Una mirada interna al Catálogo" para obtener más información sobre los atributos y aprender a utilizarlos.\
  Cuando un producto con uno o varios atributos ya no está disponible, tienes dos posibilidades:\

  * Primera posibilidad: Dejar esta preferencia activa. Ejemplo: El "iPod Shuffle" no está disponible en color "Azúl" en su tienda. Al mantener esta opción activada, la combinación del producto permanecerá visible en la tienda. Un mensaje indicará que el producto ya no está disponible en la opción elegida, e invitará a los clientes a seleccionar otra combinación. Si has activado la opción "Permitir comprar productos fuera de stock" (véase más adelante), los clientes podrán añadir los productos a sus carritos aunque la combinación no esté disponible.
  * Segunda posibilidad: Desactivar esta preferencia. Si la combinación "Azúl" del producto "iPod Shuffle" no está disponible, esta selección no se mostrará en el front-office y los clientes no podrán seleccionarla. Esta característica ayuda a visualizar claramente la disponibilidad de tus productos.
* **Mostrar el botón "añadir al carrito" cuando el producto tiene atributos**. Esta opción evita que los clientes puedan añadir un producto a su carrito directamente desde la página de la categoría, si ese producto tiene combinaciones. Esto obliga a que los clientes visiten la página del producto, y allí sea donde elijan una combinación, de esta manera se evita la confusión de que los clientes añadan el producto con la combinación predeterminada que aparece en la página de la categoría. Ten en cuenta que los productos que no tienen ninguna combinación tendrán un botón "Añadir al carrito", en la página de la categoría.
* **Separador del atributo ancla en los enlaces del producto**. Elige el separador que deseas utilizar entre las dos opciones disponibles: "," y "-".
* **Mostrar el precio descuento incluido**. En la tabla de descuentos por volumen, muestra el nuevo precio con el descuento aplicado en lugar de mostrar sólo el descuento (ej. "-5%").![](../../../.gitbook/assets/54887097.png)

## Preferencias de productos en stock <a href="#preferenciasdeproductos-preferenciasdeproductosenstock" id="preferenciasdeproductos-preferenciasdeproductosenstock"></a>

* **Permitir ventas de productos que no están en stock**. Aunque un producto no tenga unidades disponibles en stock, el cliente podría comprar o no este artículo.
* **Activar la gestión automática del inventario**. Esta opción te permite ajustar la función principal del gestor de existencias: puedes establecer la cantidad actual que tiene un producto (stock), y permitir que PrestaShop reduzca esta cantidad cada vez que se produzca un pedido, e incremente esta cantidad por cada pedido cancelado o devuelto.\
  &#x20;De manera predeterminada, deberías dejar esta función activada, ya que al desactivarla afectarías a toda el inventario de tu tienda. Solamente debes desactivar esta opción, si no tienes ningún inventario físico  – por ejemplo, si sólo vendes productos virtuales.
* **Habilitar la administración avanzada de stock**. Otra pequeña opción que tiene importantes implicaciones: ésta añade un nuevo menú denominado "Stocks", que te permite manejar con precisión el inventario, incluso de varios almacenes si es necesario. Puedes visualizar todos los detalles del inventario: movimiento, administrar los proveedores y almacenes, realizar pedidos de suministro, etc.\
  &#x20;Puedes aprender más sobre la administración avanzada de stock, leyendo el capítulo de esta guía "Gestionar el stock".
* **Los productos nuevos utilizan la administración avanzada de stock**. Si se activa, los nuevos productos usarán automáticamente la administración avanzada de gestión de stock. El almacén predeterminado es el que se indica en la siguiente opción.
* **Almacén predeterminado en productos nuevos**. Si está utilizando la administración avanzada de stock para los nuevos productos, tienes que indicar tu almacén predeterminado  en esta opción.
