# Presenting the Stock Management Interface

**Presenting the Stock Management Interface**

* ****[Stock management from the product sheet](presenting-the-stock-management-interface.md#PresentingtheStockManagementInterface-Stockmanagementfromtheproductsheet)
* [Warehouses management](presenting-the-stock-management-interface.md#PresentingtheStockManagementInterface-Warehousesmanagement.1)
* [Stock management](presenting-the-stock-management-interface.md#PresentingtheStockManagementInterface-Stockmanagement)
* [Stock Movement](presenting-the-stock-management-interface.md#PresentingtheStockManagementInterface-StockMovement)
* [Instant Stock Status](presenting-the-stock-management-interface.md#PresentingtheStockManagementInterface-InstantStockStatus)
* [Stock Coverage](presenting-the-stock-management-interface.md#PresentingtheStockManagementInterface-StockCoverage)
* [Supply orders](presenting-the-stock-management-interface.md#PresentingtheStockManagementInterface-Supplyorders)
* [Configuration](presenting-the-stock-management-interface.md#PresentingtheStockManagementInterface-Configuration)

Stock management is essential from the moment you start selling products whose quantity is depleting at each sale.\
In order to assert if you need PrestaShop's advanced stock management feature, read this chapter's "General concepts": [http://doc.prestashop.com/display/PS16/General+Concepts](http://doc.prestashop.com/display/PS16/General+Concepts).

If you wish to use the advanced stock management, you must:

* Associate your products with warehouses.
* Associate your warehouses with carriers.
* Associate your warehouses with the appropriate shops.

Stock management within PrestaShop runs through several screens, and can use one of two levels.

These levels are:

* No stock management: there is no product quantity, PrestaShop assumes that a product's stock is infinite. Use this if you only sell virtual products (files, services, etc.).
* Simple stock management: for every product you sell, you can indicate the currently available quantity (including product combinations). Use this if you have few products or a simple storing location.
* Advanced stock management: for every product you sell (and its combinations), you can indicate where the available quantity is located in an unlimited number of warehouses (with varying carriers and valuation methods). You can also see your stock movements, the current status of your stock, you stock coverage, and you can place an order to your product suppliers.

These screens are:

* Preferences > Products > Products stock: this is where you enable the feature.
  * **Enable stock management**. This option gives you access to basic stock management options and features: you can set the current quantity of product, and have PrestaShop lower it for each order, and "re-stock" for each canceled or returned order. By default you should leave this feature enabled, as disabling it affects the entire inventory management of your shop. Only if you do not have any physical inventory should you disable it – for instance, if you only have virtual products.
  * **Enable advanced stock management**. Another little option which has major implications: it adds a new menu called "Stocks", which makes it possible to manage very precisely your stock, on a per-warehouse basis if necessary. You can see all the details about your stock: movement, coverage, re-stocking orders, etc. You can read more about PrestaShop's advanced stock management feature in the "Managing Stock" chapter of this guide.
  * **New products use advanced stock management**. If enabled, new products will automatically use the advanced stock management feature. The default warehouse is the one indicated in the next option.
  * **Default warehouse on new products**. If new products use the advanced stock management feature, you have to indicate their default warehouse here.
* Catalog > Products > product's page: one to two tabs are added to the creation/edition page of a product.\

  * &#x20;Quantities:
    * In Simple mode: you can manually indicate the quantity of each product.
    * In Advanced mode: quantities are handled from PrestaShop's "Stock" menu.
  * Warehouses: in Advanced mode, you can indicate the location of a product or is combinations within a warehouse.
* Stock: in Advanced mode, you can make use of all the stock management pages (warehouse creation, stock movement, stock status, stock coverage, supplier order).

The following section describe these pages one by one.

## Stock management from the product sheet <a href="#presentingthestockmanagementinterface-stockmanagementfromtheproductsheet" id="presentingthestockmanagementinterface-stockmanagementfromtheproductsheet"></a>

### Quantities management <a href="#presentingthestockmanagementinterface-quantitiesmanagement" id="presentingthestockmanagementinterface-quantitiesmanagement"></a>

In PrestaShop 1.4, you could manually set the quantity of product available for sale.

In PrestaShop 1.5 and 1.6, you can still set the quantity manually for each product. But once advanced stock management is also enabled, you can also automatically set the quantity depending on the current quantity status of the physical product. Note that it is possible to enable advanced stock management globally, yet only use it for one product or just a few.

When the "Enable stock management" option is enabled (in the "Preferences > Products" page), all the products get a new tab in their administration page, called "Quantities". This clear and simple interface enables you to manage the available quantities for sale on your shop(s) for a given product, and any potential combination.

With only this option enabled, you can manage the product quantities for individual products, one by one.

If you prefer to have all your product quantities managed directly from PrestaShop's advanced stock management feature rather than on a product basis, you have to enable another option from the "Preferences > Products" page: "Enable advanced stock management".

![](<../../../.gitbook/assets/23789949 (2).png>)

The "Quantity" tab opens with an explanatory section, which we urge you to fully read. That section is followed by the quantities management interface itself, which opens with three options:

* **I want to use the advanced stock management system for this product**.
* **The available quantities for current product and its combinations are based on stock in your warehouses**.
* **I want to specify available quantities manually**.

By default, the third option is ("I want to specify available quantities manually") is enabled. As long as you haven't check the first option ("I want to use the advanced stock management system for this product"), quantities are managed the same way they were in version 1.4 of PrestaShop, which means that you have add the quantities manually, and PrestaShop will remove quantities for each sale.

If you'd rather synchronize the available quantities with your warehouse stock (or that of several warehouses), you have to change the quantities management method:

1. Check the "I want to use the advanced stock management system for this product" box in order the change method.
2. This makes the second option, "Available quantities for current product and its combinations are based on stock in the warehouses", finally available. Select it in order to synchronize the available quantity for this product with your warehouse stock.

As soon as you have selected the second option, the table's "Quantity" column cannot be edited anymore: quantities are now directly handled from the advanced stock management feature rather than from each product's "Quantities" tab.

Product packs are a special case. Since it is not yet possible to add product combinations to a pack, the PrestaShop developers have decided that when necessary, PrestaShop would use the default combination when decrementing the physical stock.

Also, a notice indicates the recommended maximal number of packs.

The rest of the tab explained in the "Managing the Catalog" chapter of this guide.

### Supplier management <a href="#presentingthestockmanagementinterface-suppliermanagement" id="presentingthestockmanagementinterface-suppliermanagement"></a>

You can now set more than one supplier for a given product. For each supplier associated to a product, you can set the supplier's reference number and a default purchase price for that product as well as its combination. This information is used when making an order to the supplier.

![](<../../../.gitbook/assets/23789951 (2).png>)

### Warehouses management <a href="#presentingthestockmanagementinterface-warehousesmanagement" id="presentingthestockmanagementinterface-warehousesmanagement"></a>

If advanced stock management is enabled, a "Warehouses" tab appears in the product sheet, where you can indicate which warehouse(s) the product and each of its combinations can be stored in. You can even indicate the location for the product and its combinations.

![](<../../../.gitbook/assets/23789953 (2).png>)

You must first create at least one warehouse (see below) before associating a product to it and setting the product location in it. This step is essential: it is important to at least set one warehouse in which a product can be stored. This will have considerable impact on the order preparation in the multi-shipping context.

## Warehouses management <a href="#presentingthestockmanagementinterface-warehousesmanagement.1" id="presentingthestockmanagementinterface-warehousesmanagement.1"></a>

The advanced stock management feature makes it possible to create one or more warehouses. In order to create one, go to the "Warehouse" page under the "Stock" menu.

![](<../../../.gitbook/assets/23789955 (2).png>)

Once you start creating a new warehouse, you must fill in the following fields:

* **Reference** and **Name**. The warehouse's unique reference identifier and name. Make sure to use something recognizable: you must be able to easily differentiate to warehouses from a drop-down list.
* **Address**, **Postcode/Zip Code**, **City** and **Country**. The warehouse's physical address. This information will be used on the purchase order to suppliers.
* **Manager**. A person in charge of the warehouse, chosen among your shop's registered employees. If the employee's account is not yet created, you must create it first.
* **Carriers**. The carriers who you authorize for orders shipping from this warehouse. Maintain the "Shift" key pressed while clicking to select more than one carrier.
* **Management type**. A method of accounting valuation, based on your country's regulations. See the "Stock management rules" part of this chapter for more information.
* **Stock valuation currency**. A valuation currency for this warehouse's stock (among the registered currencies).

It is not possible to change a warehouse's valuation method and currency once it has been set. If you need to change that information, you will have to recreate the warehouse, and delete the wrong one. You can only delete a warehouse if it does not contain any product anymore.

Be careful of the carriers you choose to authorize, as this will a huge impact on the order preparation in the multishipping scenario.

![](<../../../.gitbook/assets/30965769 (1).png>)

In the situation where you manage more than one shop, you will also have to associate each shop to one or more warehouses. This enables you to set from which warehouse the client orders for a given shop can be sent.

Once the warehouse has been created, you are taken back to the list of warehouses. Click the "View" icon on the right of its row to access a bird's eye view of its information, including the references of all the products stored in it, the sum of all the available quantities, a global accounting valuation, details of the stored products, and the history of the stock movements for that warehouse.

![](<../../../.gitbook/assets/23789959 (2).png>)

Each warehouse page also contains two links at the bottom:

* **See product details**. Takes you to the warehouse's "Instant Stock Status" page.
* **See warehouse's activity details**. Takes you to the warehouse's "Stock Movement" page.

## Stock management <a href="#presentingthestockmanagementinterface-stockmanagement" id="presentingthestockmanagementinterface-stockmanagement"></a>

Now that you have created one or more warehouses, you have to set stock for each of them. To that end, go to the "Stock Management" page under the "Stock" menu.

![](<../../../.gitbook/assets/23789962 (2).png>)

All available products from your catalog are listed in this interface. If you have any combination of product, you can manage them from the "Details" action.

In your daily activities, you can use this interface in order to manually:

* **Add stock**. This button adds stock for a specific product in a given warehouse.
* **Remove stock**. This button removes stock for a specific product in a given warehouse.
* **Transfer stock**. This button transfers stock from one warehouse to another.

![](<../../../.gitbook/assets/23789963 (2).png>)

The last two actions only appear if there already is some stock of the chosen product in any warehouse.\
The "Transfer stock" only appears if you have at least two registered warehouses.

### Adding stock to a warehouse <a href="#presentingthestockmanagementinterface-addingstocktoawarehouse" id="presentingthestockmanagementinterface-addingstocktoawarehouse"></a>

To add more stock to a product, use the "Add stock" action (up arrow) for said product or product combination. A new page opens, containing a form where the most important information is displayed in order to help you identify a product with certainty (reference, EAN13 and UPC code, and name). This information cannot be changed from this form, therefore it is grayed out.

![](<../../../.gitbook/assets/43089926 (1).png>)

You must then set:

* **Quantity to add**. This must be a positive number. You cannot remove stock by using a negative number.
* **Usable for sale?**. Whether that quantity of stock is usable for sale, or simply stored until you make a decision about it. In the second case, it is considered "reserved".
* **Warehouse**. The warehouse where the stock is to be added. The form lets you add product stock to only one warehouse at a time. If you need to add stock for this product in more than one warehouse, you must make the entire adding process again for each warehouse.
* **Unit price (tax excl.)**. The unit price for the product at the time of the addition. This is for valuation purpose.
* **Currency**. The currency of the unit price. If the currency is not available, you can create one from the "Currencies" page, under the "Localization" menu, or import from the "Localization" page under the "Localization" menu, by importing the localization pack of the country whose currency you want to use.
* **Label**. A label for the stock movement that you are generating, for future reference. This is purely informational.

When hovering the "Quantity to add" and "Unit price (tax excl.)" fields with the mouse cursor, the interface will display a reminder of their values the last time you added some stock.

### Removing stock from a warehouse <a href="#presentingthestockmanagementinterface-removingstockfromawarehouse" id="presentingthestockmanagementinterface-removingstockfromawarehouse"></a>

When you want to remove a certain quantity of product stock, you must use the "Remove stock" action (down arrow, available only when there already are products in stock). A new page opens, containing a form where the most important information is displayed in order to help you identify a product with certainty (reference, EAN13 and UPC code, and name). This information cannot be changed from this form, therefore it is grayed out.

You must then set:

* **Quantity to remove**. This must be a positive number. You cannot add stock by using a negative number.
* **Usable for sale**. Whether this quantity should be removed from the usable quantity or from the whole physical quantity (including the reserved one).
* **Warehouse**. From which warehouse that quantity should be removed. The form lets you remove product stock from only one warehouse at a time. If you need to remove stock for this product in more than one warehouse, you must make the entire removing process again for each warehouse.
* **Label**. A label for the stock movement that you are generating, for future reference. This is purely informational.

### Transferring stock from one warehouse to another <a href="#presentingthestockmanagementinterface-transferringstockfromonewarehousetoanother" id="presentingthestockmanagementinterface-transferringstockfromonewarehousetoanother"></a>

The stock transfer enables you to transfer stock from one warehouse to another, or from one status to another (usable in store / reserved) within a single warehouse. Click on the "Transfer stock" action (sideways arrows, available only when there already are products in stock). A new page opens, containing a form where the most important information is displayed in order to help you identify a product with certainty (reference, EAN13 and UPC code, and name). This information cannot be changed from this form, therefore it is grayed out.

You must then set:

* **Quantity to transfer**. This must be a positive number.
* **Source warehouse**. The warehouse from which you want to transfer some products, or where you want to change the status of some of the stock.
* **Is this product for sale in your source warehouse?**. Whether the quantity to remove from the "source" warehouse should be from the "usable for sale" stock or the "reserved" stock.
* **Destination warehouse**. The warehouse to which you want to transfer some products. If you simply want to change the status of some of the stock from your source warehouse, make sure to select the same warehouse in this form.
* **Is this product usable for sale in your destination warehouse?**. Whether the quantity to add to the "destination" warehouse is usable for sale or reserved. This is also the option to use when you simply want to change the status of some of the stock in the source warehouse:
  * If you do not want to change status while moving warehouses: make sure both "Use for sale?" option are set alike.
  * If you do want to change status, whether within the same warehouse or while moving warehouses: make sure both "Use for sale?" option are set differently.

For these operations, all that is related to valuations is run automatically according to the management method chosen for each warehouse. Currency conversions work the same.

## Stock Movement <a href="#presentingthestockmanagementinterface-stockmovement" id="presentingthestockmanagementinterface-stockmovement"></a>

This interface enables you to view the stock movement history. You can display all of the stock movements, or only those tied to one warehouse. Filters can be applied to refine your search.

![](<../../../.gitbook/assets/23789968 (2).png>)

When the "Filter movements by warehouse" drop-down list is set to a warehouse, you can make a CSV export of the obtained list.

## Instant Stock Status <a href="#presentingthestockmanagementinterface-instantstockstatus" id="presentingthestockmanagementinterface-instantstockstatus"></a>

This interface enables you to have an instant overview of your stock, either globally or per warehouse. The numbers are current.

![](<../../../.gitbook/assets/23789970 (2).png>)

For each product or product combination in stock, the following indicators are available:

* Unit price (tax excluded).
* Product valuation depending on the physical quantity of stock. The sum (for all prices) is not available for all warehouses, please filter by warehouse.
* Physically available stock.
* Stock that is usable for sale.
* Real quantity (physical usable quantity - client orders + supply Orders).

As appropriate, and depending on the chosen valuation method, the breakdown of the unit prices and of the associated valuations is available by clicking on the "Details" action.

Moreover, for a given warehouse, you have two ways to export the current list in CSV format:

* Export the indicators tied to the quantities.
* Export the indicators tied to the valuation (prices).

## Stock Coverage <a href="#presentingthestockmanagementinterface-stockcoverage" id="presentingthestockmanagementinterface-stockcoverage"></a>

This interface enables you to overview the coverage of your stock. The coverage indicates how many days your current stock can last. This information is very useful, as it helps you predict the necessary restocking. Coverage is calculated according to previously registered stock movements.

![](<../../../.gitbook/assets/23789971 (2).png>)

You can get the stock coverage for all the warehouses, or for a single warehouse.\
&#x20;You can also set the time period (one week, two weeks, three weeks, one month, six months, a year) of registered stock movement which is to be taken into account when calculating the coverage.\
&#x20;Finally, you can highlight the stock coverage which is below a given number of days. This will highlight the relevant products, helping you identify them quicker.

In order to view the stock coverage of product combinations, you have to click the "Details" action of the product.

It is possible to receive notifications of the stock coverage for a product. The e-mail notification module (mail alerts) can take product stock coverage into account. It is thus possible to set a number of coverage days below which you will receive a notification. See the configuration for this module.

## Supply orders <a href="#presentingthestockmanagementinterface-supplyorders" id="presentingthestockmanagementinterface-supplyorders"></a>

One of the major features of the stock manager is the ability to place orders to suppliers so as to better manage your restocking.\
&#x20;This interface enables you to manage all your supplier orders, as well as reusable order templates.

![](<../../../.gitbook/assets/23789974 (2).png>)

The order template creation process is the same as the order creation process (except for the "Expected delivery date" field). We will therefore only explain the order creation process.

### Creating a new order <a href="#presentingthestockmanagementinterface-creatinganeworder" id="presentingthestockmanagementinterface-creatinganeworder"></a>

The creation of an order for a supplier can be broken down in two steps: creating the order, then adding products to it.

![](<../../../.gitbook/assets/23789976 (2).png>)

So, the first step is to define the order's headers:

* Set the unique reference number. This is an administrative number; do not put any seemingly unique number.
* Select the supplier. If the supplier you want is not in the drop-down list, you must create it in the "Suppliers" page, under the "Catalog" menu.
* Select the warehouse which will take delivery of the order. You must have created at least one warehouse.
* Select the currency in which the order will be formalized. If needed, you can create or import a currency using, respectively, the "Currencies" or "Localization" page under the "Localization" menu.
* Select the language in which the order will be formalized. If needed, you can create or import a language using, respectively, the "Languages" or "Localization" page under the "Localization" menu.
* If needed, set the global discount on the order (in percentage). You can just leave it at "0" if you do not have a discount on this order.
* If needed, set the physical quantity of a product below which all the products have to be restocked, and are therefore to be added to the order automatically. Each pre-added product will be ordered with a quantity equal to the entered quantity, minus the already available quantity.
* Set the expected delivery date.

The second step consists of adding actual products to the order. To make that second step, you can either:

* Click on the "Save order and stay" button.
* Click on the "Save order" button. You are taken back to the list of supply orders: click on the "Edit" action for the order you just created.

The interface of the order creation form has been updated with a second form below the previously-filled fields. You must use that second form to add products to your order, using the integrated search engine. The products that you add appear in a new list.

![](<../../../.gitbook/assets/23789978 (2).png>)

For each product, you must set or update the unit purchase price (tax excluded), the quantity to order, any applicable tax rate, and any product-specific discount.

Once the order is created, it appears in the list with the "Creation in progress" status. This status enables you to view and edit the information that were previously entered as well as add products to the order. You will not be able to change the order once you change its status to "Order validated".

You can never delete a supply order: you can only cancel it.

You need to follow through for the whole order process, always indicating its status change in PrestaShop's interface. This is what the first action button of the list ("Change state") is for: click on it to reach the status changing form. See the "Changing the status of a supplier order" section below for more information on the available statuses, and see the "Registering the reception of products" to understand how to follow through on a supply order.

The "+" icon in the supply order list displays the order's history, which enables you to see who did what and when.

### Order template creation <a href="#presentingthestockmanagementinterface-ordertemplatecreation" id="presentingthestockmanagementinterface-ordertemplatecreation"></a>

The whole point of creating a template is to serve as a basis for new orders.

![](<../../../.gitbook/assets/23789980 (2).png>)

The supply order template creation process is the same as the one for a real order, except that:

* You do not have to set a planned delivery date.
* The "Automatically load products" value will be the quantity to order for the loaded products, not the stock/typed value difference.

![](<../../../.gitbook/assets/23789981 (2).png>)

Moreover, contrary to an ordinary supply order:

* A template does not have a status.
* A template can be deleted.
* A template has no edit history.

Once you have created your template, you only need to use the "Use this template to create a supply order" action from the template list (the "two windows" icon) to start creating an order.

### Changing the status of a supply order <a href="#presentingthestockmanagementinterface-changingthestatusofasupplyorder" id="presentingthestockmanagementinterface-changingthestatusofasupplyorder"></a>

Each order has many available actions (in the "Actions" column of the order list). One of them enables you to edit the status: the "Change state" one. There are six possible default statuses, but you can add your own (see the "Configuration" section of this chapter).

![](<../../../.gitbook/assets/43089928 (1).png>)

An order's status helps you understand your stock movements at a glance thanks to their color code. Here is the significance of the six default statuses:

1. **Creation in progress**. This is when you are in the first step of the creation step, where you can edit everything.
2. **Order validated**. This status validates the order and freezes the information it contains (purchase prices, quantities, etc.). At this step, a new action appears in the "Actions" column, which enables you to edit the invoice that is sent to the supplier in PDF format.
3. **Pending receipt**. As soon as the supplier has received and validated your invoice, you have to change the supply order's status to "Pending receipt".
4. **Order received in part**. As soon as a delivery is made, you must switch the order to this status. There can be multiple deliveries, and a delivery history is logged for each product. The restocking is made with each delivery.
5. **Order received completely**. Once an order is completely delivered, or partially because of a partial cancellation, it should be switched to this status. Stocks are unaffected in this case, and it is possible to perform actions on the order.
6. **Order canceled**. This status is to be given to canceled orders, whatever the reason. Stocks are unaffected in this case, and it is not possible to perform actions on the order.

With each status change, the status drop-down selector evolves in order to present only the possible status changes, in regard to the current status. The unavailable statuses are grayed out.

### Details of a supplier order <a href="#presentingthestockmanagementinterface-detailsofasupplierorder" id="presentingthestockmanagementinterface-detailsofasupplierorder"></a>

Clicking the "View" icon from the list of supply orders enables you to get a synthetic view of your order.\
You can also download the invoice generated as a PDF file (provided the order is validated by you) from the list of orders or from the status change page.

The "Details" action enables you to display the status change history for the current order.

### Registering the reception of products <a href="#presentingthestockmanagementinterface-registeringthereceptionofproducts" id="presentingthestockmanagementinterface-registeringthereceptionofproducts"></a>

You must change the status of your supply order within PrestaShop as soon as actions are taken in the real world. This is done using the "Change state" action in the "Actions" column from the list of orders. The form in this page always preselects the next logical status, but you are free to choose any of the other statuses available.

While you are preparing the supply order, keep its status to "Creation in progress". Once you are done preparing the order, switch it to "Order validated", then print the invoice PDF and send it to your supplier. As soon as your supplier confirms the reception of the invoice, change the status to "Pending receipt".

During the "Pending receipt" and "Order received in part" statuses, a new action is available in the "Actions" column. Using the "truck" icon, the "Update ongoing receipt of products" action enables you to register the reception of products for a given order during the current day.\
The form that opens after clicking that "truck" action enables you to see how many items were expected, and to indicate the quantity of product delivered for each product that day. Click the "Update selected" button to mark the selected products as received with the number of items you indicated in the "Quantity received today?" field. The checkbox on the left of each row must be checked for PrestaShop to take that line into account.

This step can be done as many times as necessary, and it is possible to receive and incorporate more stock than planned.

If you receive less stock than expected, PrestaShop automatically changes the order's status to "Order received in part".

For each product, a reception history is available ("+" action), as well as an indication of the received quantity, the expected quantity, and the remaining quantity. If the "received quantity" is equal to the "expected quantity", the corresponding row is highlighted in green. If you received more than expected, it is in red.

When all the products from the order have been received, you must manually change the supply order's status to "Order received completely". This ends the supply order process, and a new "Export" action appears, which you can use to download a CSV file of all the information pertaining to that order.

### CSV export <a href="#presentingthestockmanagementinterface-csvexport" id="presentingthestockmanagementinterface-csvexport"></a>

Using the supply orders interface, you can filter the list of orders or the details of these orders so that you may export it, according to the current filters (reference, supplier, etc.).\
&#x20;Moreover, you can choose not to display the orders that are completed or canceled, using the appropriate checkbox.

## Configuration <a href="#presentingthestockmanagementinterface-configuration" id="presentingthestockmanagementinterface-configuration"></a>

The configuration page enables you to customize the way certain parts of the advanced stock manager work:

* The available statuses for a supply order.
* The labels for the stock movements.
* The default statuses for some stock movements which are used throughout the solution.

### Adding a new default order status <a href="#presentingthestockmanagementinterface-addinganewdefaultorderstatus" id="presentingthestockmanagementinterface-addinganewdefaultorderstatus"></a>

You can add custom statuses corresponding to your business line. You cannot delete a default status.

The list on the main page enables you to get a better perspective of the available statuses, and how they can impact an order.

Click the "Add new" button to reach the creation form.

![](<../../../.gitbook/assets/23789986 (2).png>)

A status has a label, a color, and enables you to define whether:

* The order can be edited. As long as the order is editable, it cannot be sent to the supplier.
* The order delivery note can be generated.
* Product reception is ongoing, meaning that you have not yet received all the ordered products.
* Product delivery is still pending, meaning that you are still waiting for any product to arrive.

### Adding a stock movement label <a href="#presentingthestockmanagementinterface-addingastockmovementlabel" id="presentingthestockmanagementinterface-addingastockmovementlabel"></a>

It is possible to add more labels to stock movements. Click the "Add new" button from the "Stock movement labels" section to access the creation form.

![](<../../../.gitbook/assets/23789987 (2).png>)

You simply have to set a name for the label, and indicate whether it pertains to stock increase or decrease. Those labels can be used when adding/removing/transferring stock manually (as explained earlier).

### Changing default supply order labels <a href="#presentingthestockmanagementinterface-changingdefaultsupplyorderlabels" id="presentingthestockmanagementinterface-changingdefaultsupplyorderlabels"></a>

It is possible to choose the default stock movement labels in the following standard cases:

![](<../../../.gitbook/assets/23789989 (2).png>)

* Increasing stock (manually).
* Decreasing stock (manually).
* Decreasing stock following the shipment of a client order.
* Increasing stock following the delivery of products from a supplier's order.
