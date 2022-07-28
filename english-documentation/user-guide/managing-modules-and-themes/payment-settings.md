# Payment Settings

With PrestaShop, you can accept your customer's transactions using several different payment methods, such as checks, bank wire, cash on delivery, and through several partner modules such as PayPal, Moneybookers, HiPay, etc.

In the "Payment" page, you can see the following sections:

* **Modules list**. Basically, a shortcut to "Payments & Gateways" section of the module list, in the "Modules" page. You can install modules directly from this page.
* Three "restrictions" sections:
  * **Currency restrictions**. Choose with which currencies your installed payment modules should work.
  * **Group restrictions**. Choose with which user groups your installed payment modules should work.
  * **Country restrictions**. Choose with which countries your installed payment modules should work.

## Installing a Payment Module <a href="#paymentsettings-installingapaymentmodule" id="paymentsettings-installingapaymentmodule"></a>

Installing a payment module is fundamentally no different from installing a regular module: simply click the "Install" button, and all that is left to do is to configure the module.\
&#x20;You should pay a lot of attention to the settings, and make sure they do point to your address or bank account. Configuring payment modules often means you must first be known by the payment service provider, meaning having an account on their service.

Let's install the "Cash on Delivery" module. Find the module in the list, and click on the "Install" button. PrestaShop will take care of everything, send you to the page with the list of all modules, and notifying you of the result. For instance, if a module needs to be configured before it can work, PrestaShop will display a notification box at the top of the page. In the case of the "Cash on delivery" module, there is nothing to configure.

![](<../../../.gitbook/assets/23789661 (1).png>)

## Payment Module Restrictions on Currencies <a href="#paymentsettings-paymentmodulerestrictionsoncurrencies" id="paymentsettings-paymentmodulerestrictionsoncurrencies"></a>

Depending upon the payment, the customer's choice of currency can differ.\
&#x20;You can limit the choice of available payment methods depending on the available currencies: you may want customers to be able to pay with any currency when using PayPal, but those paying Moneybookers should only pay using dollars, for instance.

![](<../../../.gitbook/assets/23789664 (1).png>)

By default, only your shop's default currency is available. If you need more, follow this process:

1. In the "Localization" page under the "Localization" menu, import the localization pack for the country which has the currency in which you are interested. For instance, USA for US Dollars, United Kingdom for UK Pound, etc.
2. In the "Currencies" page under the "Localization" menu, enabled the currencies you just imported.

If you need to restrict payment module usage according to the user's currency, simply check the boxes that apply and click on the "Save restrictions".

Note that currency restrictions work in different ways depending on the payment module:

* For some, such as Cash on delivery, you cannot change their default setting.
* For others, such as Bank wire, Payment by check, Skrill, Ogone, etc., you can change any of their currency settings, except for the "Customer currency" and "Shop default currency", which stay at their default state.
* Then, for other modules such as Hipay or PayPal, you can change any of their currency settings, but you can choose only one option between "Customer currency" and "Shop default currency", not both.

The customer can set his or her currency using the drop-down menu at the top of each front office page.

You can set the shop's default currency in the "Localization" page, under the "Localization" menu.

If you change the default currency _after_ having configured some first products, you will have to reset the price of all these products. You should set the default currency once and for all before adding any product.

## Payment Module Restrictions on Groups <a href="#paymentsettings-paymentmodulerestrictionsongroups" id="paymentsettings-paymentmodulerestrictionsongroups"></a>

You can limit the choice of available payment methods depending on the group of customers: you can have a set number of customer groups where people can have access to more payment methods then regular customers.

![](<../../../.gitbook/assets/23789666 (1).png>)

For instance, you could choose to have regular customers pay with PayPal, Skrill and Hipay, while professionals would only be able to pay by bank wire. Depending on the type of customers and on your choices, customers will only pay using the methods that match with your decisions.

## Payment Module Restrictions on Countries <a href="#paymentsettings-paymentmodulerestrictionsoncountries" id="paymentsettings-paymentmodulerestrictionsoncountries"></a>

You can limit the choice of payment methods according to your customer's country of origin. For instance, you could choose to accept all payment methods for customers from France, Spain and Germany, while customers from Italy, the United Kingdom and Switzerland would only be able to pay by bank wire.

![](<../../../.gitbook/assets/23789668 (1).png>)

The table lists all the known countries. If one is missing, you can add it using the "Countries" page, under the "Localization" menu.

Here again, just as with currency limitations, the available options vary depending on the payment module:

* For some, the only option is your own country.
* For others, the only options are the set of countries supported by the service: Austria, Belgium, France, etc.
* All the others native payment modules should work with all countries.

Find the country you are looking for in the alphabetical list, and check the boxes to select or unselect the payment methods you want to make available to customers from that country. Once all of your settings have been configured, click on the "Save restrictions" button, found at the bottom of the table.\
&#x20;By default, all installed payment methods are enabled for the shop's country.
