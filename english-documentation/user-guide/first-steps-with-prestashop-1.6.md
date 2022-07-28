# First steps with PrestaShop 1.6

**Table of contents**

* [First steps with PrestaShop 1.6](first-steps-with-prestashop-1.6.md#FirststepswithPrestaShop1.6-FirststepswithPrestaShop1.6)
  * [Deactivate your shop](first-steps-with-prestashop-1.6.md#FirststepswithPrestaShop1.6-Deactivateyourshop)
  * [Delete the content of the default shop](first-steps-with-prestashop-1.6.md#FirststepswithPrestaShop1.6-Deletethecontentofthedefaultshop)
  * [Configure your shop's information](first-steps-with-prestashop-1.6.md#configure-your-shops-information)
    * [The shop's basic settings](first-steps-with-prestashop-1.6.md#the-shops-basic-settings)
    * [Shop languages](first-steps-with-prestashop-1.6.md#shop-languages)
    * [Employees information](first-steps-with-prestashop-1.6.md#FirststepswithPrestaShop1.6-Employeesinformation)
  * [Configure your payment methods](first-steps-with-prestashop-1.6.md#FirststepswithPrestaShop1.6-Configureyourpaymentmethods)
  * [Configure carriers and shipment](first-steps-with-prestashop-1.6.md#FirststepswithPrestaShop1.6-Configurecarriersandshipment)
  * [Choose your theme](first-steps-with-prestashop-1.6.md#FirststepswithPrestaShop1.6-Chooseyourtheme)
  * [Choose your modules](first-steps-with-prestashop-1.6.md#FirststepswithPrestaShop1.6-Chooseyourmodules)
  * [Create your products and product categories](first-steps-with-prestashop-1.6.md#FirststepswithPrestaShop1.6-Createyourproductsandproductcategories)
  * [Create your static content](first-steps-with-prestashop-1.6.md#FirststepswithPrestaShop1.6-Createyourstaticcontent)
  * [Build your top menu](first-steps-with-prestashop-1.6.md#FirststepswithPrestaShop1.6-Buildyourtopmenu)
  * [Activate your shop](first-steps-with-prestashop-1.6.md#FirststepswithPrestaShop1.6-Activateyourshop)

## First steps with PrestaShop 1.6 <a href="#firststepswithprestashop1.6-firststepswithprestashop1.6" id="firststepswithprestashop1.6-firststepswithprestashop1.6"></a>

You must spend a good amount of time making sure every part of your future online shop is properly set up, secured, validated and ready for business.

While PrestaShop makes it easy for you to install it and build your business online, it cannot possibly be a 5-seconds work: you are dealing with products, customers, carriers, and most importantly with real actual money that will be flowing from your customers to your bank account. We dare say you want to make sure nothing fails in the process of validating an order, having the products be found in your storage location, then be packaged, and shipped to your customers without a single glitch, or even without anything unpredicted happening without your knowledge.

PrestaShop is a very complete tool, and the number of possibilities can feel overwhelming. This chapter will therefore lead you through some basic actions to perform in order to set up your shop before the big launch. A lot can and must be done before you launch your shop, but these steps are the essential configuration steps of any shop.

### Deactivate your shop <a href="#firststepswithprestashop1.6-deactivateyourshop" id="firststepswithprestashop1.6-deactivateyourshop"></a>

We will consider that you are still within the first hour following your installation of PrestaShop, in a single-shop instance.

Deactivating your shop means making sure that no one can access it while you are busy making changes, creating products, settings prices and taxes, installing payment modules and a new theme, setting carriers... This is called "putting your shop in maintenance mode".

![](<../../.gitbook/assets/23038235 (1).png>)

In your back office, go the "Preferences / Maintenance" page. This page features two simple settings:

* **Enable Shop**. Simply set it to "No", and your front-end will display the maintenance page to your visitors, which simply states that your shop will soon be back online.
* **Maintenance IP**. This is where you must put your own IP address, so that you can still get access to your front page, and browse your shop as if it was available to all. This is a must-do every time you put your shop in maintenance mode, as you will always need to browse your front-end so as to make sure everything is in place as intended.\
  Simply click on the "Add my IP" button. You can add more IP addresses by separating them with commas.

If you have already decided what your theme and products are, you can simply put your shop in Catalog mode. This means that customers can browse your shop, but no price will be displayed, and they won't be able to add anything to their cart until you disable the Catalog mode.

You can activate the Catalog mode by going to the "Preferences / Products" page, where it is the first option.

![](<../../.gitbook/assets/23038237 (1).png>)

### Delete the content of the default shop <a href="#firststepswithprestashop1.6-deletethecontentofthedefaultshop" id="firststepswithprestashop1.6-deletethecontentofthedefaultshop"></a>

The default installation features a handful of products – mainly women's clothing. Their only use is to help you explore the organization of a real store. After you've learned the intricacies of the ties between products, categories, orders and customers, you should delete all these items in order to start your shop with a clean slate.

![](<../../.gitbook/assets/23038239 (1).png>)

You must therefore delete all the default data, which means:

* products and their...
  * categories
  * attributes
  * features
  * manufacturers
  * suppliers
  * image mappings
  * tags
* orders
  * order messages
* customers
  * customers shopping carts
* carriers
  * price ranges
  * weight ranges
* contact & stores (delete or adapt to your business' needs)
* CMS pages (delete or adapt to your business' needs)

This would mean browsing through the many various screens of the back office and deleting content one page after the other, but there is much easier way:

1. Go to the "Modules > Modules" page.
2. Find the "Database Cleaner" module and click its "Install" button.
3. You are directly taken to its configuration page (if not, click its "Configuration" button).
4. Read and accept the warning, then click the "Delete Catalog" button: it will delete all your products and their attributes, manufacturers, etc.
5. Read and accept the warning, then click the "Delete Orders & Customers" button: it will delete all your customers and their orders, carts, etc.
6. Click the "Check & fix" button to refine your database integrity constraints.
7. Click the "Clean & optimize" button to reorganizes the physical storage of table data and associated index data, to reduce storage space and improve I/O efficiency when accessing the tables.

THERE IS NO WAY BACK. Be sure to only click these buttons if you do intend to wipe your database from its default content.

### Configure your shop's information

Now that you have a clean shop, you can start making it your own, and that implies setting everything up to your likings, starting with your personal information and your preferences.

#### The shop's basic settings

You should pay attention to the following settings, most of which are important because they are displayed on the front office, and therefore in plain sight of your customers.

Some of these settings require you to configure a module instead of changing one of PrestaShop's preferences.

Configuring a module is easy:

1. Go to the "Modules" page under the "Modules" menu.
2. Type the name of the module (or part of it) in the module search box. It should display results as you type.
3. When the module is found, click its "Configure" button, and follow the instructions.

For each module presented here, you should read their documentation for more information.

| Setting                               | Description                                                                                                                                                                                                                                                                                                                                                                          | Where to find it                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| ------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Shop name                             | Defines your brand, most notably on search engines (Google, Yahoo!, Bing...).                                                                                                                                                                                                                                                                                                        | "Preferences" menu, "Store Contacts" page, then in the "Contact details" section, edit the "Shop name" option.                                                                                                                                                                                                                                                                                                                                                                                                 |
| Shop logo                             | <p>Defines your brand visually. The default logo says "YourLogo" as an incentive to use yours.<br>Displayed at the top left of every page of your store, as well as in your invoices and other automatic e-mails.</p>                                                                                                                                                                | "Preferences" menu, "Themes" page, "Appearance" section, then change the various default images to your logo.                                                                                                                                                                                                                                                                                                                                                                                                  |
| Default shop currency                 | The currency in which you want to set the default price for your products.                                                                                                                                                                                                                                                                                                           | <p>"Localization" menu, "Localization" page, "Configuration" section.<br>If the currency is not available, you must import localization pack for its country first: use the "Import a localization pack" tool from the same page.</p>                                                                                                                                                                                                                                                                          |
| Customer service info                 | <p>A block presenting the phone number for your customer service, and a button to send you an e-mail.<br>Displayed in the front office's right column.</p>                                                                                                                                                                                                                           | "Contact block" module.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| <p>Company info /<br>Contact info</p> | <p>A block presenting your contact address, the phone number for your customer service, and a link to send you an e-mail.<br>Displayed in the front office's footer.</p>                                                                                                                                                                                                             | "Block contact info" module.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| Advertising                           | <p>A block presenting an image with a link to another site.<br>Displayed in front office, left column.</p>                                                                                                                                                                                                                                                                           | "Advertising block" module.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| Image slider                          | <p>The slider presents several images, scrolling one after the other. It is a strong visual signature for your store and products.<br>Usually placed front and center of the homepage</p>                                                                                                                                                                                            | "Image slider for your homepage" module.                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| CMS pages                             | <p>The content of static pages, such as "About Us", "Delivery", "Legal Notice", "Terms and Conditions", and "Secure Payment". Some of them have default content, which you should adapt to your business; some others are empty, and you should paste your own text.<br>Displayed in the "Information" block in the left column, and in the "Information" section of the footer.</p> | "Preferences" menu, "CMS" page, then edit and create pages at will.                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| Social networks                       | <p>A block presenting three links: your company's Facebook page, your company's Twitter account, and the RSS feed for your company's blog (or "current events" site).<br>By default, all these links lead to the PrestaShop company's own sites. It is important that you change it to your own.<br>Displayed in the "Follow us" section of the footer.</p>                          | "Social networking block" module.                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| Top menu                              | The top of the default theme uses a top menu to indicate categories that the visitor can go to, as well as links to other locations – for instance, the default installation has a "Blog" link which sends the use to the official PrestaShop blog.                                                                                                                                  | "Top horizontal menu" module.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| Homepage content                      | The default theme contains a lot of demo content: texts, images, links, etc. If you intend on using that theme for your own store instead of buying your theme, you should make sure to remove all the default content first.                                                                                                                                                        | <p>"Theme configurator" module: this module handles a lot of things on your theme. Mainly, it enables you to switch some feature off and on (social sharing buttons, top banner, payment logos, etc.), and perhaps more importantly, it lets you easily add/change images on your home-page.<br>"Custom CMS information block" module: this module helps you manager the two last blocks at the bottom of the home-page, right before the footer: the "Free shipping etc." one and the "Custom block" one.</p> |

These are the most visible default settings on your front-end – at least with the default theme.\
The "Where to find it" column enables you to see where you can find the interface to change these aspects of your store. This user guide will provide you with more details for each interface.

#### Shop languages

PrestaShop is able to work with many languages, both on the front office and the back office. As soon as more than one language is enabled in your back office, each back office text-field is accompanied with a language code selector, which indicates the current language, and which you can click in order to choose another language in which to write that field's content.

![](<../../.gitbook/assets/23038241 (1).png>)

By default, PrestaShop is installed with two languages: the one used when installing the software, and French. To manage the currently installed languages, go to the "Localization / Languages" page. It presents you with a table of the available languages.

![](<../../.gitbook/assets/23038243 (1).png>)

The currently enabled language(s) have a green "Yes", while the others have a red "No". Click on a "Yes" to disable the selected language; click on a "No" to enable it back.

You can install and enable many languages if you think your shop needs them, but be aware that you will have to translate your content for all of the enabled languages: product names, descriptions, tags, category names and descriptions, static content (CMS pages), module settings, etc.

You can easily import many more languages in the "Localization / Localization" page, and then enable them in the "Localization / Languages" page.

#### Employees information <a href="#firststepswithprestashop1.6-employeesinformation" id="firststepswithprestashop1.6-employeesinformation"></a>

Should you have people helping you with your shop (whether they are your family, your friends, or paid employees), you should make sure to create an employee account for each of them – if only to know who has performed which recent action. The other advantage is that you can give them specific profiles and specific access rights to the administration pages: for instance, you might not want everyone to have access to your statistics, your invoices or your payment settings.\
You can create as many profiles as needed.

To create a new employee account, go to the "Administration" menu, select "Employees", and click the "Add new employee" button. Give it a name, such as "Martin Doe" or "Shipping handler", and save.\
An account can be used for as many people as needed – but we do advise you to create one for each helping person.

Now that you have a proper account for this employee, you should give that account specific permissions, tailored to the employee's tasks. By default, a new profile cannot do much. It is up to you to set exactly the parts of your shop to which that profile should have access. It can be a tedious task, but it is an important one.\
To assign permissions to an employee account, you must use the "Profile" option in the account creation page: this menu lets you pick the account's profile (SuperAdmin, translator, etc.)

![](<../../.gitbook/assets/23038245 (1).png>)

You can edit these permissions this way: go to the "Administration" menu, select "Permissions", and select the profile you want to change. A long list of permissions appears: edit them at will. Your changes are saved automatically.

### Configure your payment methods <a href="#firststepswithprestashop1.6-configureyourpaymentmethods" id="firststepswithprestashop1.6-configureyourpaymentmethods"></a>

Your shop is meant to earn money, and this can only become a reality if you use at least one payment module. Several modules are already available in the default install, which you can install and configure (from the "Modules" page under the "Modules" menu, in the "Payments & Gateways" category), and create restrictions for them (in the "Payment" page under the "Modules" menu). Many payment modules require you to first set up an account on the service they were built for.

See the "Payment" section of the "Making the Native Modules Work" chapter of this guide in order to learn about them all.

You can also install other payment modules, downloaded from the Addons marketplace: [http://addons.prestashop.com/en/4-payments-gateways-prestashop-modules](http://addons.prestashop.com/en/4-payments-gateways-prestashop-modules)

Check and bank wire are the only two payment methods which are enabled by default. If you choose to keep them, you **need** to configure them with your information: check order and address, account owner, bank details (IBAN, BIC, etc.).

These payment methods are configured through the "Bank Wire" and "Payment by check" modules, which you can find in the "Payments & Gateways" category of the modules list.

### Configure carriers and shipment <a href="#firststepswithprestashop1.6-configurecarriersandshipment" id="firststepswithprestashop1.6-configurecarriersandshipment"></a>

Products sold on your shop must be shipped to your customers – unless you only sell downloadable products, in which case the "Shipping" menu will be of little use to you.

Whether you are sending your products yourself by regular post office mail, or you have set up a contract with a carrier, you should set this information within PrestaShop.

See the "Managing Shipping" chapter of this guide in order to learn about shipping and carriers.

**Merchandise return is not enabled by default**. If you want to allow your customers to return products and get a refund or a voucher, you can do it in the "Merchandise return (RMA) options" of the "Merchandise return" page, under the "Orders" menu.\
&#x20;Merchandise return is explained in the "Managing Orders" chapter of this guide.

### Choose your theme <a href="#firststepswithprestashop1.6-chooseyourtheme" id="firststepswithprestashop1.6-chooseyourtheme"></a>

Your shop should have its own theme in order to have a distinctive style, and therefore be more recognizable, separating it from the numerous other online shops.

There are many themes to choose from on the PrestaShop Addons marketplace: [http://addons.prestashop.com/en/3-templates-prestashop](http://addons.prestashop.com/en/3-templates-prestashop).

You can also choose to create your own theme, or have it created for you by a developer. Refer to the PrestaShop Designer Guide for help.

Once your theme is installed, you should explore it fully in order to know it by heart and be able to help customers out of a situation. Read its documentation carefully.

You can and should customize some of the theme's aspects, most notably its logo in various situations (header, mail, invoice, etc.). This is done using the "Themes" preferences page, which you can find under the "Preferences" menu.

### Choose your modules <a href="#firststepswithprestashop1.6-chooseyourmodules" id="firststepswithprestashop1.6-chooseyourmodules"></a>

PrestaShop comes bundled with more than a hundred modules. These are very varied: analytics, front office features, payment, shipping... You should explore the available modules in full, in order to know which ones you might want to enable, and which you'd rather keep disabled.

See the "Managing Modules" and "Making The Native Modules Work" chapters of this guide in order to learn about them all.

You can also find many other modules on the Addons marketplace: [http://addons.prestashop.com/en/2-modules-prestashop](http://addons.prestashop.com/en/2-modules-prestashop)

Every time you activate and configure a module, make sure that it does work well within the confines of your theme, in case its features impact your shop's front-end.

### Create your products and product categories <a href="#firststepswithprestashop1.6-createyourproductsandproductcategories" id="firststepswithprestashop1.6-createyourproductsandproductcategories"></a>

This is described in details in the "Adding Products and Product Categories" chapter.

### Create your static content <a href="#firststepswithprestashop1.6-createyourstaticcontent" id="firststepswithprestashop1.6-createyourstaticcontent"></a>

If you haven't done this already, you should take the time to write the content for the various static pages which are either already available in your PrestaShop installation, or ones that you feel are needed.

Some pages already exist, but their content should really be triple-checked, as they can have a lot of impact on your shop's legal status, among other things.

The default pages are "About Us", "Delivery", "Legal Notice", "Terms and Conditions", and "Secure Payment". Some of them have default content, which you should update; some others are empty, and you should paste your own text.\
To edit these pages, go to the "Preferences" menu, click the "CMS" page, then choose the page you want to edit, or create new ones.

You can create as many pages as you feel are necessary.

### Build your top menu <a href="#firststepswithprestashop1.6-buildyourtopmenu" id="firststepswithprestashop1.6-buildyourtopmenu"></a>

Now that you have product categories and CMS pages, you should arrange them in a logical and compelling way in the top menu.

This is done using the "Top horizontal menu" module: go to the "Modules" page, type "menu" in the module search form, and you should find the module. Enable it if it is disabled, then configure it: remove the pages or categories you deem unnecessary, add other pages, and move the content around, until you are satisfied with your menu's hierarchy.

### Activate your shop <a href="#firststepswithprestashop1.6-activateyourshop" id="firststepswithprestashop1.6-activateyourshop"></a>

Now that all is set and done, you can finally open your shop to the public.

Go the "Preferences / Maintenance" page, and change the two options:

* **Enable Shop**: set it back to "Yes".
* **Maintenance IP**: remove your IP from the list. This is optional: your shop will still work if you leave the field as it is.

Your shop should now be fully ready to receive its first visitors... and take its first orders!
