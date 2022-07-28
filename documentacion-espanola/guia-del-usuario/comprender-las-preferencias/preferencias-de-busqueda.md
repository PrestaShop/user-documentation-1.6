# Preferencias de Búsqueda

La página "Búsqueda" te permite configurar las funciones de búsqueda de tu tienda.

## Listado de alias <a href="#preferenciasdebusqueda-listadodealias" id="preferenciasdebusqueda-listadodealias"></a>

Cuando los clientes realizan una consulta utilizando el buscador interno de tu tienda, podrían cometer errores. Si PrestaShop no encuentra resultados correctos para la consulta del cliente, la característica "alias" podría proporcionar al cliente ciertas alternativas. De esta manera, podría sregistrar productos que pudieran causar errores al escribirlos, y corregir las consultas erróneas introducidas por tus clientes.

![](../../../.gitbook/assets/54887224.png)

Para crear un nuevo alias, deberías primero conocer los errores de escritura cometidos más frecuentemente por tus clientes:

1. Dirígete a la pestaña "Palabras clave en el motor de búsqueda" de la página "Estadísticas", bajo el menú "Estadísticas". Desde aquí puedes ver las palabras escritas por tus clientes, así como los errores más frecuentes que cometen.
2. Toma nota de los errores más frecuentes, y añádelos a tu listado de alias, para indicar al usuario el producto correcto que seguramente esté buscando.
3. Haz clic en el botón "Añadir nuevo" en la página de preferencias "Buscar".

El formulario de creación tan solamente presenta dos campos que tendrás que rellenar: indicar el error que deseas corregir, y presentar la palabra corregida correspondiente a dicha consulta.

![](../../../.gitbook/assets/30245120.png)

Por ejemplo, supongamos que tus clientes con frecuencia escriben erróneamente la palabra "player" utilizando los términos "palyer" y "plaier". Puedes crear un alias para cada uno de estos errores, el cual corresponderá con la palabra "Player". Tus alias pueden ser utilizados tan pronto como se guardan.

Te invitamos a que consultes las secciones de esta guía dedicadas a las metaetiquetas de los productos y las categorías, para que comprendas mejor de qué manera PrestaShop muestra los productos basándose en las palabras escritas por tus clientes. Consulta los capítulos "Añadir productos y categoría de productos" y "Una mirada interna al catálogo".

## Indexación <a href="#preferenciasdebusqueda-indexacion" id="preferenciasdebusqueda-indexacion"></a>

Esta sección proporciona información sobre el número de productos que se pueden buscar a través del buscador de tu tienda, y lo compara con el número de productos presentes en la base de datos. Si los valores no coinciden, debes hacer clic en el enlace "Añadir los productos que faltan al índice". Sólo los nuevos productos serán indexados.

![](../../../.gitbook/assets/54887227.png)

Si has realizado cambios a los productos ya indexados, es posible que prefieras volver a reconstruir todo el índice. El proceso "Reconstruir el índice completo" toma más tiempo, pero es más completo.

PrestaShop también te ofrece una dirección URL para ejecutar una tarea periódicamente, utilizando "cron" (en Linux) o "Tareas programadas" (en Windows) que reconstruya tu índice automáticamente. Si no sabes lo que es una tarea cron o un archivo crontab, ponte en contacto con tu proveedor de hosting.

Finalmente, la opción "Indexando" te permite indexar los productos  tan pronto como son creados o son modificados, de lo contrario, tendrás que indexar los productos de forma manual o automática utilizando el enlace previamente mencionado.

## Opciones de búsqueda <a href="#preferenciasdebusqueda-opcionesdebusqueda" id="preferenciasdebusqueda-opcionesdebusqueda"></a>

Esta sección te permite configurar el comportamiento de la función de búsqueda de tu tienda:

![](../../../.gitbook/assets/54887230.png)

* **Búsqueda AJAX**. Al habilitar esta opción el cliente obtendrá una lista de 10 resultados que se mostrarán debajo de la barra de búsqueda, en el mismo momento en el que escriba unas cuantas letras.
* **Búsqueda instantánea**. Al habilitar esta opción, el resultado aparecerá inmediatamente en la barra de búsqueda, mientras el usuario escribe su consulta. Este ajuste está desactivado por defecto, porque muchos visitantes no están acostumbrados a ver todo el contenido coincidente y escribir al mismo tiempo en la barra de búsqueda. Por lo tanto, utiliza esta opción con precaución.
* **Buscar en el interior de las palabras**. Esta opción mejora las búsquedas, permitiendo encontrar coincidencias no sólamente al inicio de la cadena, sino también en el interior de las mismas; por ejemplo, "lus" para "blusa".
* **Buscar coincidencia exacta**. Con esta opción activada, puedes ofrecer resultados que coincidan exactamente con el final de la palabra de búsqueda. Por ejemplo, si buscas "libro", visualizarás "portalibro", pero no "librero".
* **Longitud mínima de la palabra (en carácteres)**. Puedes seleccionar el tamaño mínimo que debe tener una palabra para se registre en el índice de búsqueda y pueda ser encontrada por tus clientes. Esta característica te permite eliminar palabras cortas en la búsqueda, como preposiciones o artículos (el, y, por, etc.)
* **Palabras en la lista negra**. Puedes añadir las palabras que serán descartadas automáticamente de los términos de búsqueda. Introdúcelas directamente en este campo, separando cada una de ellas con un carácter "|". (carácter "pleca" o también denominado "barra vertical", no L minúscula). De manera predeterminada, PrestaShop rellena la lista con palabras cortas comunes.

## Peso <a href="#preferenciasdebusqueda-peso" id="preferenciasdebusqueda-peso"></a>

PrestaShop te permite dar prioridad a ciertos datos cuando se realiza una búsqueda en tu tienda.

![](../../../.gitbook/assets/54887235.png)

Como se indica en la sección, el "Peso" representa el grado de importancia y de relevancia que se le dará a los campos en los resultados de una búsqueda.\
Un artículo con un peso 8 tendrá 4 veces más valor que un artículo con peso 2.

Por ejemplo, de manera predeterminada el "Peso del nombre del producto" tiene un valor 6, el "Peso de las etiquetas" tiene un valor 4, y tanto el "Peso de la descripción breve" como el "Peso de la descripción" tienen un valor 1. Esto significa que un producto con "ipod" en su nombre aparecerá más alto en los resultados de la búsqueda que otro producto que tenga "ipod" sólo en sus etiquetas. Mientras tanto, un producto que sólo tenga "ipod" en cualquiera de sus campos de descripción ocupará la posición más baja en los resultados de la búsqueda.

Dispones de muchos elementos a los que puedes asignar un peso: descripción breve, categorías, etiquetas, atributos, etc. Te darás cuenta de que los resultados pueden revertirse simplemente cambiando el peso de ciertos campos. El refinamiento de estos ajustes será especialmente visible en los catálogos con muchas referencias.

Una vez hayas guardado los cambios realizados, serán aplicados inmediatamente.
