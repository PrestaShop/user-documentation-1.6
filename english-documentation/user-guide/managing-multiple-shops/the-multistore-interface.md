# The multistore interface

## Managing your stores <a href="#themultistoreinterface-managingyourstores" id="themultistoreinterface-managingyourstores"></a>

The "Multistore" page comprises three mains sections:

* **Multistore tree**. Gives you a bird's eye view of your shop groups, their shops, and even the various URLs tied to a single shop.\
  &#x20;By default, there is only one shop, in the default group: the main shop.
* **Shop groups** table. Lists the available shop groups. You can edit them by click on the 'edit' icon on the right.
* **Multistore options**. Lists the available options for the existing shops.
  * **Default shop**. The default shop is the one which will serve a central hub for all the other ones, shares its details with other shops (products, carriers, etc.), and is the one that appears when you log in the administration.

![](<../../../.gitbook/assets/23789996 (1).png>)

## One back office to rule them all <a href="#themultistoreinterface-onebackofficetorulethemall" id="themultistoreinterface-onebackofficetorulethemall"></a>

When the multistore feature is enabled for your PrestaShop installation, many aspects of PrestaShop become customizable on a per-shop or per-shop-group basis.

To help you understand which shop your changes are applied to, PrestaShop adds a dropdown selector at the top of each screen, where you can choose the scope of application of your changes:

* Apply to all of your shops on this installation of PrestaShop.
* Apply to only the shops of the selected shop group.
* Apply to only the selected shop.

![](<../../../.gitbook/assets/23789992 (1).png>)

This shop selector helps you know on which shop(s) you are currently working.

That being said, once the multistore mode is in place, many of the regular settings can only be changed on a global (all shops) scale (most notably the settings pages: localization, preferences, advanced preferences, administration) and will therefore present the options as disabled in any other selection. Still, you can choose to edit those settings on a more local (per group shop or even per shop) scale if it is needed.

Indeed, settings pages will look regular when the shop selector is on "All shops", while in any other selection (shop group or single shop) they get additional options:

* A "Yes/No" option at the top of each section of the settings page.
* A check box next to each option.

![](<../../../.gitbook/assets/25722904 (2).png>)

They both serve the same purpose: letting you enable the options that would otherwise be disabled in the current shop context. You can pick the options that you want to enable, or you can enable all the options of the section by switching the Yes/No option. Once enabled, it is up to you to change the value of each options: clicking the checkbox or switching the Yes/No option does not change any settings, it just allows you to change it in that context.

Nevertheless, some options cannot be edited on a local context: they will display "You can't change the value of this configuration field in the context of this shop."

The following table indicates whether the item can also be customized for a single shop, for a group of shops, or for all shops at once.

| Item                                                                                                                                                                                                                                  | Per shop | Per shop group | All shops |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------- | -------------- | --------- |
| Employees                                                                                                                                                                                                                             | X        | X              | X         |
| Customer groups                                                                                                                                                                                                                       | X        | X              | X         |
| Products                                                                                                                                                                                                                              | X        | X              | X         |
| — Prices                                                                                                                                                                                                                              | X        | X              | X         |
| — Combinations and prices                                                                                                                                                                                                             | X        | X              | X         |
| — Languages                                                                                                                                                                                                                           | X        | X              | X         |
| — Multiple images (**except for the main image**)                                                                                                                                                                                     | X        | X              | X         |
| <p>— Available quantity for sale, provided that:</p><ul><li>The "Share quantity available for sale" option is checked for the group,</li><li>The group does not share its quantity available for sale outside of the group.</li></ul> | X        | X              |           |
| — All other information (description, tags, friendly URL, etc.)                                                                                                                                                                       | X        | X              | X         |
| Catalog values and attributes                                                                                                                                                                                                         | X        | X              | X         |
| Discounts: cart rules                                                                                                                                                                                                                 | X        |                |           |
| Discounts: catalog price rules                                                                                                                                                                                                        | X        |                |           |
| Taxes: tax rules                                                                                                                                                                                                                      | X        | X              | X         |
| Categories (**except for the main image**)                                                                                                                                                                                            | X        | X              | X         |
| Carriers                                                                                                                                                                                                                              | X        | X              | X         |
| Warehouses                                                                                                                                                                                                                            | X        | X              | X         |
| Advanced stock management                                                                                                                                                                                                             | X        |                |           |
| Suppliers                                                                                                                                                                                                                             | X        | X              | X         |
| Manufacturers                                                                                                                                                                                                                         | X        | X              | X         |
| CMS pages                                                                                                                                                                                                                             | X        | X              | X         |
| Contacts                                                                                                                                                                                                                              | X        | X              | X         |
| <p>Countries<br> A country's status (enabled or disabled) is common to all shop it is associated to.</p>                                                                                                                              | X        | X              | X         |
| Currencies                                                                                                                                                                                                                            | X        | X              | X         |
| Languages                                                                                                                                                                                                                             | X        | X              | X         |
| Modules                                                                                                                                                                                                                               | X        | X              | X         |
| — Hooks and exceptions                                                                                                                                                                                                                | X        | X              | X         |
| — Enabling/disabling                                                                                                                                                                                                                  | X        | X              | X         |
| — Configuration (for instance, PayPal login credentials)                                                                                                                                                                              | X        |                |           |
| Payment modules                                                                                                                                                                                                                       | X        | X              | X         |
| — Per-country restrictions                                                                                                                                                                                                            | X        |                |           |
| — Per-currency restrictions                                                                                                                                                                                                           | X        |                |           |
| — Per-customer group restriction                                                                                                                                                                                                      | X        |                |           |
| Friendly URLs                                                                                                                                                                                                                         | X        |                |           |
| Scenes                                                                                                                                                                                                                                | X        | X              | X         |
| Web service account                                                                                                                                                                                                                   | X        | X              | X         |
| Homepage image slider                                                                                                                                                                                                                 | X        |                |           |

Notes

**Categories**: A product can only appear in a given category of a shop if it has been associated to this category in that shop's context. In other words: if shop A and shop B have the C category in common, we can associate the P product to the C category for the A shop's context, and P will not appear in category C on shop B.

**Carriers**: You can manage the carriers association on a per-shop basis, a per-shop-group basis or for all shops; but you cannot customize a carrier on a per-shop basis. You must duplicate the carrier if you want to use the same carrier with different price ranges on two shops.

**Warehouses**: While advanced stock management can only be used for a single shop at a time, warehouses can be used with shop groups, and you can simply manage the warehouses in order to have advanced stock management.

For each shop, you can set specific price for every products, share part of the catalog or the whole of it, change product images, etc.

You can choose to share the customer accounts between your shops, enabling your customers to use the credentials between all shops, and even be transparently signed-in to each.

With advanced stock management, you can do a fine-grained management of the associations between yours shops and your warehouses.
