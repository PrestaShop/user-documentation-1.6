# Servicio de atención al cliente

PrestaShop te permite centralizar todas las solicitudes de los clientes dentro de sus confines. Esto te ayuda a mantener un seguimiento de los temas de discusión que necesitas responder, en lugar de tener que consultar todas las bandejas de salida de tus cuentas de correo para ver si han respondido a ellas, o lo ha hecho ya algún otro miembro de tu equipo.

En la práctica, el formulario de contacto de tu tienda, disponible en los enlaces "Contáctenos" situados en la parte inferior y superior del front-office de tu tienda, presenta al cliente dos contactos predeterminados: "Webmaster" y "Servicio de Atención al cliente". El cliente sólo tiene que elegir con quién contactar, y a continuación, rellenar el resto de campos. El mensaje es guardado posteriormente, en la herramienta de Servicio al cliente de PrestaShop.

![](../../../.gitbook/assets/54268442.png)

Los temas de discusión sólo son almacenados en la herramienta de servicio al cliente, siempre que cuente con la opción "¿Guardar en servicio al cliente?" habilitada. Puedes cambiar esta configuración, o añadir más contactos, dirigiéndote a la página de "Contactos", bajo el menú "Clientes". Esta página se explica con detalle en la siguiente sección de este capítulo de la Guía del usuario de PrestaShop.

Si la opción está deshabilitada para el contacto que elija el cliente, el mensaje será simplemente enviado a la dirección de correo electrónico del contacto, y no será almacenado en PrestaShop.

También es necesario configurar correctamente tu configuración IMAP, para que así PrestaShop pueda recibir respuestas de los clientes de los emails que fueron enviados desde la herramienta de Servicio al cliente. Esto se realiza en la sección "Opciones de servicio al cliente".

En esta página, cada contacto tiene su propio cuadro, donde pueden ver rápidamente si hay mensajes nuevos (es decir, aquellos que aún no han sido leídos). De manera predeterminada, hay dos, y si añadimos más contactos las cajas "Significado del estado" y "Estadísticas" se desplazarán más a la izquierda y hacía abajo.

Estos dos últimos cuadros son muy útiles cuando necesitas gestionar los nuevos mensajes recibidos en el día:

* **Significado del estado**. Un simple recordatorio de los códigos de color que tu equipo puede aplicar a un hilo de discusión.
* **Estadísticas**. Una visión general de la actividad global del Servicio de atención al cliente desde el nacimiento de tu tienda.

Más abajo se encuentra el listado de los mensajes recibidos, tanto antiguos como nuevos.

Puedes editar un par de opciones en la parte inferior de la página, que se aplicarán a todos los contactos:

* **Permitir subida de archivos**. Donde el cliente puede adjuntar un archivo al mensaje. Esto puede serte útil en caso de problemas gráficos en tu tienda, ya que el cliente puede enviar capturas de pantalla.
* **Mensaje predeterminado**. La plantilla predeterminada para la respuesta de tus empleados. Compón un mensaje simple, de modo que pueda adaptarse a muchas situaciones, realizando las mínimas modificaciones.

Finalmente, en la parte inferior de la página se presenta la sección "Opciones de Servicio al cliente", donde puedes configurar muchas opciones relacionadas con tu servidor de correo (IMAP).

## Gestionar los mensajes del Servicio de atención al cliente <a href="#serviciodeatencionalcliente-gestionarlosmensajesdelserviciodeatencionalcliente" id="serviciodeatencionalcliente-gestionarlosmensajesdelserviciodeatencionalcliente"></a>

Cada conversación con un cliente puede ser gestionada enteramente a través de la completa interfaz de PrestaShop, sin tener que utilizar un cliente de correo electrónico como Outlook o Thunderbird.

![](../../../.gitbook/assets/54268447.png)

En la lista de conversación, haz clic sobre una fila para visualizar los detalles de la conversación:

* Puedes aplicar un puñado de acciones a una discusión, con el fin de ordenarlas y así gestionarlas más rápidamente. Hay 4 estados disponibles:\

  * **Marcar como "gestionado"** o **"Reabrir"**. Cambia el estado de la discusión de "Cerrado" o "Abierto".
  * **Marcar como "pendiente 1"** y **Marcar como "pendiente 2"**. Estos dos estados son internos: sus significados dependen de tu equipo. Puedes incluso optar por no utilizarlos, y dejarlo todo en manos de los estados "Abierto" y "Cerrado".
  * **Transferir esta conversación a otro empleado**. Desde el instante en que un empleado comienza a responder a un mensaje del cliente, se convierte en el responsable de la solicitud del cliente. Si durante la discusión resulta que es otro empleado el que debe gestionar la situación, puedes utilizar este botón para atribuirselo a través de una lista desplegable. Ese otro empleado recibirá una notificación al respecto. Si la persona que deseas que continúe la presente discusión no está disponible en la lista, selecciona "Otra persona (Someone else)" en la lista desplegable y dos opciones más aparecerán, permitiéndote indicar la dirección de correo electrónico del destinatario y un comentario acerca de tu mensaje.
* **Responder al siguiente mensaje sin respuesta en este hilo**.

El equipo de la tienda también tiene acceso a los detalles esenciales:

* Nombre del cliente y correo electrónico, en los que puedes hacer clic para acceder a la información del cliente
* Número de pedidos, importe total gastado y la fecha de registro del cliente.
* Fecha y hora del mensaje.
* Finalmente, el propio mensaje.

Para responder a este hilo, sólo tienes que utilizar el formulario con tu mensaje predeterminado (que se establece en la sección "Opciones de contacto" de la página "Servicio al cliente"), y hacer clic en "Enviar".

En la parte inferior de la página, la sección "Pedidos e históricos de mensajes" te ofrece una clara vista cronológica de los acontecimientos pertenecientes a este hilo de discusión.

![](../../../.gitbook/assets/54268450.png)

## Opciones del Servicio de atención al cliente <a href="#serviciodeatencionalcliente-opcionesdelserviciodeatencionalcliente" id="serviciodeatencionalcliente-opcionesdelserviciodeatencionalcliente"></a>

Básicamente, esta sección te permite configurar con precisión el acceso de PrestaShop a tu servidor de correo electrónico a través de su interfaz IMAP. Deberías asegurarte de rellenar todos los campos necesarios con el fin de que la herramienta de servicio al cliente funcione correctamente. La mayor parte de esta información debería ser proporcionada por tu proveedor de hosting.

![](../../../.gitbook/assets/54268452.png)

* **URL IMAP, Puerto IMAP, Usuario IMAP** y **Contraseña IMAP**. Los detalles esenciales para acceder al servidor de correo electrónico utilizando el protocolo IMAP.
* **Eliminar mensajes**. Si se activa, los mensajes en el servidor serán eliminados tan pronto como PrestaShop los reciba. Utiliza esta opción con precaución: esto haría que tus mensajes no se encuentren disponibles para otros clientes de correo electrónico.
* **/norsh**. Si se activa, la conexión con el servidor de correo electrónico no será preautenticada. No se recomienda.
* **/ssl**. Si se activa, la conexión al servidor de correo electrónico no será cifrada. No se recomienda.
* **/validate-cert**. Si se activa, PrestaShop obligará a validar el certificado TLS/SSL del servidor.
* **/novalidate-cert**. Si se activa, PrestaShop nunca tratará de validar el certificado TLS/SSL del servidor. Esencial para servidores con certificados de firma.
* **/tls**. Si se activa, PrestaShop forzará el uso de StartTLS para cifrar la conexión. Los servidores que no soporten StartTLS serán rechazados.
* **/notls**. Si se activa, PrestaShop no utilizará StartTLS para cifrar la sesión, incluso con los servidores que lo soporten.
