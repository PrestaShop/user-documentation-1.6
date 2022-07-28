# Taxes

Taxes are a complex subject, which should be fully understood as it can have a significant impact on your product prices or your shipping fees. While this user-guide is not meant to teach all the ins-and-outs of taxes, we will try our best to give you pointers.

Taxes are "compulsory contribution to state revenue, levied by the government on workers' income and business profits or added to the cost of some goods, services, and transactions". In short, every product you sell is subject to sales taxes, which depend on your state's tax laws. In effect, you contribute to your state or government functioning (public goods and services) with a percentage of all your sales, as defined by local tax rates.

There are hosts of tax rates in the World, and they vary considerably from one country to another, and even within a single country if it has federal states (USA, Germany, Spain, Russia...). You should therefore make sure to strictly conform to your country's tax laws, and even those of your state or town if they apply to you. Check with your local tax representative as soon as possible in order to get all the official details.

By default in PrestaShop, a tax applies to all countries/states/zones. If order to apply a specific tax rate for a single country or a set of countries (and not some others), you must create a tax rule. The tax rule is then applied on a per-product basis, during the creation of the product ("Prices" tab).

You cannot directly apply a tax to a product; you can only apply tax rules. Therefore, you must first register all relevant taxes, and then create a tax rule for that tax in order to specify the countries the tax applies, and finally set the tax rule to the product.

![](<../../../.gitbook/assets/23789719 (1).png>)

## Tax Options <a href="#taxes-taxoptions" id="taxes-taxoptions"></a>

At the bottom of the page is the "Tax options" section. These options apply to the whole shop, and all of the orders.

![](<../../../.gitbook/assets/23789721 (1).png>)

* **Enable tax**. Whether or not taxes are included in each purchase.
* **Display tax in shopping cart**. You might prefer the customer not to be aware of the taxes that are applied to the order. In that case, disable this option.
* **Based on**. The customer can choose to have the product not delivered at the same address as the one the order invoice should be sent to. This can have a great impact on taxes. By default, PrestaShop bases its tax rates on the delivery address, but you can choose to have them based on the billing address.
* **Use ecotax**. The ecotax refers to "taxes intended to promote ecologically sustainable activities via economic incentives". It is a tax that shop owners pay in order to "feel the social burden of their actions". Learn more about ecotax on this Wikipedia page: [http://en.wikipedia.org/wiki/Ecotax](http://en.wikipedia.org/wiki/Ecotax).\
  &#x20;Once you have enabled the use of ecotax, all your products' back office page will feature an "Eco-tax (tax incl.)" field in their "Prices" tab. You should fill that field with the exact value of the tax, which depends on your country's tax laws (it is probably based on the product's price).

If you decide to enable the ecotax after having added products, you will have to edit them all in order to set the tax properly for each product.\
&#x20;Note that if you have set ecotaxes for your products already, and that you choose to disable ecotax, then all your products will lose their ecotax settings. Re-enabling the ecotaxe will mean having to set all your products' ecotaxes again.\
&#x20;The ecotax will also appear to the customer, on the product's page.

![](<../../../.gitbook/assets/23789724 (1).png>)

## Adding a New Tax <a href="#taxes-addinganewtax" id="taxes-addinganewtax"></a>

Adding a new tax is very easy, because tax rules take out all the burden of having to specify the countries where the tax applies. The tax creation form is therefore very short:

* **Name**. Be very specific, as this will help you build tax rules faster.\
  &#x20;It is a recommended to add reminders within the name, such as the country/group/zone the tax applies to, and its rate. This greatly helps you remember which tax is to be used in a tax rule.
* **Rate**. The exact rate, in the XX.XX format.
* **Enable**. You can disable and re-enable a tax at any time.

![](<../../../.gitbook/assets/23789726 (1).png>)
