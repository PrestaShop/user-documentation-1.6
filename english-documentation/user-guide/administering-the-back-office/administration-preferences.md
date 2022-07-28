# Administration Preferences

The "Preferences" administration page contains general options and settings on the way PrestaShop itself works. It has four sections.

## General <a href="#administrationpreferences-general" id="administrationpreferences-general"></a>

This section is for the more general settings:

![](<../../../.gitbook/assets/43089940 (1).png>)

* **Automatically check for module updates**. You can ask PrestaShop to regularly check if there are new versions of your modules available from the Addons website. If so, the "Modules" page will display a "Update it!" button for installed modules, right next to their "Uninstall" button.
* **Check the IP address on the cookie**. This is an added security measure: you can tell PrestaShop to check that the user comes from the IP stored in his or her browser's cookie.
* **Lifetime of the Front Office cookie**. By default, the longevity of a PrestaShop cookie is 480 hours (20 days). You can reduce it if you feel your security needs it.
* **Lifetime of the Back Office cookie**. By default, the longevity of a PrestaShop cookie is 480 hours (20 days). You can reduce it if you feel your security needs it.

## Upload quota <a href="#administrationpreferences-uploadquota" id="administrationpreferences-uploadquota"></a>

This page helps you define the authorized size of uploaded files from your own team – not from your customers.

![](<../../../.gitbook/assets/43089941 (1).png>)

There are three options, one being general and the two others being more specific:

* **Maximum size for attachment**. The default value is directly taken from your server's settings, but you can lower it if necessary.
* **Maximum size for a downloadable product**. If you sell virtual products (services, booking and downloadable products), this setting can limit the size of the files your team can upload – and thus the size of the final product. Plan in advance so that you never leave one of your team members blocked.
* **Maximum size for a product's image**. Likewise, you can limit the size of image that you or your team can upload to your shop. This can serve as a handy reminder that team-members should strive to reduce the size of image, as it is often not useful to upload anything more than 600x600 (which is roughly 200 kB when correctly compressed). See the "Images" preferences page for the image sizes your shop is set to use. This has the added benefit of saving on both server space and bandwidth usage, as well as processor power (since PrestaShop resizes uploaded image to give you thumbnails and more).

## Help <a href="#administrationpreferences-help" id="administrationpreferences-help"></a>

_This option has been removed in PrestaShop 1.6.0.11._

To help you with your everyday usage of PrestaShop, the development team has added many tips & tricks within the interface.

![](<../../../.gitbook/assets/23789907 (1).png>)

You can have them displayed using one of these two options:

* **Back Office help boxes**. This will display yellow help boxes below some of the more obscure form fields.
* **Hide optimization tips**. This will display a box with configuration tips on the homepage of the PrestaShop back-office.

## Notifications <a href="#administrationpreferences-notifications" id="administrationpreferences-notifications"></a>

Notifications are numbered bubbles that are displayed at the very top of any administration page when you have loaded it, right next to the shop's name. They display the number of new items since the last time you clicked on them.

![](<../../../.gitbook/assets/43089943 (1).png>)

You can choose not to receive them for some content types:

* **Show notifications for new orders**. Clicking it display a larger bubble containing the name of the customers that registered since last time. From there on, you can either open any customer's single page, or open the "Customers" page to get the complete list.
* **Show notifications for new customers**. Clicking it display a larger bubble containing the numbers, amounts and customer names for the order that were last placed on your shop. From there on, you can either open any order's single page, or open the "Orders" page to get the complete list.
* **Show notifications for new messages**. Clicking it display a larger bubble containing the e-mail of the persons who last sent you a message using the contact form on your shop. From there on, you can either open any message, or open the "Customer Service" page to get the complete list.
