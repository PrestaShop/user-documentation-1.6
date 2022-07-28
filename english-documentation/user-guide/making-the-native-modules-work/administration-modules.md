# Administration modules

**Administration**

* ****[1-Click Upgrade - AutoUpgrade](administration-modules.md#Administrationmodules-1-ClickUpgrade-AutoUpgrade)
* [Advanced EU Compliance](administration-modules.md#Administrationmodules-AdvancedEUCompliance)
  * [Label options](administration-modules.md#Administrationmodules-Labeloptions)
  * [Feature options](administration-modules.md#Administrationmodules-Featureoptions)
  * [Legal content management](administration-modules.md#Administrationmodules-Legalcontentmanagement)
  * [Email content inclusion ](administration-modules.md#Administrationmodules-Emailcontentinclusion)
* [Cron tasks manager](administration-modules.md#Administrationmodules-Crontasksmanager)
* [CSV Export for Newsletters](administration-modules.md#Administrationmodules-CSVExportforNewsletters)
  * [Export Newsletter Subscribers](administration-modules.md#Administrationmodules-ExportNewsletterSubscribers)
  * [Export Customers](administration-modules.md#Administrationmodules-ExportCustomers)
* [Database Cleaner](administration-modules.md#Administrationmodules-DatabaseCleaner)
* [Email alerts](administration-modules.md#Administrationmodules-Emailalerts)
  * [Customer notifications](administration-modules.md#Administrationmodules-Customernotifications)
  * [Merchant notifications](administration-modules.md#Administrationmodules-Merchantnotifications)
* [Google Analytics API](administration-modules.md#Administrationmodules-GoogleAnalyticsAPI)
* [Image watermark](administration-modules.md#Administrationmodules-Imagewatermark)
* [Merchant Expertise](administration-modules.md#Administrationmodules-MerchantExpertise)
* [NVD3 Charts](administration-modules.md#Administrationmodules-NVD3Charts)
* [OnBoarding](administration-modules.md#Administrationmodules-OnBoarding)
* [Simple HTML table display](administration-modules.md#Administrationmodules-SimpleHTMLtabledisplay)

## 1-Click Upgrade - AutoUpgrade <a href="#administrationmodules-1-clickupgrade-autoupgrade" id="administrationmodules-1-clickupgrade-autoupgrade"></a>

This module makes it really easy to upgrade PrestaShop to its latest version.

See the "Automatic Update" chapter of the "Update PrestaShop" guide to learn more about this module: [http://doc.prestashop.com/display/PS16/Automatic+update](http://doc.prestashop.com/display/PS16/Automatic+update).

## Advanced EU Compliance <a href="#administrationmodules-advancedeucompliance" id="administrationmodules-advancedeucompliance"></a>

_New in PrestaShop 1.6.1.0._

The Advanced EU Compliance module helps merchants make their shops compliant with the recent, more restrictive EU regulations.

This is must-have module for European stores.

Most of its options are meant to provide more transparency to the final customers, with:

* More detailed price labels (“From” price, tax, shipping fees and delays, product weight, etc.)
* Advanced checkout page
* Legal content attachment for emails

Not all of its option will be useful in all countries, but they all help make your store more respectful of the EU e-commerce laws.\
The default settings are the recommended settings; you are free to enable or disable options as you see fit.

### Label options <a href="#administrationmodules-labeloptions" id="administrationmodules-labeloptions"></a>

Make sure to translate all text fields in all your available languages.

* **Estimated delivery time label (available products)**. Indicates the estimated delivery time for your in-stock products. Leave the field empty to disable the option. Default text is "Delivery: 1 to 3 weeks".
* **Estimated delivery time label (out-of-stock products)**. Indicates the estimated delivery time for your out-of-stock products. Leave the field empty to disable. Default text is "Delivery: 3 to 6 weeks".
* **'Before' Base price labe**. When a product is on sale, displays the base price with a 'Before' label.
* **Tax 'inc./excl.' label**. Displays whether the tax is included next to the product price ('Tax included/excluded' label).&#x20;
* **Shipping fees 'inc./excl.' label**. Displays whether the shipping fees are included, next to the product price ('Shipping fees included / excluded').\
  Once enabled, make sure the "Shipping and Payment" option is associated with a CMS page in the "Legal Content Management" section, further down in the configuration screen. The label will link to this content.
* **Product weight label**. Displays the weight of a product (when information is available and product weighs more than 1 kg).&#x20;
* **Product weight precision**. Helps you select precision level for product weight display (e.g: 1 kg / 1.01 kg). The value cannot be negative.
* **Revocation Terms within ToS**. Includes the content from the "Revocation Terms" CMS page within the Terms of Services (ToS).\
  Once enabled, make sure the "Revocation Terms" option are associated with a CMS page in the "Legal Content Management" section, further down in the configuration screen. The label will link to this content.
* **Revocation for virtual products**. Adds a mandatory checkbox when the cart contains a virtual product. Use it to ensure customers are aware that a virtual product cannot be returned.&#x20;
* **'From' price label (when combinations)**. Displays a 'From' label before the price on products with combinations. Since prices can vary from one combination to another, this label indicates that the final price may be higher.
* **Upper shopping cart text**. Adds a custom text above the shopping cart summary.
* **Lower shopping cart text**. Adds a custom text at the bottom of the shopping cart summary.&#x20;

### Feature options <a href="#administrationmodules-featureoptions" id="administrationmodules-featureoptions"></a>

* **Enable 'Tell A Friend' feature**. If enabled, the "Send to a Friend" module allows customers to send to a friend an email with a link to a product's page.\
  This option makes sure you comply with your local legislation before enabling: the emails sent by this feature can be considered as unsolicited commercial emails.&#x20;
* **Enable 'Reordering' feature**. If enabled, the "Reorder" option allows customers to reorder in one click from their Order History page.\
  This option makes sure you comply with your local legislation before enabling: it can be considered as unsolicited goods.&#x20;
* **Enable "Advanced checkout page"**. Replaces the standard checkout process with a more legally (EU of course) compliant one. This option only works with the default-bootstrap template or other compatible templates and with compatible payment methods (many modules already adapted).\
  Once enabled, the advanced checkout page displays the following sections: payment methods, address summary, ToS agreement, cart summary, and an "Order with Obligation to Pay" button.
* **Proportionate tax for shipping and wrapping**. Instead of assigning a tax rules group to carriers and gift wrapping, the average tax of the products in the cart is used to compute the tax of gift wrapping and shipping. This is very useful in Germany.\
  Once enabled, tax for shipping and wrapping costs will be calculated proportionate to taxes applying to the products in the cart.\
  In effect, this means that the customer will get a definitive "with tax" price at the beginning of the checkout, and the shipping and wrapping taxes will be calculated all along the checkout process and taken on your margin.

### Legal content management <a href="#administrationmodules-legalcontentmanagement" id="administrationmodules-legalcontentmanagement"></a>

Several options of this module need the system to “know” what some CMS pages are for. If no page is available for some needed page association, then you have to create them.

### Email content inclusion  <a href="#administrationmodules-emailcontentinclusion" id="administrationmodules-emailcontentinclusion"></a>

With this interface, you can choose which documents to include at the bottom to any of the standard e-mails sent by the shop – for instance, your shop's "Terms and Conditions" textual content can be included at the bottom of all invoices sent.

The content is chosen from the settings in the "Legal content management" section of this module. If no option is set, then you cannot choose a content to send.

## Cron tasks manager <a href="#administrationmodules-crontasksmanager" id="administrationmodules-crontasksmanager"></a>

This module provides you with a cron-like tool: you can create jobs which will call a given set of secure URLs to your PrestaShop store, thus triggering updates and other automated tasks.

## CSV Export for Newsletters <a href="#administrationmodules-csvexportfornewsletters" id="administrationmodules-csvexportfornewsletters"></a>

This module was built to export a CSV file of the e-mail addresses that your customers registered in your system.

Your customers can give you their e-mail address either by entering it in the Newsletter block located on the homepage or by checking the "Yes" box to subscribe to the newsletter when they register. You need these e-mail addresses in order to do some marketing.\
Upon registration, your customers have two choices related to the newsletter: The first one to subscribe to the newsletter, the second to receive offers from your partners (Opt-In).

### Export Newsletter Subscribers <a href="#administrationmodules-exportnewslettersubscribers" id="administrationmodules-exportnewslettersubscribers"></a>

This first section enables you to export all the e-mail addresses recorded from the Newsletter block on your homepage. After clicking the "Export .CSV file" button, a notification appears, asking you to click on a link to download the file containing the addresses.

Four pieces of information will be present in this file: the customer id, e-mail address, the day of registration, and the IP address. If you use this data with software such as Microsoft Excel, you can sort the information as you wish.

### Export Customers <a href="#administrationmodules-exportcustomers" id="administrationmodules-exportcustomers"></a>

This second section enables you to filter your customers' e-mail addresses before you export a CVS file of their data. For instance, filtering by country is particularly useful for sending newsletters in the right language and for adapting your offers.

You therefore take more information into account when exporting the e-mail addresses. Use the "Newsletter subscribers" selector to select one of the following three items:

* **All customers**. Enables you to select all the e-mail addresses of your customers who open an account on your shop. That is to say, those who do want to receive information from your part, as well as those who do not. Be careful what you did with it, then.
* **Subscribers**. Enables you to select only those customers who do want to receive a newsletter from you.
* **Non-subscribers**. Enables you to select only those customers who do not want receive a newsletter from you.

Next is the "Opted-in subscribers" selector, where you can filter the contacts based on their desire to register for messages from advertising partners. Similarly, three choices are available:

* **All customers**. Enables you to select all the e-mail addresses of your customers who open an account on your shop. That is to say, both those who do and do not wish to receive information from your part.
* **Subscribers**. Enables you to select only those customers who do want to receive a newsletter from your partners.
* **Non-subscribers**. Enables you to select only those customers who do not want receive a newsletter from your partners.

Once you have filtered the e-mail addresses to export, click the "Export .CSV File" button to retrieve all addresses. A notification appears, asking you to click and download the file. This file contains six types of information: the customer ID, last name, first name, e-mail address, IP address, and date of registration. You can then use this information to send your marketing campaigns.

## Database Cleaner <a href="#administrationmodules-databasecleaner" id="administrationmodules-databasecleaner"></a>

This module is very useful when you are done exploring PrestaShop for the first time, and you are ready to start adding your own content: you must first remove all the demo data that was installed along with PrestaShop: products, categories, client, orders, etc.

The configuration page has three sections:

* **Catalog.** This will erase all the data from the current catalog, even the items that you added yourself. Check the box and click the "Delete catalog" button to start the process.
* **Orders and customers**. This will erase all the currently registered orders and clients, even the ones that you created yourself. Check the box and click the "Delete catalog" button to start the process.
* **Functional integrity constraints.** This will check your database and make sure that everything is correctly set, and will try to fix what is not.
* **Database cleaning**. This will help reduce storage space and improve disk access efficiency.

**Be very careful**: any action triggered by clicking on one of these buttons is irremediable. Be sure to have a fresh backup of your database available first.

## Email alerts <a href="#administrationmodules-emailalerts" id="administrationmodules-emailalerts"></a>

PrestaShop enables you to alert you and your clients by e-mail in certain cases:

* Your clients: when a product is out of stock.
* You: when a new order is placed in your shop.
* You: when a product's stock is below a certain threshold.&#x20;
* You: when a product's coverage is below a certain number of days.

### Customer notifications <a href="#administrationmodules-customernotifications" id="administrationmodules-customernotifications"></a>

There is only one setting in this section:

* **Product Availability**. When you enable this setting, a field appears on the product page of your shop when the product is out of stock. It asks your customers to leave their contact information so that they may be contacted when you shop will have this product back in stock.

### Merchant notifications <a href="#administrationmodules-merchantnotifications" id="administrationmodules-merchantnotifications"></a>

There are several settings for merchants:

* **New order**. Enable this setting if you wish to be alerted of each new order
* **Out of stock**. Enable this setting and set the "Threshold" field with the value at which you wish to be alerted (default is 3).
* **Coverage warning**. Enable this setting and set the "Coverage field with the value at which you wish to be alerted (default is 0).

Merchant mail alerts can be sent to multiple addresses at the same time. To do so, list each e-mail address that will receive the notification (one e-mail address per line).

## Google Analytics API <a href="#administrationmodules-googleanalyticsapi" id="administrationmodules-googleanalyticsapi"></a>

This module enables you to tie your PrestaShop store with your Google Analytics account.

First, you must choose the API version you want to use:

* The 1.3 version will require you to enter your Google Analytics e-mail, password and profile.
* The 3.0 version will require you to enter your Google Analytics Client ID, Client Secret and profile.

We recommend the 3.0 one, since the 1.3 one is deprecated. In order to have the 3.0 version work, you must enable OAuth access by following these instructions: [https://developers.google.com/analytics/devguides/config/mgmt/v3/mgmtAuthorization](https://developers.google.com/analytics/devguides/config/mgmt/v3/mgmtAuthorization)

## Image watermark <a href="#administrationmodules-imagewatermark" id="administrationmodules-imagewatermark"></a>

This module enables you to add a watermark to all the product images on your shop. This limits their circulation on the Internet – and hopefully deter people from stealing them.

If you intend to export your products on Google Shopping, know that on this service, the usage of promotional text / logos and watermarks in the images is not allowed. You may only upload images which are free of any added watermarks / logos.\
Learn more about the Google Shopping policy here: [https://support.google.com/merchants/answer/2700371?hl=en\&ref\_topic=2701481](https://support.google.com/merchants/answer/2700371?hl=en\&ref\_topic=2701481)

The configuration page notifies you right away of which settings are currently missing.

* **Watermark file**. The chosen image must be in GIF format.
* **Watermark transparency (0-100)**. 100 amounts to a non-transparent image, which means that your logo will be very visible, but it will also completely hide part of the whole picture. The default setting, 60, is usually a good compromise.
* **Watermark X align**. Select where your watermark should appear on each of your images, here on the horizontal axis.
* **Watermark Y align**. Select where your watermark should appear on each of your images, here on the vertical axis.
* **Choose image types for watermark protection**. The type of images to which the watermark should be applied. You really only need to choose the biggest sizes, as these are the ones most likely to be stolen.

Once you have saved your settings, the configuration is completed but the watermarks are not yet added to your shop's pictures. Go to the "Preferences" menu, and open the "Images" page. There, click the "Regenerate thumbnails" button, near the bottom of the page. PrestaShop will process all your pictures (as selected in the configuration), and your watermark image will appear on the types of pictures that you selected.

## Merchant Expertise <a href="#administrationmodules-merchantexpertise" id="administrationmodules-merchantexpertise"></a>

This module was specifically designed to help PrestaShop users keep track of their progress as e-merchants, see how much they’ve grown and progressed over the days, months and years. It is installed by default.

This module adds a system of badges and points, broken down into three levels, all of which are integral to your success in the e-commerce world:

* **Features**. Tracks your use of key e-commerce features such as Site Performance, Catalog Size, Employees and SEO.
* **Achievements**. Tracks your completion of specific key e-commerce goals such as number of Customers, Orders and Revenue.
* **International**. Tracks your presence in key International markets such as the Americas, Oceania, Asia, Europe, Africa and Maghreb.

The more progress your store makes, the more badges and points you earn.\
There is no need to submit any information or fill out any forms. We know how busy you are; everything is done automatically. Use this tool to drive your business, view your progress and reflect on your great achievements.

## NVD3 Charts <a href="#administrationmodules-nvd3charts" id="administrationmodules-nvd3charts"></a>

NVD3 ([http://nvd3.org/](http://nvd3.org/)) is JavaScript library that was built specifically to generate beautiful charts using D3.js ([http://d3js.org/](http://d3js.org/)), a JavaScript library built to manipulate documents based on data.

This module enables the NVD3 charting code for your own uses, providing you with ever so useful graphs.

## OnBoarding <a href="#administrationmodules-onboarding" id="administrationmodules-onboarding"></a>

The OnBoarding module greets first-time users to their PrestaShop back office: through a small playful interface, it shows the user how to launch his/her shop in several easy steps.

## Simple HTML table display <a href="#administrationmodules-simplehtmltabledisplay" id="administrationmodules-simplehtmltabledisplay"></a>

Allows the statistics system to display data in a grid.
