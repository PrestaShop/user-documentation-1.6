# Shipping and Logistics modules

## Carrier Compare <a href="#shippingandlogisticsmodules-carriercompare" id="shippingandlogisticsmodules-carriercompare"></a>

This module enables the customer to compare carrier possibilities before continuing with the checkout process.

This module is very straightforward: just install it to display its option on your front office.

All the available carriers must have their fees properly set. This is done at the bottom "Shipping" page, in the "Fees by carrier, geographical zone, and ranges".

The module configuration page only has one option, "Refresh carrier list method". This enables you to display a carrier either only when all the information is set, or at any time.

## Date of Delivery <a href="#shippingandlogisticsmodules-dateofdelivery" id="shippingandlogisticsmodules-dateofdelivery"></a>

This module displays an approximate date of delivery during the checkout process.

The configuration page has two sections:

* **Carrier configuration**. The module relies on indications from your carriers. You must therefore add rules for each of your carriers, by clicking on the "Add a new carrier rule" link.
* **Settings**:
  * **Extra time when a product is out of stock**. Estimate the time it might take for your team to re-stock products. This is only useful if customers can order out-of-stock products (the option for this is in the "Products" preference page, in the "Products stock" section).
  * **Extra time for preparation of the order**. Estimate the time it might take for your team to prepare an order.
  * **Preparation option**. If your packaging team also works on weekends, indicate it, as the module takes this into account.
  * **Date format**. The format in which the expected delivery date is displayed. It uses PHP `date()` format: each letter has a meaning, as explained in the indicated link. The default, "l j F Y", means the date will be displayed in the format "Saturday 21 January 2012". There are many more parameters that you can use to build the date format as you see fit: see [http://www.php.net/manual/en/function.date.php](http://www.php.net/manual/en/function.date.php).

Adding a new carrier rule is pretty straightforward:

* **Carrier**. Choose the carrier for which you want to add the rule. If the wanted carrier is not there, you must create it in the Shipping > Carriers page.
* **Delivery between**. Set the timeframe in which the chosen carrier promises to deliver products. You have to gather this information from the carrier itself.
* **Preparation options**. Some carriers also prepare their packages on weekend days, so as to send them first thing on Monday morning. Be sure to indicate it if so.

You should create as many carrier rules as necessary.

## Fedex (fedexcarrier) <a href="#shippingandlogisticsmodules-fedex-fedexcarrier" id="shippingandlogisticsmodules-fedex-fedexcarrier"></a>

Offer your customers, different delivery methods with Fedex

## Globkurier <a href="#shippingandlogisticsmodules-globkurier" id="shippingandlogisticsmodules-globkurier"></a>

**Poland only.**

![](<../../../.gitbook/assets/23036725 (4).png>)

GlobKurier.pl is one of the biggest national leaders in delivering shipments. We provide domestic and international services to more than 200 countries. Our main aims are competitive price, speed and security. With GlobKurier.pl you can be sure that your shipments always come on time. Moreover we offer convenience of using our services.

## GoInterpay <a href="#shippingandlogisticsmodules-gointerpay" id="shippingandlogisticsmodules-gointerpay"></a>

![](<../../../.gitbook/assets/23038228 (3).png>)

Bring over 200 payment methods to your checkout with one simple integration.

## Kiala Advanced (Kiala contract holders only) <a href="#shippingandlogisticsmodules-kialaadvanced-kialacontractholdersonly" id="shippingandlogisticsmodules-kialaadvanced-kialacontractholdersonly"></a>

This module makes it possible for your customers to have their parcels delivered in a Kiala collection point. Kiala points are widely available in France, and also in other select European countries.

You must have a Kiala account in order to use this module. You can reach the sign-up form here: [http://www.kiala.com/](http://www.kiala.com/).\
&#x20;Then, configure the module with all the information about you and your shop in the form in the "Kiala Module Status" section.\
&#x20;The "Country settings" section further down helps you indicate in which countries you want to make Kiala delivery available for your customers.\
&#x20;Finally, the "Kiala advanced settings" section adds a few more options:

* **Export folder**. The local folder where the module will save its export, containing a lot of useful information.
* **Prefix for order and parcel number**. You can have a shop-specific prefix for your shop, which make it look more personalized for your customers.
* **Export on each order?**. You may prefer to have several order-specific export files rather than a big one.
* **Parcel tracking criterion?**. Should the parcel be tracked on a per-customer or a per-order basis? If you are unsure, keep it to per-order.

Once the settings are in place, your customers will see the "Kiala" option appear in the shop's front office as part of the available delivery methods.

## Mondial Relay <a href="#shippingandlogisticsmodules-mondialrelay" id="shippingandlogisticsmodules-mondialrelay"></a>

This module enables you to display rates for delivering in Mondial Relay points. This service is available in France, Luxembourg, Spain and Belgium.

You must have a Mondial Relay account in order to use this service. You can reach the sign-up form here: [http://www.mondialrelay.com/](http://www.mondialrelay.com/).\
&#x20;Then, from the module's configuration page, click on the "Account details" icon and enter the necessary information, as provided by Mondial Relay: Webservice Enseigne, Code marque, Webservice Key, Etiquette's Language and Weight Coefficient. The Etiquette's Language can only use the languages that are enabled on your shop; you can enable more language from the "Languages" page, under the "Localization" menu. Click "Update Settings" in order to connect your shop to the Mondial Relay webservice, and from there on, follow the module's instructions in the "Shipping" and "Advanced settings" screens.

Once the settings are in place, your customers will see the "Mondial Relay" option appear in the shop's front office as part of the available delivery methods.

## So Colissimo <a href="#shippingandlogisticsmodules-socolissimo" id="shippingandlogisticsmodules-socolissimo"></a>

This module enables you to display rates for deliveries via SoColissimo, a service by La Poste, France's historical postal service. This service is available mainly in France.

You must have a SoColissimo account in order to use this module. This is done by calling La Poste from a French phone, using this number: **3634**.\
&#x20;Then, configure the module with your SoColissimo information: ID So, key, preparation time, overcost, URL So, Fancybox, Supervision and Supervision URL.\
&#x20;A full documentation is available (in French) as a PDF file, which you can find under the "Documentation" link on the configuration page.

In order to finalize the installation, copy/paste the two final URLs in your SoColissimo back office.

Once the settings are in place, your customers will see the "SoColissimo" option appear in the shop's front office as part of the available delivery methods.

## TNT Express France <a href="#shippingandlogisticsmodules-tntexpressfrance" id="shippingandlogisticsmodules-tntexpressfrance"></a>

**France only.**

This module enables you to display rates for deliveries via TNT express services. This service is available worldwide.

You must have a TNT account in order to use this module. You can reach the sign-up form here: [http://www.tnt.com](http://www.tnt.com).\
&#x20;Then, configure the module with your TNT login, password and account number, all in the "Account settings" tab.\
&#x20;From there on, you can keep configuring the module using the "Shipping Settings" and "Service Settings" tabs. This last tab enables you to be very specific about the delivery service you want to make available for your customers, as well as any additional charge you might require depending on the package's weight.

Once the settings are in place, your customers will see the "TNT Express France" option appear in the shop's front office as part of the available delivery methods.

## Tracking - Front office <a href="#shippingandlogisticsmodules-tracking-frontoffice" id="shippingandlogisticsmodules-tracking-frontoffice"></a>

This module completes PrestaShop with an integrated affiliate program feature, which enables your affiliates to access their own statistics.

The affiliate program tool is located in the "Referrers" page, under the "Stats" menu. Once you have installed the "Tracking - Front office" module, these affiliates can access their statistics by going to [http://www.example.com/modules/trackingfront/stats.php](http://www.example.com/modules/trackingfront/stats.php).

To create a new affiliate, click the "Add new" button, and in the creation form, add the affiliate account username and password, then specify the fee they receive per click, per order and per percentage of sales.

Click on the header of the "Help" section to display instructions on how to set up the referrer URLs.

The "Technical information - Expert mode" enables you to use regular expression instead of plain text URLs.

## UPS <a href="#shippingandlogisticsmodules-ups" id="shippingandlogisticsmodules-ups"></a>

Offer your customers, different delivery methods with UPS

## USPS <a href="#shippingandlogisticsmodules-usps" id="shippingandlogisticsmodules-usps"></a>

Calculates shipping rates for United States Postal Service for Domestic shipping within the USA
