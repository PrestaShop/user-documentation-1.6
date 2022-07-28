# Themes Preferences

**Themes Preferences**

* ****[Your current theme](themes-preferences.md#ThemesPreferences-Yourcurrenttheme)
  * [The Theme Configurator](themes-preferences.md#ThemesPreferences-TheThemeConfigurator)
  * [The theme's advanced settings](themes-preferences.md#the-themes-advanced-settings)
* [Select a theme for your "\[name\]" shop](themes-preferences.md#select-a-theme-for-your-name-shop)
* [Adding and exporting a theme](themes-preferences.md#ThemesPreferences-Addingandexportingatheme)
  * [Importing a theme: the "Add new theme" button](themes-preferences.md#importing-a-theme-the-add-new-theme-button)
  * [Creating a brand new theme](themes-preferences.md#ThemesPreferences-Creatingabrandnewtheme)
  * [Exporting a theme](themes-preferences.md#ThemesPreferences-Exportingatheme)
* [Live from PrestaShop Addons!](themes-preferences.md#ThemesPreferences-LivefromPrestaShopAddons!)

The "Themes" page enables you to efficiently manage your themes.

## Your current theme <a href="#themespreferences-yourcurrenttheme" id="themespreferences-yourcurrenttheme"></a>

The first section of the page serves as a reminder of which theme you are currently using, with its details:

* Theme name.
* Theme version.
* Theme author's name, website and email address.
* Thumbnail for the theme.

![](<../../../.gitbook/assets/25722885 (1).png>)

This section also gives you access to a handful of tools, which helps you to quickly customize the current theme: header logo, mail logo, invoice logo, favicon, store icon and even the navigation pipe can be easily modified from there. This section features:

* **Customize your theme**. A link to the Theme Configurator (provided that the Theme Configurator module is indeed installed and enabled).
* **Configure your theme**. A link to the theme's advanced settings.
* 4 tabs with the theme's appearance options:
  * **Logo**. The logo that will appear on all the pages of your shop.
  * **Invoice & email logos**. The logos that will respectively appear in your shop's invoices, and its email notifications.
  * **Icons**. Your shop's favicon (displayed in the web browser's address bar) and your Store icon (for use on the Store map as an indicator of where a store is).
  * **Mobile**. The logo that will appear on all the pages of your shop, when accessed through a mobile device. You can also choose to selectively enable or disable your theme's mobile version (if it does exist) for smartphones, tablets, or both.

The default theme uses a "YourLogo" logo. It is strongly recommended to change all of the instances of the logo and use yours!

In multistore mode, you can apply these changes to all your stores or to a group of stores at one time, using the multistore menu.

The "Enable the mobile theme" makes it possible for you to use the default mobile theme. With this theme, any PrestaShop merchant can have his or her shop be accessible to mobile devices: from the home page to the payment process, along with product pages and conversion funnel.

![](<../../../.gitbook/assets/25722886 (1).png>)

The mobile theme only works for PrestaShop's default theme, since it is included in its folder: `/themes/default/mobile`. Therefore, it will not work if you use another theme which does not have its own mobile theme.

Nonetheless, you can easily use the default mobile theme with any other theme, at least temporarily: simply copy the mobile theme's folder from the default theme's folder to the new theme's folder, and you should be good to go. For instance, if your new theme's folder is `/themes/magnolia`, copy the `/themes/default/mobile` folder to the new theme's folder: `/themes/magnolia/mobile`.\
&#x20;This is particularly useful if the new theme does not feature a responsive design: this way, your shop can still look good on mobile devices – albeit with the default PrestaShop look.

### The Theme Configurator <a href="#themespreferences-thethemeconfigurator" id="themespreferences-thethemeconfigurator"></a>

The Theme Configurator module helps you configure some aspects of your theme.

Clicking on the link from the "Themes" preferences page opens its configuration page. That page gives you direct links to the most usual front office modules: you can enable and disable a dozen of features, such as displaying social buttons or the Facebook block (provided their respective modules are enabled), and get direct access to their configuration page. You can also enable and access the Live Configurator from there, which makes it possible to easily change your theme's main color and font.

In a second section, the Theme Configurator makes it possible for you to easily attach images with links on specific home page hooks: home, top, left, right, footer. Each available language has its own tab with its own hooks that you can edit from here: this is essential as images often contain text directly on them, making it necessary to have as many versions of the image per available languages.

The module is explained in more details in the "Making the Native Modules Work" chapter of this guide.

If you are using the default theme and want to customize it, here is a summary of the [different image sizes you will need](https://www.prestashop.com/blog/en/image-sizes-types-prestashops-default-template/).

### The theme's advanced settings

Clicking on the "Advanced settings" button displays the main information about the theme (see the "Creating a brand new theme" section below to find an explanation of the fields).

![](<../../../.gitbook/assets/23790009 (1).png>)

Below the main section, the "Appearance of columns" section displays a lot of information about the way the left and right columns appear, depending on the page:

* If the box is checked, the column appears in the page (for instance, the Category page).
* If it is left unchecked, it will not appear on that page.

Note that even if you can click on the buttons at will, these settings are only informational, and the theme will not necessarily be able to adapt to your changes!

![](<../../../.gitbook/assets/23790010 (1).png>)

## Select a theme for your "\[name]" shop

This section is only display if you have at least two themes installed. It presents you with the other available themes on your PrestaShop installation beside the already-enabled one.

This section simply shows the thumbnails of the available themes, with their names.

![](<../../../.gitbook/assets/23789780 (2).png>)

Move your mouse cursor over the thumbnail to display a menu with two options:

* **Use this theme**. This will replace your current theme with this theme.
* **Delete this theme**. This will delete this theme's files from your web server.

At the top right, the "Visit the theme store" opens a new page to the PrestaShop Addons marketplace, where you can find more themes.

In multistore mode, you cannot apply a theme to all your stores or a group of stores; you must select a single store in the multistore menu, then pick a theme.

## Adding and exporting a theme <a href="#themespreferences-addingandexportingatheme" id="themespreferences-addingandexportingatheme"></a>

Two buttons at the top of the screen enable you to import a theme and install it (and its attached modules), or to export a theme and its modules from your shop in order to share it with the world.

### Importing a theme: the "Add new theme" button

This screen presents you with 3 methods to install a new theme:

* from your computer,
* from a public website,
* from your own FTP server.

A final button leads you to the theme creation form, presented in the next section.

![](<../../../.gitbook/assets/30670862 (1).png>)

Whatever the method, the process remains the same: indicate the location of the theme's Zip archive, then click "Save". The only thing that changes is the source of the Zip file:

* **Import from your computer**. Use the file explorer to find the archive.
* **Import from the web**. Indicate the direct public URL to the archive.
* **Import from FTP**. Using your FTP client, upload the archive in the following folder: `/themes/` .

Click "Save" to validate your choice. The theme is now installed, and PrestaShop asks you if you wish to install modules that were imported along with the theme, what you would rather do with the current modules configuration, and how you would like the images configuration to be taken into account.

Click "Save" one last time. A final confirmation page presents you with all the changes applied to your PrestaShop install. Click "Finish" to end the process.

### Creating a brand new theme <a href="#themespreferences-creatingabrandnewtheme" id="themespreferences-creatingabrandnewtheme"></a>

The best way to create a new theme for PrestaShop is to copy the files from the default theme, and start modifying its TPL and CSS files to make them your own. The reason is that a PrestaShop theme requires many files to be present: by starting from an existing theme instead of from scratch, you make sure that your own theme will not be missing any part.

You can do this directly on the web server, but PrestaShop makes it easy to copy the files from an installed theme and register your new theme in its system (a step you would have to do in any case).

All of this is done by clicking on the "Create new theme" button from the "Add new theme" button at the top of screen. It displays a creation form.

![](<../../../.gitbook/assets/23789773 (1).png>)

Fill-in its fields:

* **Name of the theme**. Make sure the name is not already used by another theme (check on the Addons website).
* **Preview image for the theme**. You should always add a preview image, as it is a clear reminder of what the theme looks like. If you do not have one yet, leave that for later, when the time will come to release the theme.
* **Default left column** and **Default right column**. Indicate if your theme has a column (or even two columns), and if so, on which side of the screen. This is purely informational, and can be changed at any time.
* **Number of products per page**. Indicate the default number of products that should be shown on a page. This option can be adjusted later on.
* **Name of the theme's directory**. Try to keep it close to your theme's name. If you have not already created a theme folder, PrestaShop will create one for you.
* **Copy missing files from existing theme**. This is the cleanest method to start a new theme from another theme's files. Choose "default-bootstrap", or any other theme that you would like to base your foundation on.
* **Responsive**. Indicate if your theme has a responsive design or not (if you do not know what a responsive design is, then you probably should choose "No"). This is purely informational, and can be changed at any time.

Click save, and PrestaShop will register this information for you: the theme is ready to be enabled, and its preview image appears in the theme selector.

It is now up to you to change your theme's files in order to make it unique! On your local installation (not a production one!), select your new theme, and start working!\
Once you are done with your designing and code it, go back to this setting page and change it accordingly: definitive preview image, default column, number of products, and responsiveness.

Is your theme so good that other merchants could pay money for it? You can sell it on Addons, PrestaShop's official theme & module marketplace: [http://addons.prestashop.com/](http://addons.prestashop.com/).

### Exporting a theme <a href="#themespreferences-exportingatheme" id="themespreferences-exportingatheme"></a>

This section is only available when there is at least one theme installed on your PrestaShop site. It gives you a method to export your module in the correct format (most notably with a working configuration file).

Exporting a theme is very useful when you want either to back the theme up for safety, and create an archive of the theme for a friend or in order to make it available on the Addons marketplace ([http://addons.prestashop.com/](http://addons.prestashop.com/)). Not only does it generate a complete Zip archive of your theme, but it also adds many information in an XML files, which is very useful both when uploading to Addons, and when importing to another PrestaShop site.

![](<../../../.gitbook/assets/30670863 (1).png>)

Select a theme and click on "Save". A configuration form appears where you can set the exported themes parameters: author name, modules to export along, theme name, version compatibility, etc.

![](<../../../.gitbook/assets/23790012 (1).png>)

Once all the parameters are correctly set, click on "Save". You will quickly get a file to download from your browser. Save it on your hard-drive, then give the saved file a proper name instead of the random one it currently has. From there on, you can easily share this theme, and if it is your own creation, you can start selling it on PrestaShop's Addons marketplace at [http://addons.prestashop.com/](http://addons.prestashop.com/).

## Live from PrestaShop Addons! <a href="#themespreferences-livefromprestashopaddons" id="themespreferences-livefromprestashopaddons"></a>

This final section presents you with 12 of the latest themes from PrestaShop's Addons marketplace. You can click on each image to reach the theme's individual Addons page and get a better view of it, and possibly buy it.

You can also use the search form to find the theme that best suits your store.

![](<../../../.gitbook/assets/23789784 (2).png>)
