# Currencies

PrestaShop can accept a large number of currencies. By default, there is only one standard currency: the one for your country. However, you must add and configure new currencies depending on your customers' needs. Indeed, customers will appreciate the ability to display your shop's prices in their country's currency.

![](<../../../.gitbook/assets/23789714 (1).png>)

The two sections at the bottom of the "Currencies" page are very simple yet essential, as relate to your currencies exchange rates (or "conversion rates"). To quote Wikipedia, "In finance, an exchange rate between two currencies is the rate at which one currency will be exchanged for another. It is also regarded as the value of one country’s currency in terms of another currency." Rates change daily, sometimes drastically depending on current events, and your shop should always be updated to the latest values.

In order to change the default currency, you must go to the "Localization" page of the "Localization" menu, and use the "Default currency" option from the "Configuration" section.\
If the currency you want to use is not available in this option, you must import the currency from one of the countries which use it, using the "Import a localization pack" section of the "Localization" page.

## Updating the Currency Rates <a href="#currencies-updatingthecurrencyrates" id="currencies-updatingthecurrencyrates"></a>

In PrestaShop, there are two ways to update your conversion rates:

* **Manually**. In the "Currency rates" section, click on the "Update currency rates" button. This will download the update file from the PrestaShop.com servers using PrestaShop web-service.
* **Automatically**. This is the recommended way. Instead of having to click on the "Update currency rates" button once or thrice a day, you can create a cron task that will trigger the rate file download as often as you feel necessary. Add the provided URL to your `crontab` file in order to activate automatic update. If you do not know what a cron task or a crontab file is, contact your hosting provider.

![](<../../../.gitbook/assets/23789715 (1).png>)

Note that the rates are provided as-is: the PrestaShop team does pay attention to have correct rates in these file, but might slightly differ from the actual ones, if only because these rates can fluctuate greatly in a short time.

## Adding a New Currency <a href="#currencies-addinganewcurrency" id="currencies-addinganewcurrency"></a>

The easiest way to add a country's currency is to import its localization package. This is done in the "Localization" page, under the "Localization" menu. Once import, you must go the "Currencies" page to enable it.

You might need to add a currency not featured in any the localization packages. In that case, you can use the creation form.

![](<../../../.gitbook/assets/23789718 (1).png>)

* **Currency**. The name of the currency, preferably in English that as many customers as possible can read it.
* **ISO code**. The currency's three-letter ISO 4217 code. See this Wikipedia page: [http://en.wikipedia.org/wiki/ISO\_4217](http://en.wikipedia.org/wiki/ISO\_4217).
* **Numeric ISO code**. Its three-digit code ISO 4217 code. Same Wikipedia page as above.
* **Symbol**. The currency's symbol, if any. See this Wikipedia page: [http://en.wikipedia.org/wiki/Currency\_sign](http://en.wikipedia.org/wiki/Currency\_sign).
* **Exchange rate** (or **Conversion rate** in earlier version). This rate is to be defined according to your shop's default currency. For example, if the default currency is the Euro and this currency is dollars, type "1.31", since 1€ usually is worth $1.31 (at the time of this writing). Use the converter here for help: [http://www.xe.com/ucc/](http://www.xe.com/ucc/).
* **Formatting**. Set up how you want your price to be displayed. The X corresponds to the currency's symbol. You have five possibilities.
* **Decimals**. You can indicate whether your shop should display decimals. While you may choose to have all your prices be a round number, discounts and other price variations might warrant decimals. You can prevent them with this option.
* **Spacing**. Once you have chosen the currency's formatting, you can choose whether to have a space character between the symbol and the price itself. Some languages require this. For instance, Spanish people would use "50€" whereas French people would use "50 €". Choose whichever you feel is best.
* **Enable**. Any currency can be disabled at any time, both from its own edit page, and the currencies table on the "Currencies" page.
* **Shop association**. You can make the currency only available to a selection of your shops, for instance shops that target a specific locale.
