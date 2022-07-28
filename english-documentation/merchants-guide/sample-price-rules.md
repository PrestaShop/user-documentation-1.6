# Sample price rules

**Table of contents**

* [Sample price rules](sample-price-rules.md#Samplepricerules-Samplepricerules)
  * [10% off for all products on the store](sample-price-rules.md#Samplepricerules-10%offforallproductsonthestore)
  * [10% off for all products in a given category](sample-price-rules.md#Samplepricerules-10%offforallproductsinagivencategory)
  * [10% off for a specific product](sample-price-rules.md#Samplepricerules-10%offforaspecificproduct)
  * [10% off for a specific product when the customer orders 5 of this product](sample-price-rules.md#Samplepricerules-10%offforaspecificproductwhenthecustomerorders5ofthisproduct)
  * [10% off for a specific product for the first 50 customers](sample-price-rules.md#Samplepricerules-10%offforaspecificproductforthefirst50customers)
  * [Buy 1, Get 1 Free](sample-price-rules.md#Samplepricerules-Buy1,Get1Free)
  * [Buy 4, get the 5th one free](sample-price-rules.md#Samplepricerules-Buy4,getthe5thonefree)
  * [Buy one, get two free](sample-price-rules.md#Samplepricerules-Buyone,gettwofree)
  * [Free shipping on any order](sample-price-rules.md#Samplepricerules-Freeshippingonanyorder)
  * [Free shipping on orders over $20](sample-price-rules.md#Samplepricerules-Freeshippingonordersover$20)

## Sample price rules <a href="#samplepricerules-samplepricerules" id="samplepricerules-samplepricerules"></a>

The Price Rules menu contains two incredibly powerful tools to create automated discounts and vouchers: the cart rule generator and the catalog price rule generator. Both are powerful, but they can be complex to master. There is a wide variety of rules you could want to implement on your stores, either temporarily or permanently. The most obvious rules are a breeze to set up, but the real power of the Price Rules tools lies in their details.

This page explores a dozen of rules which will certainly help you get a better grip of these tools, and might inspire you to come up with your own.

Before you read these explanations, you should brush up on your knowledge of the price rule generators: [https://app.gitbook.com/@prestashop/s/prestashop-1-5-documentations/english-documentation/user-guide/creating-price-rules-and-vouchers#CreatingPriceRulesandVouchers-CreatingPriceRulesandVouchers](https://app.gitbook.com/@prestashop/s/prestashop-1-5-documentations/english-documentation/user-guide/creating-price-rules-and-vouchers#CreatingPriceRulesandVouchers-CreatingPriceRulesandVouchers)

The gist of it is:

* Use the Catalog Price Rules generator to create discounts that will apply on the product sheet
* Use the Cart Rules generator to create discounts and vouchers that will apply once the customer views the content of his/her cart.

In short, create a catalog price rule to build discount prices that the customer will see right away ; create a cart rule to build a discount that the customer will only see when viewing the content of the cart, or vouchers that the customer will be able to apply to cart using a code.

Another aspect to remember is this:

* Catalog Price Rules can only reduce the price of a product or a set of products (fixed amount or percentage).
* Cart Rules can reduce the price of a product or the whole cart (fixed amount, percentage, cheapest product), offer free shipping, and add a free gift to the order.

To create a new catalog price rule, go to the "Price Rules" menu, open the "Catalog Price Rules" page, and then click on the "Add New" button.\
&#x20;To create a new cart rule, go to the "Price Rules" menu, open the "Cart Rules" page, and then click on the "Add New" button.

### 10% off for all products on the store <a href="#samplepricerules-10-offforallproductsonthestore" id="samplepricerules-10-offforallproductsonthestore"></a>

To lower the price by the same percentage for ALL products on your store, you can either create a catalog price rule or a cart rule.

#### Catalog price rule <a href="#samplepricerules-catalogpricerule" id="samplepricerules-catalogpricerule"></a>

* Enter a name, choose "Percentage" as the reduction type, and type "10.00" in the "Reduction" field.
* Do not add any condition: the price rule will apply to all products in all categories.

Save your settings. The discount is immediately applied.

#### Cart rule <a href="#samplepricerules-cartrule" id="samplepricerules-cartrule"></a>

* Information tab: Enter a name and description. If you want the discount to depend on the customer entering the correct code, enter that code in the "Code" field.
* Conditions tab: Do not change anything. Of course, you can limit the discount to a certain customer, or during a certain time frame.
* Actions tab: Choose "Percent" in the "Apply a discount" option. Enter "10" in the "Value" field.

Save your settings. The discount is immediately applied.

### 10% off for all products in a given category <a href="#samplepricerules-10-offforallproductsinagivencategory" id="samplepricerules-10-offforallproductsinagivencategory"></a>

To lower the price by the same percentage for all products of a specific category, you can either create a catalog price rule or a cart rule.

#### Catalog price rule <a href="#samplepricerules-catalogpricerule.1" id="samplepricerules-catalogpricerule.1"></a>

* Enter a name, choose "Percentage" as the reduction type, and type "10.00" in the "Reduction" field.
* In the "Conditions" section, choose a category and click "Add condition".

Save your settings. The discount is immediately applied.

#### Cart rule <a href="#samplepricerules-cartrule.1" id="samplepricerules-cartrule.1"></a>

* Information tab: Enter a name and description. If you want the discount to depend on the customer entering the correct code, enter that code in the "Code" field.
* Conditions tab:
  1. Check the "Product selection" box at the bottom.
  2. Click the "Product selection" link that appears.
  3. Choose "Add a rule concerning Categories", click OK.
  4. Click the "Choose" button. In the interface that appears, choose a category in the "Unselected" section on the left, and click the "Add" button so as to move that category in the "Selected" section on the right. Once all the proper categories are chosen, click to cross at the top right of the interface, or press the Escape key.
* Actions tab: Choose "Percent" in the "Apply a discount" option. Enter "10" in the "Value" field.

Save your settings. The discount is immediately applied.

### 10% off for a specific product <a href="#samplepricerules-10-offforaspecificproduct" id="samplepricerules-10-offforaspecificproduct"></a>

#### Cart rule <a href="#samplepricerules-cartrule.2" id="samplepricerules-cartrule.2"></a>

To lower the price by the same percentage for a product or a selection of products, you must create a cart rule.

* Information tab: Enter a name and description. If you want the discount to depend on the customer entering the correct code, enter that code in the "Code" field.
* Conditions tab:
  1. Check the "Product selection" box at the bottom.
  2. Click the "Product selection" link that appears.
  3. Choose "Add a rule concerning Products", click OK.
  4. Click the "Choose" button. In the interface that appears, choose one or more products in the "Unselected" section on the left, and click the "Add" button so as to move them in the "Selected" section on the right. Once all the proper products are chosen, click to cross at the top right of the interface, or press the Escape key.
* Actions tab: Choose "Percent" in the "Apply a discount" option. Enter "10" in the "Value" field.

Save your settings. The discount is immediately applied.

#### Catalog price rule <a href="#samplepricerules-catalogpricerule.2" id="samplepricerules-catalogpricerule.2"></a>

You could also use a catalog price rule, with a bit of cheating. Caution: this can have unpredictable side-effects!

* Enter a name, choose "Percentage" as the reduction type, and type "10.00" in the "Reduction" field.
* In the "Conditions" section, you cannot choose a product, but you can limit the rule's application to a manufacturer and product-specific attributes and features, if any. If the product has several versions/editions depending on its attributes, you must create a new condition group for each attribute in order to cover all bases.

Save your settings. The discount is immediately applied.

#### Specific product price <a href="#samplepricerules-specificproductprice" id="samplepricerules-specificproductprice"></a>

This is not a "price rule" per se, but it works just as well. Everything is done in the product's page within the store's catalog, not in any of the "price rule" generators.

Once in the product's configuration page, open the "Prices" tab on the left, and click "Add a new specific price" in the "Specific prices" section. A form opens. You can change everything in that form in order to make the discount availability even more specific, but if you simply want to make it available to all, just change the value of the "Apply a discount of" option to 10, and indicate that is a percentage.

Save your settings. The discount is immediately applied.

### 10% off for a specific product when the customer orders 5 of this product <a href="#samplepricerules-10-offforaspecificproductwhenthecustomerorders5ofthisproduct" id="samplepricerules-10-offforaspecificproductwhenthecustomerorders5ofthisproduct"></a>

#### Cart rule <a href="#samplepricerules-cartrule.3" id="samplepricerules-cartrule.3"></a>

To lower the price by the same percentage for a product or a selection of products if and only if the customer buys at least 5 if these products, you must create a cart rule.

* Information tab: Enter a name and description. If you want the discount to depend on the customer entering the correct code, enter that code in the "Code" field.
* Conditions tab:
  1. Check the "Product selection" box at the bottom.
  2. Click the "Product selection" link that appears.
  3. Select "The cart must contain at least 5 Product(s)".
  4. Choose "Add a rule concerning Products", click OK.
  5. Click the "Choose" button. In the interface that appears, choose one or more products in the "Unselected" section on the left, and click the "Add" button so as to move them in the "Selected" section on the right. Once all the proper products are chosen, click to cross at the top right of the interface, or press the Escape key.
* Actions tab: Choose "Percent" in the "Apply a discount" option. Enter "10" in the "Value" field.

Save your settings. The discount is immediately applied.

#### Catalog price rule <a href="#samplepricerules-catalogpricerule.3" id="samplepricerules-catalogpricerule.3"></a>

You could also use a catalog price rule, with a bit of cheating. Caution: this can have unpredictable side-effects!

* Enter a name, choose "Percentage" as the reduction type, and type "10.00" in the "Reduction" field.
* Put "5" in the "From quantity" field.
* In the "Conditions" section, you cannot choose a product, but you can limit the rule's application to a manufacturer and product-specific attributes and features, if any. If the product has several versions/editions depending on its attributes, you must create a new condition group for each attribute in order to cover all bases.

Save your settings. The discount is immediately applied.

#### Specific product price <a href="#samplepricerules-specificproductprice.1" id="samplepricerules-specificproductprice.1"></a>

This is not a "price rule" per se, but it works just as well. Everything is done in the product's page within the store's catalog, not in any of the "price rule" generators.

Once in the product's configuration page, open the "Prices" tab on the left, and click "Add a new specific price" in the "Specific prices" section. A form opens. You can change everything in that form in order to make the discount availability even more specific, but if you simply want to make it available to all, just change the value of the "Starting at" option to 5 and change the value of the "Apply a discount of" option to 10, and indicate that is a percentage.

Save your settings. The discount is immediately applied.

### 10% off for a specific product for the first 50 customers <a href="#samplepricerules-10-offforaspecificproductforthefirst50customers" id="samplepricerules-10-offforaspecificproductforthefirst50customers"></a>

To lower the price of a specific product one a first-come first-served basis, you must create a cart rule:

* Information tab: Enter a name and description. If you want the discount to depend on the customer entering the correct code, enter that code in the "Code" field.
* Conditions tab:
  1. Enter "50" in the "Total available" option. Leave "1" in the "Total available for each user" option, so that a single customer can only use this promotion once.
  2. Check the "Product selection" box at the bottom.
  3. Click the "Product selection" link that appears.
  4. Choose "Add a rule concerning Products", click OK.
  5. Click the "Choose" button. In the interface that appears, choose one or more products in the "Unselected" section on the left, and click the "Add" button so as to move them in the "Selected" section on the right. Once all the proper products are chosen, click to cross at the top right of the interface, or press the Escape key.
* Actions tab:\

  1. Choose "Percent" in the "Apply a discount" option. Enter "10" in the "Value" field.
  2. Select "Specific product" in the "Apply a discount to" option and find the product you chose in Conditions tab.

Save your settings. The discount is immediately applied.

### Buy 1, Get 1 Free <a href="#samplepricerules-buy1-get1free" id="samplepricerules-buy1-get1free"></a>

This is a classic. So many online and real-life store use it, it actually has its own Wikipedia page ([http://en.wikipedia.org/wiki/Buy\_one,\_get\_one\_free](http://en.wikipedia.org/wiki/Buy\_one,\_get\_one\_free)), and an acronym: BOGO (or BOGOF). This is a very effective way to promote your products.

#### Cart rule, "50% discount" way <a href="#samplepricerules-cartrule-50-discount-way" id="samplepricerules-cartrule-50-discount-way"></a>

Offering a second product when the customer buys one product is akin to giving a 50% discount when the customer buys two of a product. To do this, you must create a cart rule.

* Information tab: Enter a name and description. If you want the discount to depend on the customer entering the correct code, enter that code in the "Code" field.
* Conditions tab:
  1. Check the "Product selection" box at the bottom.
  2. Click the "Product selection" link that appears.
  3. Select "The cart must contain at least 2 Product(s)".
  4. Choose "Add a rule concerning Products", click OK.
  5. Click the "Choose" button. In the interface that appears, choose a single product in the "Unselected" section on the left, and click the "Add" button so as to move the product in the "Selected" section on the right. Once the proper product is chosen, click to cross at the top right of the interface, or press the Escape key.
* Actions tab: Choose "Percent" in the "Apply a discount" option. Enter "50" in the "Value" field.

Save your settings. The discount is immediately applied.

#### Cart rule, per-product 50% way <a href="#samplepricerules-cartrule-per-product50-way" id="samplepricerules-cartrule-per-product50-way"></a>

You can also create a per-product cart rule. The rule will only apply to a single product, so if you want your customer to be able to get the "buy one get one free" discount on several products, you will have to create as many cart rules. If you want your whole catalog to respect this discount, you will have to create rules for everyone single one of your products.

* Information tab: Enter a name and description. If you want the discount to depend on the customer entering the correct code, enter that code in the "Code" field.
* Conditions tab:
  1. Check the "Product selection" box at the bottom.
  2. Click the "Product selection" link that appears.
  3. Select "The cart must contain at least 2 Product(s)".
  4. Choose "Add a rule concerning Products", click OK.
  5. Click the "Choose" button. In the interface that appears, choose a single product in the "Unselected" section on the left, and click the "Add" button so as to move the product in the "Selected" section on the right. Once the proper product is chosen, click to cross at the top right of the interface, or press the Escape key.
* Actions tab: Choose "Percent" in the "Apply a discount" option. Enter "50" in the "Value" field.

Save your settings. The discount is immediately applied.

#### Cart rule, per-product gifting way <a href="#samplepricerules-cartrule-per-productgiftingway" id="samplepricerules-cartrule-per-productgiftingway"></a>

You can also use the per-product gifting way, where you choose to offer a free gift (of the same product) instead of applying a 50% discount for 2 purchases of the same product.

* Information tab: Enter a name and description. If you want the discount to depend on the customer entering the correct code, enter that code in the "Code" field.
* Conditions tab:
  1. Check the "Product selection" box at the bottom.
  2. Click the "Product selection" link that appears.
  3. Choose "Add a rule concerning Products", click OK.
  4. Click the "Choose" button. In the interface that appears, choose a single product in the "Unselected" section on the left, and click the "Add" button so as to move the product in the "Selected" section on the right. Once the proper product is chosen, click to cross at the top right of the interface, or press the Escape key.
* Actions tab: Choose "Send a free gift" and find the same product.

Save your settings. The discount is immediately applied.

### Buy 4, get the 5th one free <a href="#samplepricerules-buy4-getthe5thonefree" id="samplepricerules-buy4-getthe5thonefree"></a>

The "Buy one, get one free" promotion is well-known, but you can do any variation of "Buy X, get X+1".

#### Cart rule, per-product gifting way <a href="#samplepricerules-cartrule-per-productgiftingway.1" id="samplepricerules-cartrule-per-productgiftingway.1"></a>

* Information tab: Enter a name and description. If you want the discount to depend on the customer entering the correct code, enter that code in the "Code" field.
* Conditions tab:
  1. Check the "Product selection" box at the bottom.
  2. Click the "Product selection" link that appears.
  3. Select "The cart must contain at least 4 Product(s)".
  4. Choose "Add a rule concerning Products", click OK.
  5. Click the "Choose" button. In the interface that appears, choose a single product in the "Unselected" section on the left, and click the "Add" button so as to move the product in the "Selected" section on the right. Once the proper product is chosen, click to cross at the top right of the interface, or press the Escape key.
* Actions tab: Choose "Send a free gift" and find the same product.

Save your settings. The discount is immediately applied.

#### Cart rule, percentage way <a href="#samplepricerules-cartrule-percentageway" id="samplepricerules-cartrule-percentageway"></a>

This variation is a little twisted. We apply a 20% discount on a single product once it reaches 5 in the cart. That 20% off of 5 products means that one of the products is free.

In effect, this rule is giving 20% to the product once the cart reaches at least 5 of this product. So if the customer buys 6, the 20% discount will be applied to the whole 6 items rather than the 5 first ones. We therefore do not recommend this method.

* Information tab: Enter a name and description. If you want the discount to depend on the customer entering the correct code, enter that code in the "Code" field.
* Conditions tab:
  1. Check the "Product selection" box at the bottom.
  2. Click the "Product selection" link that appears.
  3. Select "The cart must contain at least 5 Product(s)".
  4. Choose "Add a rule concerning Products", click OK.
  5. Click the "Choose" button. In the interface that appears, choose a single product in the "Unselected" section on the left, and click the "Add" button so as to move the product in the "Selected" section on the right. Once the proper product is chosen, click to cross at the top right of the interface, or press the Escape key.
* Actions tab:
  1. Choose "Percent" in the "Apply a discount" option, and enter "20" in the "Value" field.
  2. Choose "Specific product" in the "Apply a discount to", and find the product.

Save your settings. The discount is immediately applied.

### Buy one, get two free <a href="#samplepricerules-buyone-gettwofree" id="samplepricerules-buyone-gettwofree"></a>

The easiest way to give two products when one is bought is to create a pack of the two offered product, and then create a cart rule to give that pack along the purchase.

* Information tab: Enter a name and description. If you want the discount to depend on the customer entering the correct code, enter that code in the "Code" field.
* Conditions tab:
  1. Check the "Product selection" box at the bottom.
  2. Click the "Product selection" link that appears.
  3. Choose "Add a rule concerning Products", click OK.
  4. Click the "Choose" button. In the interface that appears, choose a single product in the "Unselected" section on the left, and click the "Add" button so as to move the product in the "Selected" section on the right. Once the proper product is chosen, click to cross at the top right of the interface, or press the Escape key.
* Actions tab: Choose "Send a free gift" and find the pack.

Save your settings. The discount is immediately applied – provided the pack has some quantity available for sale!

### Free shipping on any order <a href="#samplepricerules-freeshippingonanyorder" id="samplepricerules-freeshippingonanyorder"></a>

Offering free shipping for everyone is easy. Simply create a cart rule:

* Information tab: Enter a name and description. If you want the discount to depend on the customer entering the correct code, enter that code in the "Code" field.
* Conditions tab: Do no touch anything.
* Actions tab: Choose "Free shipping".

Save your settings. The discount is immediately applied – for every order! Make sure to limit this discount in time, or to a given number of customers ("Total available" option in the Conditions tab)!

### Free shipping on orders over $20 <a href="#samplepricerules-freeshippingonordersoverusd20" id="samplepricerules-freeshippingonordersoverusd20"></a>

Offering free shipping for any order above a set amount is also easy. Simply create a cart rule:

* Information tab: Enter a name and description. If you want the discount to depend on the customer entering the correct code, enter that code in the "Code" field.
* Conditions tab: Enter "20" in the "Minimum amount" option (make sure that you are using the correct currency).
* Actions tab: Choose "Free shipping".

Save your settings. The discount is immediately applied – for every order! Make sure to limit this discount in time, or to a given number of customers ("Total available" option in the Conditions tab)!
