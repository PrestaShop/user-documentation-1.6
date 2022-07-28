# Conceptos Generales

## Conceptos Generales <a href="#conceptosgenerales-conceptosgenerales" id="conceptosgenerales-conceptosgenerales"></a>

Para evitar confusiones con el gestor de stock de la versión 1.4, y ver las posibilidades que ofrece la nueva funcionalidad de gestión avanzada de stock de la versión 1.5 de PrestaShop, debes imaginar dos conceptos distintos: las existencias físicas y las cantidades de productos disponibles para la venta.

### Cantidad de productos disponibles para la venta <a href="#conceptosgenerales-cantidaddeproductosdisponiblesparalaventa" id="conceptosgenerales-cantidaddeproductosdisponiblesparalaventa"></a>

Esta es la misma funcionalidad que presenta el gestor de inventario disponible desde PrestaShop 1.4.x. Esta es la cantidad de productos que se muestran en la tienda para cada producto y combinación de productos. Esta es la cantidad que define si el producto se puede pedir o no (a menos que la opción "Permitir ventas de productos que están fuera de stock" se encuentre habilitada). Esta cantidad puede ser modificada manualmente para cada producto y combinación de producto.

En PrestaShop 1.5.x, esta cantidad puede ser determinada automáticamente de acuerdo a las existencias físicas del producto afectado. En un escenario multitienda, la cantidad es definida para cada tienda.

En consecuencia, a lo que antes llamábamos "stock" en PrestaShop 1.4.x, es ahora llamado "cantidad de productos disponibles para la venta" en PrestaShop 1.5.x.

### Existencias de productos (físicamente almacenados) <a href="#conceptosgenerales-existenciasdeproductos-fisicamentealmacenados" id="conceptosgenerales-existenciasdeproductos-fisicamentealmacenados"></a>

Esto corresponde a la gestión de productos existentes almacenados en uno o varios almacenes. Este es el nuevo concepto otorgado a "stock" en PrestaShop 1.5.x.

Esta nueva característica de gestión de existencias incluye los movimientos de stock, la valoración del stock, la transferencia de stock entre almacenes, la integración del modo multitienda y la gestión de pedidos de suministros.

También hace que sea posible tener en cuenta la noción de existencias reales. Al mismo tiempo, un producto puede tener existencias en stock, pero no estar disponible para la venta debido a que todavía hay clientes que lo pidieron y a los que todavía no se les ha enviado. Ese mismo producto puede tener una orden de suministro en curso, y por lo tanto aún no contabilizado en las existencias físicas.

El stock real es por tanto constituido por las unidades físicas en existencia que un almacén tiene disponible, a las que añadiremos las cantidades que se pidieron a los proveedores, y de la que restamos las cantidades pedidas por los clientes y que todavía no han sido enviadas.

## Utilizando el nuevo gestor de existencias <a href="#conceptosgenerales-utilizandoelnuevogestordeexistencias" id="conceptosgenerales-utilizandoelnuevogestordeexistencias"></a>

### ¿Estoy obligado a utilizar el nuevo gestor de stock? <a href="#conceptosgenerales-estoyobligadoautilizarelnuevogestordestock" id="conceptosgenerales-estoyobligadoautilizarelnuevogestordestock"></a>

No tienes ninguna obligación de utilizar el nuevo gestor de stock, así como tampoco tienes ninguna obligación de utilizar la funcionalidad "cantidad de productos disponibles para la venta".

Tanto para activar la funcionalidad "cantidad de productos disponibles para la venta" como la de existencias de productos, deberás dirigirte a la página de preferencias "Productos", donde en la parte final encontrarás la sección "Tock de productos". Seleccione "Sí" para la opción "Activar la gestión avanzada de stock". Primeramente debes habilitar el gestor básico de stock para poder habilitar el gestor avanzado de stock.

El gestor avanzando de stock, e incluso el gestor de existencias y sus almacenes, son independientes de la funcionalidad multitienda. En consecuencia, independientemente de la tienda que estés utilizando en el back-office de PrestaShop, cuando utilizas el menú "Stock", siempre estarás gestionando el stock de una manera global.

### No quiero cambiar ninguna configuración de PrestaShop 1.4.x., ¿qué debo hacer? <a href="#conceptosgenerales-noquierocambiarningunaconfiguraciondeprestashop1.4.x.-quedebohacer" id="conceptosgenerales-noquierocambiarningunaconfiguraciondeprestashop1.4.x.-quedebohacer"></a>

Si no deseas utilizar el nuevo gestor avanzado de stock de PrestaShop 1.5, y estás satisfecho con la forma en que PrestaShop 1.4 gestiona la cantidad de productos que tienes en stock, tan sólo tienes que activar el gestor de stock anterior, y no la funcionalidad del gestor avanzado de stock: dirígete a la página de preferencias "Productos", y encuentre la sección "Stock de productos", y selecciona "Sí" para la opción "¿Activar el manejo automático del inventario?", dejando la opción "Activar la avanzadas de stock" en "No".

La funcionalidad "cantidad de productos disponibles para la venta" estará ahora centralizada en la pestaña "Cantidades" de la ficha del producto: al crear un nuevo producto o editar un producto existente, aparecerá esta pestaña junto a todas las demás, a la izquierda de la pantalla.

### ¿La funcionalidad del gestor avanzado de stock se adapta a mis necesidades? <a href="#conceptosgenerales-lafuncionalidaddelgestoravanzadodestockseadaptaamisnecesidades" id="conceptosgenerales-lafuncionalidaddelgestoravanzadodestockseadaptaamisnecesidades"></a>

La nueva funcionalidad del gestor avanzado de stock permite gestionar las unidades en stock de tus productos. Esta funcionalidad se adapta a tu negocio si:

* Tienes que gestionar el número de unidades de los productos que tienes en existencia y que vendes a través de tu(s) tienda(s).
* Tienes al menos un almacén, que gestionas tu mismo.
* Pides la mayoría o todos los productos que vendes en tu tienda a uno o más proveedores.
* Necesitas conocer las estadísticas de stock y de tu(s) almacén(es).

Esta funcionalidad no se adapta a las necesidades de tu negocio si:

* No gestionas el número de unidades de los productos que tienes en existencia en tu tienda.
* Ya utilizas un sistema / herramienta / programa para gestionar el stock de tu tienda, y no deseas cambiarlo porque estás satisfecho con los resultados que te ofrece.
