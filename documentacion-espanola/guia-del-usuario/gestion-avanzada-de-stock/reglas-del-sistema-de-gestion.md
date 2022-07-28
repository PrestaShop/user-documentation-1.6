# Reglas del sistema de gestión

En esta sección, explicaremos las reglas de gestión que son automáticamente aplicadas en la gestión del stock.

Cada entrada y salida de stock debe ser valorizada. Esto es debido a que cada unidad en existencia del producto debe tener un precio unitario sin impuestos incluidos (ya sea el precio de compra o el de coste de producción) asociado, ya sea a través de un pedido de suministro o de una entrada manual. Cada salida de producto también debe ser valorizada.

Hay tres métodos principales de valoración que puedes elegir, en función de tu actividad o de las normas vigentes en tu país para cada almacén:

* FIFO (primero en entrar, primero en salir).
* LIFO (último en entrar, primero en salir).
* AVCO (Costo promedio o coste medio ponderado por unidad).

Con los métodos FIFO y LIFO, cada unidad de producto en existencia tiene un precio de compra que fue fijado en el momento de introducir las existencias. De esta manera, para una referencia determinada que tenga 100 unidades disponibles, 40 unidades pueden tener un precio de compra X, y 60 pueden tener un precio de compra Y. Cuando se realiza un pedido, y dependiendo del método elegido, sabrás que producto utilizar y su precio de compra, lo que te permite gestionar con precisión una eventual devolución y volver a poner los productos de nuevo en stock con su precio de compra original.

La siguiente tabla ofrece un ejemplo del método FIFO de valoración de stock. En este ejemplo, dispones de una tabla de doble entrada (precio y cantidad por tipo de movimiento). Se añaden más columnas cuando se reciban productos con nuevos precios.

| Precio                | 4     | 6     | 7   |
| --------------------- | ----- | ----- | --- |
| Existencias iniciales | 1000  |       |     |
| Entrada               |       | 500   |     |
| Salida                | (700) |       |     |
| Salida                | (300) | (400) |     |
| Entrada               |       |       | 900 |
| Estado instantáneo    | 0     | 100   | 900 |

La valoración del stock durante el estado instantáneo es en este caso de 6,900.

La siguiente tabla ilustra cómo puedes utilizar el método LIFO para valorizar las existencias. Utilizamos los mismos valores para las entradas y salidas del ejemplo anterior. El inicio es idéntico al del ejemplo FIFO, excepto que durante las salidas, utilizamos principalmente las unidades que fueron las últimas que fueron introducidas en las existencias.

| Price                 | 4     | 6     | 7   |
| --------------------- | ----- | ----- | --- |
| Existencias iniciales | 1000  |       |     |
| Entrada               |       | 500   |     |
| Salida                | (200) | (500) |     |
| Salida                | (700) |       |     |
| Entrada               |       |       | 900 |
| Estado instantáneo    | 100   | 0     | 900 |

La valoración de existencias durante el estado instantáneo es en este caso de 6,700.

El tercer método más utilizado para la valoración de las existencias es el Costo Promedio Ponderado (AVCO). El cálculo AVCO se realiza después de cada nueva entrada de existencias.

Para un producto dado, el cálculo AVCO se realiza utilizando la siguiente fórmula:

AVCO = (QS \* AVCO anterior + QA \* UP) / (QS + QA)\
&#x20;A no ser que QS sea negativo o nulo, en cuyo caso AVCO = UP.

De acuerdo a esta fórmula:

* QS = Cantidad de productos actualmente en existencia o existencias iniciales.
* QA = Cantidad de productos a añadir a las existencias.
* UP = Precio unitario (precio de compra sin IVA incluido, o coste de producción).

La tabla siguiente muestra la evolución del AVCO con el ejemplo de un producto inicialmente establecido con 20 unidades en existencias, y comprado a un precio de 2. Cada nueva entrada/salida se valorará de la siguiente manera:

|                       | Entrada | Entrada UP | Salida | Salida UP | AVCO | Valoración de las existencias |
| --------------------- | ------- | ---------- | ------ | --------- | ---- | ----------------------------- |
| Existencias iniciales | 20      | 2          |        |           | 2    | 40                            |
| Fecha X               |         |            | 12     | 2         | 2    | 16                            |
| Fecha Y               | 20      | 3.4        |        |           | 3\*  | 84                            |
| Fecha Z               |         |            | 10     | 3         | 3    | 54                            |

\*: Detalles del cálculo: ((8 unidades restantes en existencia \* 2) + (20 productos añadir \* 3.4)) / 28 productos totales = 3.

En la fecha Y, se calculó el AVCO de acuerdo con el número de productos añadidos a las existencias y su nuevo precio unitario. Por lo tanto, todos los productos en existencia tienen ahora un precio unitario reasignado, que depende del nuevo AVCO.
