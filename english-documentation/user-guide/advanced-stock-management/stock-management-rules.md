# Stock Management Rules

In this section, we will explain the management rules that are automatically applied to stock management.

Each stock entry and exit must be valued. That is why each unit product stock must be associated with a tax-excluded unit price (either purchase price or production cost), whether through supplier order, or manual entry. Each product exit must also be valued.

There are three main valuation methods that you can choose, depending on your business activity or on the tax laws of each warehouse's country or origin:

* FIFO (first in, first out).
* LIFO (last in, first out).
* AVCO (Average Cost, or Weighted Average Cost per Unit).

With the FIFO and LIFO methods, each unit product from the stock has a purchase price that has been fixed when it entered the stock. This way, for a given reference available in 100 units, 40 units can have a purchase price of X, and 60 can have a purchase price of Y. When an order is made, and depending on the chosen method, you know which product to use and with which purchase price, which enables you to precisely manage a potential order return and put the products back into stock with their original purchase price.

The table below gives you an example of the FIFO method of stock valuation. In this example, you have a two-input table (price and quantity per type of stock movement). You add more columns as we receive new products with new prices.

| Price         | 4     | 6     | 7   |
| ------------- | ----- | ----- | --- |
| Initial stock | 1000  |       |     |
| Entry         |       | 500   |     |
| Exit          | (700) |       |     |
| Exit          | (300) | (400) |     |
| Entry         |       |       | 900 |
| Instant state | 0     | 100   | 900 |

The stock value during the instant state in this case is 6,900.

The table below illustrates how the LIFO method can be used to value stock. We use the same entry and exit values as in the previous example. The principle remains the same as in the FIFO example, except that during exits, we primarily use the units that were the last to be entered in the stock.

| Price         | 4     | 6     | 7   |
| ------------- | ----- | ----- | --- |
| Initial stock | 1000  |       |     |
| Entry         |       | 500   |     |
| Exit          | (200) | (500) |     |
| Exit          | (700) |       |     |
| Entry         |       |       | 900 |
| Instant state | 100   | 0     | 900 |

The stock value during the instant state in this case is of 6,700.

The third most frequently used method for stock valuation is Weighted Average Cost (AVCO). The AVCO calculation is done after each new entry in the stock.

For a given product, the AVCO calculation is done using this formula:

AVCO = (QS \* previous AVCO + QA \* UP) / (QS + QA)\
&#x20;Unless QS is negative or null, in which case AVCO = UP.

With:

* QS = Quantity of products currently in stock, or initial stock.
* QA = Quantity of products to be added to stock.
* UP = Unit Price (tax-excluded purchase price, or production cost).

The table below illustrates the evolution of the AVCO with the example of a product initially with 20 units in stock, and purchased at a price of 2. The new entry/exit will be valued as follows:

|               | Entry | Entry UP | Exit | Exit UP | AVCO | Stock valuation |
| ------------- | ----- | -------- | ---- | ------- | ---- | --------------- |
| Initial stock | 20    | 2        |      |         | 2    | 40              |
| X Date        |       |          | 12   | 2       | 2    | 16              |
| Y Date        | 20    | 3.4      |      |         | 3\*  | 84              |
| Z Date        |       |          | 10   | 3       | 3    | 54              |

\*: Calculation details: ((8 remaining product in stock \* 2) + (20 products to add \* 3.4)) / 28 total products = 3.

At the Y date, we calculated the AVCO according to the number of products added in the stock their unit prices. Therefore, all products in stock now have a reassigned unit value, which depends on the new AVCO.
