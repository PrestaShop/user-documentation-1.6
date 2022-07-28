# Managing Products

## Managing Products <a href="#managingproducts-managingproducts" id="managingproducts-managingproducts"></a>

You can manage the products in your shop using the "Products" page, in the "Catalog" menu.

Sections in this chapter:

* [Managing Products](managing-products.md#ManagingProducts-ManagingProducts)
  * [The Product List](managing-products.md#ManagingProducts-TheProductList)
  * [The Product Creation Page Global Buttons](managing-products.md#ManagingProducts-TheProductCreationPageGlobalButtons)
  * [Filling out the Product Information](managing-products.md#ManagingProducts-FillingouttheProductInformation)
  * [Setting the Price of a Product](managing-products.md#ManagingProducts-SettingthePriceofaProduct)
  * [Optimizing your product's search engine position (SEO)](managing-products.md#ManagingProducts-Optimizingyourproduct'ssearchengineposition\(SEO\))
  * [Managing the Product's Associations](managing-products.md#managing-the-products-associations)
  * [Evaluating Shipping Cost: Size, Weight, Carrier](managing-products.md#ManagingProducts-EvaluatingShippingCost:Size,Weight,Carrier)
  * [Adding Product Combinations](managing-products.md#ManagingProducts-AddingProductCombinations)
  * [Managing Product Quantities](managing-products.md#ManagingProducts-ManagingProductQuantities)
  * [Configuring the Product's Images](managing-products.md#configuring-the-products-images)
  * [Configuring Product Features](managing-products.md#ManagingProducts-ConfiguringProductFeatures)
  * [Managing Customization](managing-products.md#ManagingProducts-ManagingCustomization)
  * [Managing Attachments](managing-products.md#ManagingProducts-ManagingAttachments)
  * [Setting the Product's Supplier](managing-products.md#setting-the-products-supplier)
  * [Managing Warehouses (advanced)](managing-products.md#ManagingProducts-ManagingWarehouses\(advanced\))
* [Creating a Pack of Products](managing-products.md#ManagingProducts-CreatingaPackofProducts)
  * [Pack quantities](managing-products.md#ManagingProducts-Packquantities)
* [Creating a Virtual Product](managing-products.md#ManagingProducts-CreatingaVirtualProduct)

### The Product List <a href="#managingproducts-theproductlist" id="managingproducts-theproductlist"></a>

Clicking on the "Products" option of the "Catalog" menu takes you to the list of your current products, displayed with their main details: ID, photo, name, reference, category, etc.

![](<../../../.gitbook/assets/37487185 (1).png>)

Beside the product list, this page presents you with four statistics from your store:

* Percentage of in-stock items,
* Percentage of average gross margin,
* Percentage of sales during the last 30 days,
* Number of disabled products.

The "Filter by category" option enables you to only display products pertaining to you current search, as well as reorganizing the position of products within a category.

Product position

You cannot reorganize the whole list of products. The products are displayed as is in your store (by increasing ID number), and the customer can choose the product's order using the available sorting algorithms: lowest price first, highest price first, product name A to Z, product name Z to A, in-stock first, lowest reference first, highest reference first.

You can organize products on a per-category basis by clicking on the "Filter by category" checkbox. This opens a small interface listing all your categories and sub-categories. Selecting one category automatically filters the list of products to only display products from the selected category. It also adds a "Position" column to the table, with which you can order the product on the category page. This is done either by moving the rows up and down, or by clicking the arrows.

Your product order can then be overridden by the user's sorting choice.

Note that when you change the display order in the product list in the back office (by clicking on column name's arrow in order to sort products according to that column), the "Position" column does not display arrows nor can you use it to move rows around anymore. Instead, it displays the position number of the product. In order to be able to position products again, click on the "Reset" button.

Finally, the top of the product list presents five buttons:

![](<../../../.gitbook/assets/37487181 (2).png>)

* **Add new product**. Creates a new product.
* **Export**. Downloads a CSV file of all the products in your catalog.
* **Import**. Sends you to the CSV Import option page, from where your can import your CSV files.
* **Refresh List**. Reloads the list of products to display the latest changes.
* **Show SQL Query**. Provides the SQL query to reproduce your product search or filter in your own SQL manager.
* **Export to SQL Manager**. Opens PrestaShop's SQL Manager tool (in the "Advanced Parameters") menu, from which you can query PrestaShop's database with SQL statements ("`SELECT ... FROM ... WHERE ...`").\
  If your list of product was filtered (by name, for instance), then the default SQL statement will take this into account (for instance, "``WHERE 1  AND b.`name` LIKE '%blouse%'``").

You can add new products by clicking on "Add new". A form appears, with several tabs in the left column and two buttons at the top: "Back to list" and "Help".

### The Product Creation Page Global Buttons <a href="#managingproducts-theproductcreationpageglobalbuttons" id="managingproducts-theproductcreationpageglobalbuttons"></a>

By default, the product creation page has two buttons that you will find on most the administration pages: "Recommended modules and Services" and "Help".

At the bottom of each page, there are three buttons:

* **Save**. This saves any change you have made to any of the data for the current product, and takes you back to the product list.
* **Save and stay**. This saves any change you have made to any of the data for the current product, and keeps you on the current tab. This is particularly useful when you want to switch tabs without losing your changes to the current tab, or in order to see your changes get applied immediately.
* **Cancel**. It simply takes you back to the list of product, without saving any change you have made in any of the tab from this page.

![](<../../../.gitbook/assets/23038253 (2).png>)

As soon as you give your new product a name and click on the "Save and stay" button at the bottom, more buttons appear at the top of the product page:

* **Preview**. Displays the front office page of your product. This is very handy, as it works even if the product is disabled ("Information" tab).
*   **Duplicate**. Creates an exact copy of the current product. This is very useful when you'd rather use the current product's data as a template for another new product, and not have to create every data of the new product by hand. For instance, two products might be very different, but could share the same associations, carriers or supplier settings.

    Don't over-duplicate!

    If you need to create different versions of the same product, because of its variety of colors, capacity, size, etc., then you should create product combination for the current product rather than duplicating it X times. See the "Combinations" tab on the left, which is explained in the "Adding Product Combinations" section of this chapter.
* **Product sales**. Redirects you to the "Product detail" page of the statistics dashboard ("Stats" menu), which gives you a graphic of both the visits to this product's page, and also its sales.
* **Delete this product**. Removes all the data for the current product, including its images, combinations, features, etc.
* **Recommended modules**. Opens a modal window suggesting you to install some popular modules from PrestaShop's Addons marketplace.

![](<../../../.gitbook/assets/37487187 (1).png>)

### Filling out the Product Information <a href="#managingproducts-fillingouttheproductinformation" id="managingproducts-fillingouttheproductinformation"></a>

The first tab contains the basic information about the product.

![](<../../../.gitbook/assets/37487188 (1).png>)

The first line is an essential one: indicate whether the product is a pack (a combination of at least two existing products), a virtual product (downloadable file, service, etc.), or simply a classic, mail-sent product. For now, we will only explore the classic product, and deal with packs and virtual products in their own sections of this chapter.

There are many more product-related options in the "Products" page from the "Preferences" menu:

* Number of days for which the product is considered 'new'.
* Default product order.
* Enable advanced-stock management.
* etc.

You should really check that these global settings are set as you wish.

You begin with four text fields:

*   **Name**. The first thing to complete is the product name, which will appear in the search engine results. Next to the field you will find a language code, which enables you to choose the language into which you wish to edit or create the name.

    You **must** give the product a name in at least the default language before you can save it. You won't be able to save until it has a name – and many other tabs require the product to be saved in order to be accessible.

    Make sure to translate each field in every language that your shop supports. In order to do that, click on the language code next to the field, and choose the language in which you wish to edit the text.
* **Reference code**. This is your own internal reference. It might be a number, or its reference from the storage location or its supplier, or anything that makes it unique.
* **EAN-13 or JAN barcode**. These are the numbers of the product's barcode, which are used worldwide in order to identify it. You can use either an EAN-13 or a JAN number.
  * An EAN-13 is the product's 13-digit international article number. Read more on Wikipedia: [http://en.wikipedia.org/wiki/International\_Article\_Number\_%28EAN%29](http://en.wikipedia.org/wiki/International\_Article\_Number\_\(EAN\)).
  * A JAN is specific to Japan, but is compatible with the international EAN. Read more on Wikipedia: [http://en.wikipedia.org/wiki/Japanese\_Article\_Number](http://en.wikipedia.org/wiki/Japanese\_Article\_Number).
* **UPC**. A 12-digit barcode, more widely used in North America, UK, Australia and New-Zealand. Read more on Wikipedia: [http://en.wikipedia.org/wiki/Universal\_Product\_Code](http://en.wikipedia.org/wiki/Universal\_Product\_Code).

Then come four options:

* **Enabled**. If you do not want this product to be immediately available or visible to your customers, switch the option to "No".
* **Visibility**. You can further choose to have the product available through different channels:
  * **Everywhere**. Customers can get to the product by browsing the catalog, search for the product's name, or directly using its URL.
  * **Catalog**. Customers can get to the product by browsing the catalog or directly using its URL.
  * **Search**. Customers can get to the product by searching for its name or directly using its URL.
  * **Nowhere**. Customers can only get to the product using its URL. They won't find it by browsing through the catalog or by searching for its name. This is great for creating private products, that only a few trusted visitors can access, even temporarily (you can change this setting at any time).
* **Options**. A couple of specific options.
  * **Available for order**. If you uncheck this box, customers will not be able to add this product to their cart. This makes it more like a single-product Catalog mode (in comparison with the "Catalog mode" preference).
  * **Show price**. If the "available for order" option above is unchecked, you can either choose to display the product's price nevertheless (even though visitors won't be able to buy it), or choose to not display it.
  * **Online only (not sold in store)**. If your business does have brick-and-mortar stores, this option will prove invaluable when a product is only sold online, not in store – this prevents customers from checking a product price online, then come to your store hoping to buy it directly, and thus avoid shipping cost.
* **Condition**. Not all shops sell new product. This option enables you to indicate the condition of the product:
  * **New**. The product is brand new, sealed in its original packaging.
  * **Used**. The product has been sold at least once before, and probably used by someone else (second hand). It should come in its original packaging, which might be closed with tape.
  * **Refurbished**. The product has been returned for various reasons ("scratches, dents or other forms of cosmetic damage which do not affect the performance of the unit"). Read more on Wikipedia: [http://en.wikipedia.org/wiki/Refurbishment\_%28electronics%29](http://en.wikipedia.org/wiki/Refurbishment\_\(electronics\)).

Now that these details are set in stone, you can start adding a description for your product.\
&#x20;Describing your product well is essential, both for the customer (the more information, the better) and search engines (it will help your shop appear in more search requests).

![](<../../../.gitbook/assets/23038447 (2).png>)

At the bottom of the screen, the two description fields each serve different purposes:

* The **"Short description" field** enables you to write a short description that will appear in search engines and in the category description for your product.\
  This field is limited to 400 characters by default: if you exceed that limit, PrestaShop will warn you with a message in red below the field. You can change that limit in the "Products" preference page, where you will find the "Max size of short description" option.
* The **"Description" field** enables you to write a full description of your product, which will appear directly on the product page. The text editor offers a wide range of options for creating visually attractive descriptions (font, size, text color, etc.).\
  &#x20;While the second field has no limits, there is such thing as too much content: strive to provide the essential information in a compelling way, and your product should be good to go.

Below the "Description" field, you can find a small tool to add one of the images you attached to the product (through the "Images" tab) to the "Description", using image tags. Click on "Click here" to open it.

![](<../../../.gitbook/assets/23038449 (2).png>)

Simply select the image you want, choose its position according to the text and its size, and PrestaShop will generate an image tag which you can then put right into the description (preferably between two paragraphs, or at the very beginning of a paragraph).

In the **"Tags" field**, add some terms and keywords that will help your customers easily find what they are looking for.

![](<../../../.gitbook/assets/23038459 (2).png>)

They are displayed on the store in the "Tags" block (if available). If you do not want the tag block displayed, simply disable the "Tags block" module (in the "Modules" page).

Differences with PrestaShop 1.4

PrestaShop 1.4 enabled you to indicate the product's manufacturer right in this tab. Since version 1.5, this setting is to be found in the "Associations" tab on the left. Same for the "Default category" field, the associated categories, and the "Accessories" field.

Version 1.4 also enabled you to indicate the size and weight of the final package. Since version 1.5, these settings are to be found in the "Shipping" tab on the left.

The "Location" field of version 1.4 can be found in the optional "Warehouses" tab on the left, which is only available if you have enabled Advanced Stock Management ("Preferences" menu, "Products" page, "Products stock" section).

Once you have filled out all this information, save your work, after which you will be sent to your list of products. If you save by clicking on "Save and Stay", you will be able to continue working on your product's presentation.

### Setting the Price of a Product <a href="#managingproducts-settingthepriceofaproduct" id="managingproducts-settingthepriceofaproduct"></a>

This is all done in the "Prices" tab on the left. The pricing section can be quite intimidating, with fields influencing each other and taxes to take into account – but it is in fact quite simple.

![](<../../../.gitbook/assets/30245485 (2).png>)

Set the price that will appear in your store by following the instructions below:

* **Wholesale price**. Enables you to instantly know your wholesale, factory price, and thus compare it to your selling price in order to easily calculate your profit.
* **Retail price**. The price of your product before taxes.
* **Tax rule**. The tax applicable to the product. Choose between the different rates that you have registered.\
  &#x20;If you need to create new tax rates, click the "Create New Tax" button. Tax creation is done in the "Localization" menu, "Taxes" page; it is fully explained in the "Understanding Local Settings" chapter of this guide.
* **Eco-tax (tax incl.)**. The value of the ecotax for this product. This value is already included in your retail price. You are supposed to declare that tax to your country's tax agency.\
  &#x20;_Note that this field is not displayed by default_. If you have to include an ecotax, you must first enable it: go to the "Localization" menu, "Taxes" page, "Tax options" section (bottom of the page), and choose "Yes" for the "Use ecotax" option.
* **Retail price with tax**. Displays the price of the product with taxes included. You can edit the value, and it will automatically update the "Pre-tax retail price" field according to the tax rule that you chose.
* **Unit price**. Enables you to conform to local legislations that require products to be displayed with their unit price.\
  &#x20;For instance, if you are selling a pack of 6 cans of soda, then you should fill this field with the price per can, and indicate "can" in the text field. The description on the same line will update accordingly.
* **Display the "on sale" icon on the product page and in the text found within the product listing**. Check that box to show that your product is on sale, both on the product page and in the text on the product listing. An "On sale" icon will appear under the product. You can modify this logo by changing the following file: `themes/default/img/onsale_en.gif`
* **Final retail price**. This price, including the discount taken, will update as you type.

You can fill out the "retail price with tax" field and choose the tax rate to apply, and the field will automatically calculate the pre-tax retail price. The opposite operation is also available.

At this point, you are done with the essential information for a basic product page. You can save it and have it immediately available for sale on your shop!\
&#x20;But keep reading, as there are many more details you can add to your product to make it more attractive to customers.

#### Specific prices: Managing Quantity Discounts <a href="#managingproducts-specificprices-managingquantitydiscounts" id="managingproducts-specificprices-managingquantitydiscounts"></a>

You can changes the total price of the product depending on the quantity of products your customer buys, the user group, the country, etc. This is done with the "Specific prices" section of the "Prices" tab. Click on the "Add a new specific price" button to reveal the creation form.

![](<../../../.gitbook/assets/23038463 (2).png>)

This is a very easy way to create a discount price for this product (and all its combinations).

Click "Add a New specific price", and a form appears.

* **For**. This enables you to be very specific about the various groups to which this price applies, including currencies, countries and even your customer groups (which we'll discuss in a later chapter).
* **Customer**. You can choose to be even more specific and directly set at who the discount you are creating is targeted. Start typing the first letters of the clients' first name or last name, and select the ones you want.
* **Combination**. You can choose to have this specific price apply to all of the product's combinations, or only one. If you wish to apply to more than one combination but not all of them, you will have to create a specific price for each combination.
* **Available from/to**. Here you can define a range of dates between which the discount price is active. Clicking each selector will open a calendar, simplifying the process.
* **Starting at \[] unit**. Contains the value from which the discount should be applied. Default is "1", which means any quantity.
* **Product price (tax excl.)**. This is where you can set an arbitrary price, independent of calculations and regular prices. Keep this field at "0" to use the default price.\
  **Leave base price**. Check this box to reset the "Product price" field and prevent yourself from editing it.
* **Apply a discount of**. The discount that will be applied once the client has chosen a quantity of product. Use the selector to set the type of discount (either a specific amount in the default currency, or a percentage of the default price).

Once you have chosen your values click on "Save and stay": the summary of your discount settings appears below. The discount will be immediately visible on the store.\
If you wish to delete a value, click on the trashcan icon in the table.

If you want to build more complex discounts, go read about the "Price rules" menu in the "Creating Price Rules and Vouchers" chapter of this guide.

#### Managing Price Priority <a href="#managingproducts-managingpricepriority" id="managingproducts-managingpricepriority"></a>

A customer might fit into multiple prices or discount rules, even when you have set detailed prices and quantity discounts, with custom groups and shops (if in a multistore context). PrestaShop therefore uses a set of priorities in order to apply a single price rule to such customers. You might want the user group to be more important than the currency, for instance.

You can change PrestaShop default settings using the "Priority Management" section.

![](<../../../.gitbook/assets/23038464 (2).png>)

The default order of importance is:

1. Shop (when in a multistore context).
2. Currency.
3. Country.
4. Group.

A checkbox at the bottom enables you to update the settings for all products. If the checkbox remains unchecked, then your changes only apply to the current product.

### Optimizing your product's search engine position (SEO) <a href="#managingproducts-optimizingyourproductssearchengineposition-seo" id="managingproducts-optimizingyourproductssearchengineposition-seo"></a>

To improve your product listing as well as increase your store's visibility we suggest that you carefully fill out the various SEO fields: meta titles, meta descriptions, and keywords and friendly URLs.

"SEO" itself stands for "Search Engine Optimization. Read more on Wikipedia: [http://en.wikipedia.org/wiki/Search\_engine\_optimization](http://en.wikipedia.org/wiki/Search\_engine\_optimization)

Get to know the best SEO practices for e-commerce! Download and read PrestaShop's free "Complete Guide to SEO": [http://www.prestashop.com/en/white-paper-seo](http://www.prestashop.com/en/white-paper-seo)

To access the product's SEO information, open the "SEO" tab on the left.

![](<../../../.gitbook/assets/23038467 (2).png>)

The fields in this page enable you to directly optimize your catalog's visibility on search engines.

* **Meta title**. This is the most important field, as the title that will appear on all search engines. Be very factual: you must convince the search engine user to click your link, not one from another site. Make sure the title is unique to this product within your site.
  * Good example: "Levi's 501® Original Jeans - Tidal Blue - Original Fit".
  * Bad example: "Item #02769869B bestseller".
* **Meta description**. A presentation of the product in just a couple lines (ideally, less than 155 characters), intended to capture a customer's interest. This will appear in results for some search engines, depending on the search request: some search engine might choose to display the searched keywords directly in the context of the page content. Make sure the description is unique to this product within your site.
* **Friendly URL**. This is another extremely important field. It enables you to rewrite the web addresses of your products as you wish. For example, instead of having an address such as\
  &#x20;[http://www.myprestashop.prestashop.com/index.php?id\_product=8\&controller=product](http://www.myprestashop.prestashop.com/index.php?id\_product=8\&controller=product)\
  &#x20;you can have:\
  &#x20;[http://www.myprestashop.prestashop.com/8-name-of-the-product.html](http://www.myprestashop.prestashop.com/8-name-of-the-product.html).\
  &#x20;All you need to do is indicate in the "Friendly URL" field the words that you wish to see appear instead of the default name, separated by dashes.\
  &#x20;The "**Generate**" button makes it easy to produce a proper friendly URL based on the product name. Once generated, you can edit the URL produced if necessary.

Friendly URLs will only work if URL rewriting is enabled. You can do this in "SEO & URLs" preference page, in its "Set up URLs" section.

You will find more information on the "SEO & URLs" preference page in the "Understanding the Preferences" chapter of this guide.

### Managing the Product's Associations

Creating associations for your product means pairing it with other content in your database:

* Product categories.
* Other products (accessories).
* Manufacturer.

![](<../../../.gitbook/assets/23038469 (2).png>)

#### Product categories <a href="#managingproducts-productcategories" id="managingproducts-productcategories"></a>

The "Associated categories" section enables you to select in which category the product should appear. You can select more than one, but keep in mind that it is better for the customer if the category only contains equivalent and comparable products. Therefore, you should prevent from selecting root categories, and prefer child categories.\
&#x20;For instance, the "telephone" category can feature sub-categories of "brands" (Apple, Samsung, Nokia, etc.) and as well as "characteristics" (smart-phone, flip-phone, etc.). It is up to you to indicate the category most useful to your customers.\
&#x20;If you feel you need to add a category, save the current state of your product before clicking the "Create new category" button. Category creation is explained in another section of this guide.

The "Default category" selector is useful when an article is filed under several categories. It serves mainly to clarify which category to use in case your customer arrives at your site from a search engine, since the name of the category will appear in the product's URL.

Featured List

Checking the "Home" box enables you to highlight the product on your shop's homepage, provided your theme supports it. To remove a product from the Featured list, simply uncheck the "Home" box.

#### Accessories <a href="#managingproducts-accessories" id="managingproducts-accessories"></a>

The "Accessories" field gives you the option of choosing relevant products to associate with this product, to suggest them to your customers when the visit the product's page (if the theme supports it). Type in the first letters of product and select it. The product is then added at the bottom of the field.

![](<../../../.gitbook/assets/23038470 (2).png>)

You can associate a product with as many other products as you deem necessary. Click on the cross to delete the product association.\
&#x20;An association goes one way only: the associated product will not feature an association to the current product in its setting page.

Accessories addition/removal is not automatically saved! Do not forget to click on the "Save" button.

#### Manufacturer <a href="#managingproducts-manufacturer" id="managingproducts-manufacturer"></a>

A product can only be associated with one manufacturer. Choose one in the dropdown menu, or create a new manufacturer if it is needed (but do save your current product before clicking the "Create a new manufacturer" link).

### Evaluating Shipping Cost: Size, Weight, Carrier <a href="#managingproducts-evaluatingshippingcost-size-weight-carrier" id="managingproducts-evaluatingshippingcost-size-weight-carrier"></a>

Shipping costs are not be neglected: they can easily double the final cost of an order, and you should be very upfront about them – customers hate bad surprises.

![](<../../../.gitbook/assets/23038472 (2).png>)

The "Shipping" tab on the left enables you to give some precious details about your product's package:

*   **Package width, height, depth & weight**. You should strive to fill each field, because knowing the exact size and weight of a package is not only useful to you, but PrestaShop can also direct specific sizes/weights to specific carriers automatically, based on these settings. The order's final price will appear to the customer once PrestaShop (or the customer) has selected a carrier.

    These values use the default weight, volume, distance and dimension units, as set in the "Localization" page of the "Localization" menu.

    These values do not have to be integers. If your products weight less than 1 lbs, you can simply use a period (.) to indicate the fractions:

    * 123 lbs
    * 1.23 lbs
    * 0.23 lbs (equals 3.68 oz)
    * etc.
* **Additional shipping fees**. This can prove very useful to you for specific products that are particularly tricky to package, or really heavy.
* **Carriers**. You can choose to have the current product only be shipped by a selection of carriers. If no carrier is selected then all the carriers will be available for customer orders.

### Adding Product Combinations <a href="#managingproducts-addingproductcombinations" id="managingproducts-addingproductcombinations"></a>

You will often sell the same product under different versions: they share the same overall name, but they might differ by their color, their capacity, their screen size, and other attributes. Most of the time, these attributes come together: you could have the red version of the product available with either 1 Gb capacity or 2 Gb, or with 12'' screen or a 15'' screen. This is why PrestaShop calls these versions "combinations": your stock of products can be made of several variations of a single product, which in effect are simply its attributes combined in specific ways.

You cannot create combinations if you do not already have product attributes properly set in PrestaShop.\
&#x20;Also, you should not create combination for features that your customers should not be able to choose from.

Attributes creation is done in the "Product Attributes" page from the "Catalog" menu, and is explained in details in the chapter of the same name of this guide.

![](<../../../.gitbook/assets/23038474 (2).png>)

How your product attributes are combined into combinations is up to you, and PrestaShop gives you two methods to achieve this.

#### Manual method <a href="#managingproducts-manualmethod" id="managingproducts-manualmethod"></a>

This method helps you create combinations one after the other. Therefore, it is to be reserved to either products with few combinations, or products with very specific combinations that can't be created reliably using the automatic method (see next section).

![](<../../../.gitbook/assets/23038476 (2).png>)

Adding a new variation to your product takes just a few steps. Click on the "New Combination" button at the bottom of the page, next to the "Save" buttons. A form appears:

* **Attribute-value pair**.
  1. From the drop-down menu, choose a group of attributes, such as "Color" for example. The content of the "Value" dropdown list updates accordingly.
  2. Choose the attribute value that you would like to include, for example "Blue".
  3. Click on the "Add" button and it will appear in the selector.\
     &#x20;You can add as many attribute-value pairs as necessary to one combination.\
     &#x20;You can only add one pair per attribute to one combination: it is impossible to have both "Color: Blue" and "Color: Red" in your pairs; if this is necessary, you will have to create new attributes, for instance "Primary color" and "Secondary color".\
     &#x20;You can delete an attribute-value pair by selecting it and clicking on the "Delete" button.
* **Reference, EAN-13 & UPC**. If necessary, indicate the combination's reference, EAN-13 and/or UPC numbers into each field, as if you were creating a brand new product in PrestaShop. These numbers may be used by your warehouse or your carrier, so make sure to fill these fields, they are often essential to your business.
* **Wholesale price**. This field is useful if the original price of the product changes simply because this is a combination.
* **Impact on price/weight/unit price**. If the combination is supposed to have an impact on the product's original price/weight/unit price, choose the appropriate dropdown menu, select "Increase" or "Reduction" depending on the context, and fill the field that appears with the value of that impact.
* **Ecotax**. The specific ecotax for this combination (if the ecotax option is enabled).
* **Minimum quantity**. You might prefer this combination to only be sold in bulk. Use this field to set the number of items to be sold in bulk.
* **Available date**. If this product is out of stock, you can indicate when the product will be available again.
* **Image**. The images that are linked to the original product (as uploaded using the form in the "Images" tab on the left) are displayed. Check the box for the images that best represent this combination.
* **Default**. Check this box if you want the combination you are creating to actually be the main one for this product.

When you have set all of the combination's details, save your product changes using the "Save and stay" button. Your combination will appear in the attributes list at the bottom of the screen.

Differences with PrestaShop 1.4

In PrestaShop 1.4, there used to be a "Color picker" form at the bottom of the list of combinations, where you could choose to display a color picker or not on the product page.

Since PrestaShop 1.5, this option has been moved and improved. When creating a new attribute (in the "Catalog" menu, "Attributes & Values" page), you can use the "Attribute type" drop-down list to choose whether the front-page should display it as a drop-down list, a radio button list, or a color picker.

#### Automatic method <a href="#managingproducts-automaticmethod" id="managingproducts-automaticmethod"></a>

If you have too many different products versions or varieties, you can use the "Product Combinations Generator." This tool allows you to automatically generate all of the combinations and possibilities.

Clicking the "Product combinations generator" takes you to the complete form.

![](<../../../.gitbook/assets/23038478 (2).png>)

A warning window might appear, saying "You will lose all unsaved modifications. Are you sure that you'd like to proceed?" This means your product already had some combinations created. If you agree to this, this will delete the combinations that have not yet been saved. Be careful, and always save your work before using the generator!

On the left side of this page are your attributes and their values. Select the combinations by clicking on the value names (if want to select more than one value, hold the Ctrl key while clicking), then click on "Add".\
&#x20;For example, you might select the "Blue", "S, M, L" values.\
To remove an existing attribute selection, simply select their values and click on "Delete".

Once the varieties have been selected, you can edit the impact on product price and on product weight for each selection. You do not have to: they might simply be the same price and weight.\
Insert the quantity of each product in the "Default quantity" field at the bottom. **Be careful, it needs to be the same for every combination.** For instance, 200 products in each combination = 2 colors \* 1 size \* 200 = 400 items in all.\
&#x20;You may add a default reference for this combination if it serves your administrative needs.\
&#x20;Click the "Generate these Combinations" button, and PrestaShop sends you back to the "Combinations" tab, with all the generated combinations. If you need to, you can now edit them one by one.

As you can see, the combination generator helps you save a lot of time when you have numerous attributes to assemble, such as sizes and materials. It automatically creates **all of the possible combinations**, which will then appear under the product's public page, in the "Combinations" tab (if the theme supports it).\
&#x20;If you do not want to keep all generated combinations or if they are in fact not all exactly the same (different references, prices, available dates...), you can delete them (trashcan icon) or modify them (file icon) from the product's combination list. The star icon turns the selected combination into the default one – in which case it is highlighted in blue.

### Managing Product Quantities <a href="#managingproducts-managingproductquantities" id="managingproducts-managingproductquantities"></a>

Product quantities are managed in a single tab. The way it works is quite easy: the page presents you with a table of all the combinations for the current product (if there are no combinations, the table simply has a single row). It is up to you to set the initial stock for all the combinations. PrestaShop will use this to determine when a product is soon out-of-stock or unavailable anymore.

#### Stock Management Options <a href="#managingproducts-stockmanagementoptions" id="managingproducts-stockmanagementoptions"></a>

The quantities tab supports the advanced stock management feature, if activated. This means that if the current product's combinations are distributed among several storage locations, PrestaShop is able to handle the exact location of each combination, even within a given warehouse.

![](<../../../.gitbook/assets/23038481 (2).png>)

By default, you have to manage the current product's quantities by hand, for each combination, from this page. With the advanced stock management feature activated, you can rely on PrestaShop's stock management feature to handle this.

To use advanced stock management for the current product, checking the box for "I want to use the advanced stock management system for this product". Once this is done, an option becomes available: "Available quantities for current product and its combinations are based on warehouse stock". Click it, and you cannot edit the current product's quantities from the "Quantities" page anymore: it has new become dependent of your stock management.

#### When out of stock <a href="#managingproducts-whenoutofstock" id="managingproducts-whenoutofstock"></a>

The "When out of stock" option enables you to set PrestaShop behavior when the product is out of stock: deny orders (the product is not available for sale anymore) or allow order (in essence, you are doing pre-sales). The third and default option simple uses the global default setting ("Preferences" menu, "Products" page, "Product Stock" section, "Allow ordering of out-of-stock products" option).

#### Availability Settings <a href="#managingproducts-availabilitysettings" id="managingproducts-availabilitysettings"></a>

At the bottom of the page, you can set the exact behavior of PrestaShop depending on the availability of the current product.

![](<../../../.gitbook/assets/23038483 (2).png>)

The options are:

* **Displayed text when in-stock**. Enables you to display a message to your visitors when your product is in stock, for example "Item available". It reassures them that your shop can immediately send them the product.
* **Displayed text when allowed to be back-ordered**. Enables you to display a message to your visitors when your product is out of stock but they can still order it (as set using the "**When out of stock**" selector), for example "Pre-order now!". It reassures them that your shop will send them the product immediately once it is in stock.

You can also configure the general settings applied to all of your products: the default option is to deny orders, but this can be modified under the "Products" preference ("Allow ordering of out-of-stock products" option), which is fully explained in the "Understanding the Preferences" chapter of this guide.

### Configuring the Product's Images

The "Images" tab on the left is for including photos on your product page. You should upload all the images for this product, including all of its combinations (color, size, shape, etc.).

![](<../../../.gitbook/assets/30245486 (2).png>)

To add one or more images to your product:

1. Click the "Add files" button and then select at least one image file from your computer to upload. You can select as many images as necessary by keeping the Ctrl-key pressed while selecting files, or you can make your selection one by one. PrestaShop will display the chosen images in a list, with their size and a button to remove some.\
   &#x20;The default maximal size for an image file is set by PrestaShop according to your server's PHP settings. This size can be lowered in the "Images" preference page, "Product images" section.
2. Give the image a caption. It will be displayed if the image cannot be displayed – which can be very good for your search engine optimization.
3. Click on the upload button to put your file online.
4. The uploaded images appear in a table below the button. If you have more than one image, you can choose which image is to be used as the default/cover image by clicking on the red "no entry" button and turn it into a checkmark. That cover image will also appear automatically on the product page of your shop.\
   You can click on a thumbnail to display the image in full size.

Once you have uploaded all your product images, you can modify the image order by drag-and-dropping each table row when the mouse cursor changes to a "movable" cursor.

### Configuring Product Features <a href="#managingproducts-configuringproductfeatures" id="managingproducts-configuringproductfeatures"></a>

The "Features" tab is where you specify your products' features (i.e. weight, material, country of origin, etc.).

![](<../../../.gitbook/assets/23038519 (2).png>)

When you create features and values (i.e. wool knit and micro-fiber materials), you assign them to the products when it is appropriate. This means that you do not have to fill out the features fields for each of your products but instead simply fill in the necessary values and apply them later.

PrestaShop's comparison engine relies entirely on product features: this is what gets compared.

Also, since product comparison works on a per-category basis, you should make sure that all the products in a given category do share the same features, with various values to be compared between each other.

Be aware that **contrary to the combinations, these values do not change, and are valid for the general product** (meaning: all your combinations will share these same features).

#### Creating a feature <a href="#managingproducts-creatingafeature" id="managingproducts-creatingafeature"></a>

Before adding a feature to a product, you must create it for general use in your shop. You either go to the "Features" page of the "Catalog" menu, or directly click on the "Add a new feature" button. A warning will appear, "You will lose all unsaved modifications. Are you sure that you'd like to proceed?" – make sure all your changes are saved before validating.

Feature and feature value creation are explained in details in the dedicated section of the guide.

#### Assigning a value and feature to a product <a href="#managingproducts-assigningavalueandfeaturetoaproduct" id="managingproducts-assigningavalueandfeaturetoaproduct"></a>

We will assume here that you have already set all your features and feature values.

In the current product's "Features" tab on the left, a table is displayed, listing all of your shop's features. Not all of them pertain to this product: PrestaShop will only take as relevant the features where you actually set a value.

You can either set a value manually, in the field on the far right a feature's row, or you can use one of the pre-defined values (as set when creating the feature) if there are any available.\
&#x20;If no value is available for a feature, the mention "N/A" appears (short for "not available" or "not applicable"), followed by a "Add pre-defined values first" button.

If you choose to use a custom value, do not forget to set it for every language that your shop supports. Use the language code selector to change language.

If there are pre-defined values available, they will appear in a dropdown list. Simply click it and choose the correct value.

Once you have set all the relevant features, save your changes to see them immediately applied in the front-page.

Remember: If a feature does not have any value assigned to it, it will not be taken into account for this product, and will not be visible on your shop.

### Managing Customization <a href="#managingproducts-managingcustomization" id="managingproducts-managingcustomization"></a>

PrestaShop makes it possible for your customers to customize the product that they will buy.

Example: You are a jewelry retailer and your customers have the possibility to engrave their jewelry with a text or an image. Your customers can submit the text and/or the image when they place their order.

The advantage of this function is that it offers your customers a personal service, which they will without a doubt appreciate!

Let's look at how to configure this function. In the "Customization" tab on the left, you can indicate what type of context (file and/or text) can be personalized.

![](<../../../.gitbook/assets/23038520 (2).png>)

* **File fields**. Puts the indicated number of file upload buttons on the order page. Each button accepts only one file, so put as many field as you allow your customers to upload.
* **Text fields**. Puts the indicated number of text fields on the order page. You can add as many text fields as necessary.\
  &#x20;Example: If you allow your customer to use a 5-line text with each line limited to 14 characters, you can add 5 fields and indicate the number of allowed characters in the field's label. You cannot limit the number of characters in the string.

Once you have added the needed number for each field, click "Save and stay". The page will reload and display as many text fields as necessary. Fill every one of them with the appropriate public label: this will be an indicator for the customer, so be very specific about what you expect.

For instance, if you allow images for a book cover, you could use the following:

* "Front cover (20.95 x 27.31 cm, color)".
* "Back cover (20.95 x 27.31 cm, black and white)".
* "Spine (20.95 x 1.716 cm, color)".

Same for text: if customers can engrave words to a product, you could use the following:

* "First line (24 chars)".
* "Second line (24 chars)".
* "Last line, signature (16 chars)".

**Removing fields**. If in the end you added too many fields, simply change the number of needed fields for each of the two types and click "Save and stay". The page will reload with the right number of fields, with the first ones preserved.

Once all the label fields have been filled, do not forget to save your changes.

#### On the customer's side <a href="#managingproducts-onthecustomersside" id="managingproducts-onthecustomersside"></a>

Once a product has customizable properties set, its front-end product page has a new tab, next to the "More info" tab: "Product customization".

The customer must choose the file(s) and/or add some text and save them before they add the product in the cart.

The custom image(s) and text(s) will appear in the final cart.

The rest of the purchase process is the same as usual.

#### On the merchant's side <a href="#managingproducts-onthemerchantsside" id="managingproducts-onthemerchantsside"></a>

Once the order has been validated by the customer, the merchant gets a notification of the order in the back office.

He can then check on the order, which will indicate the image(s) and the text(s) in the list of products, for each product. The merchant then simply has to download the image(s) (simply by clicking on the image in the order) or copy/paste the text and use that in its customization tool.

The rest of the order and delivery process is the same as usual.

### Managing Attachments <a href="#managingproducts-managingattachments" id="managingproducts-managingattachments"></a>

PrestaShop enables you to make some files available to your customers before their purchase. This is done in the "Attachments" tab on the left.

![](<../../../.gitbook/assets/23038523 (2).png>)

For example, let's say you sell electronics, and you would like to urge your customers to read a document on how a product works. You can upload a document for that purpose.\
&#x20;You could also simply have the product's PDF manual directly available for download right on the product page.

Adding an attachment is really quick:

1. Fill out the file name of your attachment (it doesn't have to be the same as the original file name).
2. Give it a description. This will help you distinguish between your uploaded files with certainty.
3. Click on "Add file" to select a file on your computer to upload. As soon as you choose the file, PrestaShop uploads it, then displays it in the list
4. The attachment appears in the "Available attachments" list: you have to select it then click on the "Add" to move it to the "Attachments for this product" list.
5. Save your product with either the "Save" button or the "Save and stay" one.

Now the "Download" tab will appear on the product's page (if the theme supports it), and your customers can download the file(s) that you just uploaded.

If you need to remove an attachment, select it in the "Attachments for this product" selector and click on the "<- Remove" button. The file will be moved to the "Available attachments" selector if you need to set it back online later on.

You can view all of your store's attached files, add some more and remove some, by going to the "Attachments" page under the "Catalog" menu. This also makes it possible to use the attachments that you already uploaded for other files: if you need to apply the associated one file with many products, you will thus only have to upload it once.

### Setting the Product's Supplier

Indicating the product's supplier is not really important to your customers (very much less so than its manufacturer in any case), but it may turn out to be an essential part of your own internal management, not the least when managing your stock: you simply need to know who you bought the product from. The supplier of the current product is to be set from the "Suppliers" tab on the left.

![](<../../../.gitbook/assets/23038526 (2).png>)

You cannot use this feature if you do not already have at least one supplier registered in your shop. Suppliers are created from the "Suppliers" page, under the "Catalog" menu.

The complete supplier registration process in explained in details in the current chapter of this guide.\
&#x20;You can access the creation page directly by clicking on the "Create a new supplier" button.

Associating the current product with one or more suppliers is really easy: simply click the box corresponding to the supplier, and save your changes.

If the product is associated with more than one supplier, you can choose which one should be the default one using the radio button on the right.\
&#x20;Note: the "Default" radio buttons are unavailable by default. In order to select them, you must first click the "Save and stay" button" in order to select another supplier as default.

#### Product reference(s) <a href="#managingproducts-productreference-s" id="managingproducts-productreference-s"></a>

The product's supplier page also features a table that enables you to set the precise reference and unit price/currency for each product combination. If the product has more than one supplier, the table only opens the combination tied to the first supplier, the others being closed by default. Click on a supplier's name in order to open its references table, and close the others.

![](<../../../.gitbook/assets/23038527 (2).png>)

### Managing Warehouses (advanced) <a href="#managingproducts-managingwarehouses-advanced" id="managingproducts-managingwarehouses-advanced"></a>

Once you have enabled the advanced stock management option (in the "Products" preference page), this new tab gets available for all products, and enables you to indicate in which warehouse the current product is stored.

![](<../../../.gitbook/assets/23038528 (2).png>)

You cannot use this feature if you do not already have at least one warehouse registered in your shop. Warehouses are created from the "Warehouses" page, under the "Stock" menu.

The complete warehouse registration process in explained in details in another chapter of this guide, "Managing Stock".\
&#x20;You can access the creation form by clicking on the "Create a new warehouse" button.

The "Warehouses" tab presents you with a table that enables you to set the precise location for each product combination (if any) in each warehouse. If you have registered more than one warehouse, the table only shows the first one by default, the others being closed by default. Click on a warehouse's name in order to open its sub-table, and close the others.

For each warehouse, you can set which combination of the current product is stored, and a text field enables you to indicate precisely where it is stored in that warehouse. You can write anything in that field: "Aisle 5", "Next to the Radiohead albums", "A07 E08 H14", or anything that helps you or your packaging team to find the product as quickly as possible.

## Creating a Pack of Products <a href="#managingproducts-creatingapackofproducts" id="managingproducts-creatingapackofproducts"></a>

You may wish to sell a pack of products made of several items. I.e.: a computer start-up pack composed of the computer itself, a monitor, and a printer. PrestaShop makes it easy for you to create a "pack" product and add other products from your catalog to this pack.

Packs enable you to simplify preparing orders. They also allow customers to take advantage of special prices and offers.

You cannot currently add combinations or virtual products to a pack.\
&#x20;If you need to have packs with combinations, you will have to create single products for each combination. This is a known limitation that will be fixed in a coming version of PrestaShop.

You cannot add an existing pack within a new pack, or import the content of an existing pack into a new pack.

The process to create a pack is similar to the one for creating a regular product:

1. Go to the "Products" page, under the "Catalog" menu.
2. Click the "Add New" button.
3. From the "Information" tab on the left, change the product type to "Pack of existing products ".

Below the "Type" option, a new section will appear. It only features two text fields and a button:

* The first field is used to search for products that are already registered in your shop.
* The second field is used to indicate the quantity of chosen product should be added to the pack.
* The button adds the product to the pack.

![](<../../../.gitbook/assets/23038531 (2).png>)

You can add as many products as you would like to the pack.

You can remove a product from the pack simply by clicking the trashcan icon next to it.

A new option will also appear in the "Quantities tab": it is to help you manage your pack quantities.

### Pack quantities <a href="#managingproducts-packquantities" id="managingproducts-packquantities"></a>

When you are creating a pack of products, PrestaShop needs to know how to handle the stock. In the "Quantities" tab, under "Pack quantities", you must choose one of the following options:

* **Decrement pack only** (default behavior). When a pack is sold, only the stock for the pack will be impacted.
* **Decrement products in pack only**. When a pack is sold, only the stock for each product will be impacted.
* **Decrement both**. When a pack is sold, both the stock for the pack and the stock for each product will be impacted.
* **Default behavior**. This is the default behavior as set at the shop level in your Product preferences. By default you will have "Decrement pack only" but it will change according to your choice.

Once you are done with the "Pack", you can edit the content of all the other available tabs as if you would for a regular product.

## Creating a Virtual Product <a href="#managingproducts-creatingavirtualproduct" id="managingproducts-creatingavirtualproduct"></a>

Your shop may feature (partly or exclusively) virtual products – that is, products that are not shipped, but rather downloaded: entertainment tickets, e-books/PDF files, real-life services...\
&#x20;PrestaShop makes it easy for you to create a virtual product

The process to do this is similar to the one for creating a simple product:

* Go to the "Products" page, under the "Catalog" menu.
* Click the "Add New" button.
* From the "Information" tab on the left, change the product type to "Virtual Product".

The tabs on the left change:

* The "Virtual Product" tab appears, to which you will be redirected as soon as you change the product type.
* The "Shipping product" tab disappears.

The new tab only features one option at first: it asks if the virtual product you are creating has a file attached (i.e., if your customer will pay to download something).

* If not, leave it at that: you are selling a service, and nothing needs to be downloaded.
* If yes, click the "Yes" option.

![](<../../../.gitbook/assets/37487192 (1).png>)

When you click "Yes", PrestaShop opens a new form within the tab, from which you can upload the file you intend to sell:

* **Filename**. The name of the file. This field is automatically filled after the file has been uploaded. It is not recommended to change it to another value.
*   **File**. Click the "Browse" button to find the file on your hard drive. As soon as you have selected a file, the upload begins.

    The maximum file-upload size setting depends on your server's settings, and cannot be increased from PrestaShop.

    If you have access to your server's `php.ini` file, these are the values you should change:

    * `upload_max_filesize = 20M`
    * `post_max_size = 20M`

    If you do not have access to the `php.ini` file, contact your web host about this.

    You should compress your file in zip format, in order to avoid the browser misinterpreting `.exe` or `.jpg` file formats. Browsers automatically download zip files for the customer, no question asked.

    If you are selling a high resolution image, uploading it using this form does not prevent you from uploading its thumbnail in the "Images" tab on the left.
* **Number of allowed downloads**. You can set the number of time the file can be downloaded once the customer has bought it. You might prefer to limit this to 1, or 5. If you want to keep it unlimited, set the text field to 0.
* **Expiration date**. Virtual files can be of promotional nature, or lose their selling value after a certain date. If so, you can set the expiry date after which the product will not be available on your shop anymore. Leave it blank if there is no expiry date.
* **Number of days**. You can set the number of days after which the download link becomes non-functioning. If there is no limit, set the text field to 0.

Once you are done with the "Virtual Product" tab, you can edit all the other available tabs as if you would for a regular product.
