# Configurar Métodos de pago y restricciones

Con PrestaShop, puedes aceptar transacciones realizadas por tus clientes utilizando diferentes métodos de pago, tales como cheques, transferencia bancaria, contra reembolso, y a través de muchos otros módulos de asociados como PayPal, Moneybookers, Hipay, etc.

En la página "Pago", encontrarás las siguientes secciones:

* **Listado de los módulos de pago**. Básicamente, un acceso directo a la sección "Plataforma de pago", de la página "Módulos". Puedes instalar módulos directamente desde esta página.
* Tres secciones "restricciones":
  * **Restricciones por moneda**. Elige la moneda con la cual tus módulos de pago instalados deben trabajar.
  * **Restricciones por grupo**. Elige los grupos de usuarios con los cuales tus módulos de pago instalados deben trabajar.
  * **Restricciones por país**. Elige los países con los que tus módulos de pago instalados deben trabajar.

## Instalar un módulo de pago <a href="#configurarmetodosdepagoyrestricciones-instalarunmodulodepago" id="configurarmetodosdepagoyrestricciones-instalarunmodulodepago"></a>

La instalación de un módulo de pago no presenta diferencias con la de instalación de cualquier otro módulo: simplemente haz clic en el botón "Instalar", y todo lo que quedarás por hacer es configurar el módulo.\
Debes prestar mucha atención a la configuración de estos módulos de pago, y comprobar que tu dirección o tu cuenta bancaria están establecidas en estos módulos. Para la configuración de algunos de los módulos de pago deberás establecer los datos proporcionados por el proveedor del servicio, por lo que tendrás que tener una cuenta en éste.

Vamos a instalar el módulo "Pago contra reembolso". Encuentra el módulo en el listado, y haz clic en el botón "Instalar". PrestaShop se hará cargo de todo, te enviará a la página del listado de todos los módulos, y notificará el resultado. Por ejemplo, si un módulo necesita ser configurado antes de que puedas trabajar con él, PrestaShop se lo notificará mostrándote un cuadro de notificación en la parte superior de la página. En el caso del módulo "Pago contra reembolso", no hay nada que configurar.

![](../../../.gitbook/assets/30245040.png)

## Restricciones por Moneda de los Módulos de Pago <a href="#configurarmetodosdepagoyrestricciones-restriccionespormonedadelosmodulosdepago" id="configurarmetodosdepagoyrestricciones-restriccionespormonedadelosmodulosdepago"></a>

Dependiendo de la forma de pago elegida por el cliente, las opciones permitidas para realizar el pago pueden variar.\
&#x20;Puedes limitar la elección de los métodos de pago en función de las divisas disponibles: es posible que desees que los clientes puedan pagar con cualquier moneda, cuando utilicen PayPal, pero que los clientes que utilicen Moneybookers sólo puedan pagar en dólares, por ejemplo.

![](../../../.gitbook/assets/54886797.png)

De manera predeterminada, solamente la moneda utilizada por tu tienda está disponible para realizar los pagos. Si necesitas alguna más, sigue este proceso:

1. En la página "Localización" bajo el menú "Localización", importa el paquete de localización del país que tiene la moneda en la que estás interesado. Por ejemplo, USA para Dolares Américanos, Reino Unido para Libras Esterlinas, etc.
2. En la página "Monedas" bajo el menú "Localización", activa la moneda que acabas de importar.

Si necesitas restringir el uso de un módulo de pago de acuerdo a la moneda del usuario, simplemente selecciona las casillas correspondientes y haz clic en "Guardar restricciones".

Ten en cuenta que las restricciones monetarias funcionan de diferentes formas dependiendo del módulo de pago:

* Para algunos, como Contra reembolso, no puedes cambiar la configuración que tienen por defecto.
* Para otros, como Transferencia bancaria, Pago por cheque, Skrill, Ogone, etc., puedes cambiar la configuración establecida, a excepción de las opciones "Moneda del cliente" y "Moneda predeterminada de la tienda", que permanecerán en su estado predeterminado.
* Y para otros módulos como Hipay o PayPal, puedes cambiar la configuración establecida, pero tan sólo puedes elegir una opción entre "Moneda del cliente" y "Moneda predeterminada de la tienda", no ambas.

El cliente puede establecer la moneda con la que quiere que trabaje la tienda, utilizando el menú desplegable situado en la parte superior de cada página del front-office.

Puedes establecer la moneda predeterminada de tu tienda desde la página "Localización", bajo el menú "Localización".

Si cambias la moneda predeterminada después de haber configurado los primeros productos, tendrás que restablecer el precio de todos estos productos. Debes establecer la moneda predeterminada antes de añadir los productos.

## Restricciones por Grupo de los Módulos de Pago <a href="#configurarmetodosdepagoyrestricciones-restriccionesporgrupodelosmodulosdepago" id="configurarmetodosdepagoyrestricciones-restriccionesporgrupodelosmodulosdepago"></a>

Puedes limitar la elección de los módulos de pago disponibles en función de los grupos de clientes: puedes tener un número determinado de grupos de clientes que tengan acceso a un mayor número de métodos de pago.

![](../../../.gitbook/assets/54886803.png)

Por ejemplo, podrías establecer que los clientes que no pertenecen a un grupo especial paguen a través de PayPal, Skrill y Hipay, mientras que otros clientes que pertenecen a otro grupo podrían realizar sus pagos por transferencia bancaria. En función del tipo de cliente y sus opciones, los clientes sólo pueden pagar con los métodos de pago que hayas establecido para ellos.

## Restricciones por Países de los Módulos de Pago <a href="#configurarmetodosdepagoyrestricciones-restriccionesporpaisesdelosmodulosdepago" id="configurarmetodosdepagoyrestricciones-restriccionesporpaisesdelosmodulosdepago"></a>

Puedes limitar la elección de los módulos de pago disponibles de acuerdo al país de origen de tus clientes. Por ejemplo, puedes optar por aceptar todos los métodos de pago para los clientes procedentes de Francia, España y Alemania, mientras que los clientes de Italia, Reino Unido y Suiza, sólo puedan pagar por transferencia bancaria.

![](../../../.gitbook/assets/54886800.png)

La tabla enumera todos los países conocidos. Si falta alguno, puedes añadirlo utilizando la página "Países", bajo el menú "Localización".

Al igual que ocurre con las limitaciones de monedas, las opciones disponibles varían en función del módulo de pago:

* Para algunos, la única opción es su propio país.
* Para otros, las únicas opciones son los países soportados por el servicio: Austria, Bélgica, Francia, etc.
* Todos los demás módulos de pago nativos deberían funcionar con todos los países.

Encuentra el país que deseas configurar en el listado de países (ordenado alfabéticamente), y marca las casillas para establecer los métodos de pago que desees que estén disponibles para los clientes de ese país. Una vez configurados los métodos de pago de dicho país, haz clic en el botón "Guardar restricciones", que encontrarás al final de la tabla.\
&#x20;De manera predeterminada, todos los métodos de pago instalados están habilitados para el país de la tienda.
