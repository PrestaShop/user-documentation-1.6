# General Concepts

## General Concepts <a href="#generalconcepts-generalconcepts" id="generalconcepts-generalconcepts"></a>

In order to avoid confusion with the classic stock management feature from version 1.4 of PrestaShop and see the possibilities offered by the advanced management feature introduced with version 1.5, you should picture two distinct concepts: product quantity available for sale, and physical products.

### Product quantity available for sale <a href="#generalconcepts-productquantityavailableforsale" id="generalconcepts-productquantityavailableforsale"></a>

This is the same as the stock management feature from PrestaShop 1.4.x. It is the product quantity that is displayed in the shop for each product and product combination. This is the quantity that defines whether the product can be ordered or not (unless the "Allow ordering of out-of-stock products" option is enabled). That quantity can be manually changed for each product and product combination.

Since PrestaShop 1.5.x, that quantity can be automatically set according to the physical stock of the affected product. In a multistore scenario, the quantity is to be defined for each shop.

Consequently, what used to be called "stock" in PrestaShop 1.4.x is called "quantity of product available for sale" since PrestaShop 1.5.x.

### Product stocks (physically stored) <a href="#generalconcepts-productstocks-physicallystored" id="generalconcepts-productstocks-physicallystored"></a>

This is the physical management of the stored products from a warehouse (or more). This is the new concept introduced as "stock" in PrestaShop 1.5.x.

This new stock management feature includes stock movement, stock valuation, stock transfer between warehouses, integration in the multistore feature and supply order management.

It also makes it possible to take into account the notion of actual stock. At a given time, a product can be available as a physical stock, but not available for sale because some client orders are still waiting for shipping. That same product can also have a supply order in progress, and thus not yet accounted for in the physical stock.

Real stock is therefore made of stock that is physically available in a warehouse, to which we add the quantity presently ordered from suppliers, and from which we subtract the quantity presently ordered by clients and which have not yet been shipped.

## Using the new stock management feature <a href="#generalconcepts-usingthenewstockmanagementfeature" id="generalconcepts-usingthenewstockmanagementfeature"></a>

### Do I have to use the new stock management feature? <a href="#generalconcepts-doihavetousethenewstockmanagementfeature" id="generalconcepts-doihavetousethenewstockmanagementfeature"></a>

There is no obligation to use the new stock management feature, just as there is no obligation to use the "quantity available for sale" management feature.

To activate both the "quantity available for sale" management feature and the stock management feature, go to the "Products" preference page, scroll down to the "Products stock" section, and choose "Yes" for the two stock management options. You have to first enable basic stock management in order to enable advanced stock management.

The advanced stock management feature, or even the standard stock management feature and your warehouses, is independent from the multistore feature. Consequently, no matter which shop you are administrating in the PrestaShop back office, when you use the "Stock" menu, you are always managing the stock in a global way.

### I do not want to change anything to my settings in PrestaShop 1.4.x/15.x. What should I do? <a href="#generalconcepts-idonotwanttochangeanythingtomysettingsinprestashop1.4.x-15.x.whatshouldido" id="generalconcepts-idonotwanttochangeanythingtomysettingsinprestashop1.4.x-15.x.whatshouldido"></a>

If you would rather not use the new advanced stock management feature from PrestaShop 1.5, and simply are satisfied with the "classic" way that PrestaShop handles product quantity management, you just have to enable the old-style stock management manager, and not the advanced stock management feature: go to the "Products" preference page, scroll down to the "Products stock" section, and choose "Yes" for the "Enable stock management" option, leaving the "Enable advanced stock management" option set to "No".

The "available for sale quantity" management feature is now centralized in the "Quantities" tab from the product sheet: create a new product or edit an existing one, and the "Quantities" tab is available on the left, among the other tabs.

### Does the new stock management feature apply to my needs? <a href="#generalconcepts-doesthenewstockmanagementfeatureapplytomyneeds" id="generalconcepts-doesthenewstockmanagementfeatureapplytomyneeds"></a>

The new stock management feature enables you to manage a stock of products. This feature applies to your business if:

* You manage a stock of products which you sell on your shop(s).
* You use at least one storage place (warehouse) which you manage yourself.
* You order most or all of your products to one or more suppliers.
* You need statistics about the state of your stock and of your warehouse(s).

This feature does not apply to your business if:

* You do not manage your stock of products yourself.
* You already use a stock management system/tool/program that you are satisfied with, and you wish to keep using it without changing anything.
