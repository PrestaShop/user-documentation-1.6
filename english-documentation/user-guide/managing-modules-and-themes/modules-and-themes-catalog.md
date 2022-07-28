# Modules and Themes Catalog

**Table of contents**

* [Modules and Themes Catalog](modules-and-themes-catalog.md#ModulesandThemesCatalog-ModulesandThemesCatalog)
  * [Installing a module](modules-and-themes-catalog.md#ModulesandThemesCatalog-Installingamodule)
    * [Installing using the dedicated form](modules-and-themes-catalog.md#ModulesandThemesCatalog-Installingusingthededicatedform)
    * [Installing using a FTP client](modules-and-themes-catalog.md#ModulesandThemesCatalog-InstallingusingaFTPclient)
  * [Updating a module](modules-and-themes-catalog.md#ModulesandThemesCatalog-Updatingamodule)
  * [Uninstalling a module](modules-and-themes-catalog.md#ModulesandThemesCatalog-Uninstallingamodule)
  * [Installing a theme](modules-and-themes-catalog.md#ModulesandThemesCatalog-Installingatheme)
    * [Installing using PrestaShop's theme installer](modules-and-themes-catalog.md#installing-using-prestashops-theme-installer)
    * [Installing using a FTP client](modules-and-themes-catalog.md#ModulesandThemesCatalog-InstallingusingaFTPclient.1)
  * [Exporting a theme](modules-and-themes-catalog.md#ModulesandThemesCatalog-Exportingatheme)
  * [PrestaShop's mobile template](modules-and-themes-catalog.md#prestashops-mobile-template)
    * [Installing the mobile template for your shop](modules-and-themes-catalog.md#ModulesandThemesCatalog-Installingthemobiletemplateforyourshop)
    * [Customizing the mobile template](modules-and-themes-catalog.md#ModulesandThemesCatalog-Customizingthemobiletemplate)
    * [Using the mobile template with another theme](modules-and-themes-catalog.md#ModulesandThemesCatalog-Usingthemobiletemplatewithanothertheme)

## Modules and Themes Catalog <a href="#modulesandthemescatalog-modulesandthemescatalog" id="modulesandthemescatalog-modulesandthemescatalog"></a>

PrestaShop comes bundled with more than 100 modules, but even that number might seem limiting, or you could want to explore other directions.

![](<../../../.gitbook/assets/23789638 (2).png>)

There are many more modules available on the PrestaShop Addons website ([http://addons.prestashop.com/](http://addons.prestashop.com/)). Some are free, others are for-pay, and you are sure to find something that suits your needs! Once you are a seasoned module developer/theme designer, you can even submit your own creations, and sell them on Addons!

The "Modules & Themes Catalog" page gives you a quick and easy access to the online Addons database of modules and themes. Its interface is pretty straightforward:

* A search field, with which you can search the whole content of the Addons website.
* A list of 8 modules that you can buy directly.
* A list of 12 themes that you can buy directly.

A search query will send you to the Addons website, where more options are available.

Clicking on an item will open its Addons page in a new browser tab.

Addons is the official marketplace for PrestaShop Modules and Themes. This is where shop owners can get all the necessary items to customize their shop, and where authors can share their creations with the community.

Modules and themes can either be free or for-sale: the price is set by the author. Take the time to browse the available modules and themes, because expensive does not always mean better.

You must be logged-in before you can download or rate anything. Creating an account is free.

### Installing a module <a href="#modulesandthemescatalog-installingamodule" id="modulesandthemescatalog-installingamodule"></a>

Once you have downloaded a module from the Addons online shop to your computer, it is up to you have it installed on your PrestaShop site.

There are two ways to install a module: either using the dedicated form, or using your FTP client.

#### Installing using the dedicated form <a href="#modulesandthemescatalog-installingusingthededicatedform" id="modulesandthemescatalog-installingusingthededicatedform"></a>

To install a new PrestaShop module automatically, click on the "Add new module" link at the top of the list of modules, in the "Modules" page. A new section will slide open.

![](<../../../.gitbook/assets/23789641 (2).png>)

The form in this section enables you to upload the archive file of the module, as downloaded from Addons. You can either upload a `zip` file, or a `tar.gz` one (tarball). The form is straightforward: simply browse to the module's file that you downloaded, and click the "Upload this module" button. Do not point to the module's uncompressed folder or any of its unpacked files: only the archive file!

Once you have clicked the button, PrestaShop will upload the module from your computer to its server, unpack it, place the files in the correct location, and update the page, all this in a handful of seconds. PrestaShop will then display "Module downloaded successfully".

Modules are not installed by default: you still have to click the module's "Install" button, and then possibly configure its settings.

Once configuration is complete, be sure to test the module immediately to confirm that it works as planned.

#### Installing using a FTP client <a href="#modulesandthemescatalog-installingusingaftpclient" id="modulesandthemescatalog-installingusingaftpclient"></a>

To install a new PrestaShop module manually:

1. Unzip (decompress) the module archive file (`.zip` or `tar.gz`). This should result in a new folder.
2. Using your FTP client, connect to PrestaShop web server, and place the unpacked module folder in PrestaShop's `/modules` folder.\
   &#x20;Pay attention NOT to upload that folder in another module's folder (which can happen when drag-and-dropping items). Upload both the folder and the files it contains, not just the files.
3. Go to your back office, in the "Modules" menu.
4. Locate the new module in the modules list. You might have to scroll down; you can also use the list's search engine, which should give you a dynamically updated list of matching module names.
5. In the row for the new module, click the "Install" button.
6. Your module is now installed and should be activated too. If necessary, click on the module's "Configure" link. Also, pay attention to any warning message that might be displayed by PrestaShop.

Once configuration is complete, be sure to test the module immediately to confirm that it works as planned.

Modules can come from many sources, and not all of them are reliable. This is why PrestaShop 1.6.0.7 introduced a warning window for "Untrusted" modules – that is, modules that have not been verified by PrestaShop through its Addons marketplace. This screen window lets you choose whether to proceed with the installation with no further notification, or to stop the installation process.

![](<../../../.gitbook/assets/25722883 (2).png>)

Installing a native module or a module obtained through Addons will not trigger the display of this window.

### Updating a module <a href="#modulesandthemescatalog-updatingamodule" id="modulesandthemescatalog-updatingamodule"></a>

Your PrestaShop installation regularly checks with the Addons server if there is any update for your modules. If so, PrestaShop displays a "Update it!" link for the affected modules. Simply click it, and PrestaShop will take care of downloading and updating the module.

![](<../../../.gitbook/assets/25722884 (2).png>)

### Uninstalling a module <a href="#modulesandthemescatalog-uninstallingamodule" id="modulesandthemescatalog-uninstallingamodule"></a>

**Do not ever delete a module by directly trashing its folder using your FTP client!** You must let PrestaShop take charge of it.

When you need to temporarily stop using a module, but still wish to keep its configuration, you can simply disable it: just click on the "Disable" link. The actions will turn into "Enable" and "Delete", but the "Uninstall" button can still be seen.

If you do not care about the module's configuration, click on the "Uninstall" button: your module's folder will still be in the `/modules` folder, but the module will not have any impact on your shop anymore.\
&#x20;If you wish to entirely remove the module from your server, click the "Delete" link: PrestaShop will get rid of its folder and all its files.

Make sure that the disabling or removal of the module does not break the theme.

### Installing a theme <a href="#modulesandthemescatalog-installingatheme" id="modulesandthemescatalog-installingatheme"></a>

Once you have downloaded a theme from the Addons online store, it's up to you have it installed on your PrestaShop site.

#### Installing using PrestaShop's theme installer

This is the recommended method, as it preserves all the blocks' positions on their respective hooks.

PrestaShop has a native theme importer, which you can reach from the "Themes" page, under the "Preferences" menu. Click the "Add new theme" button at the top of the screen (not the "Add new" button above the list of themes, which is used to create a new theme). This screen presents you with 3 methods to install (or "import") a new module: from your computer, from a public website, or from your own FTP server. It also gives you a method to create a new theme from scratch.

**Importing a theme**

Whatever the method, the process remains the same: indicate the location of the theme's Zip archive, then click "Next".

**Import from your computer**: using the file explorer to find the archive.\
&#x20;**Import from the web**: indicate the direct public URL to the archive.\
&#x20;**Import from FTP**: using your FTP client, upload the archive in the following folder: `/modules/themeinstallator/import/` .

A quick summary is displayed in the next page, indicating what that importer is about to do.

Click "Next" again to validate your choice. The theme is now installed, and PrestaShop asks you if you wish to install modules that were imported along with the theme, what you would rather do with the current modules configuration, and how you would like the images configuration to be taken into account.

Click "Next" one last time. A final confirmation page presents you with all the changes applied to your PrestaShop site. Click "Finish" to end the process.

#### Installing using a FTP client <a href="#modulesandthemescatalog-installingusingaftpclient.1" id="modulesandthemescatalog-installingusingaftpclient.1"></a>

This method is not recommended, but is still available. Use with caution: your blocks might not have the expected position on their respective hooks.

To install a new PrestaShop theme via FTP:

1. Unzip (decompress) the theme archive file (`.zip`). This should result in at least one new local folder, `/themes`, containing your theme's folder(s).
2. Using your FTP client, place the theme's folder (as found in the local `/themes` folder) online in your PrestaShop `/themes` folder. Pay attention NOT to upload that folder in another theme's folder (which can happen when drag-and-dropping items). Upload the whole folder, not just the files it contains.
3. (optional) If the theme's archive contains a second `/modules` folder, it means your new theme comes bundled with modules that are specific to it, or necessary for it to run properly. Using your FTP client, place the folder(s) found in the local `/modules` folder online in your PrestaShop `/modules` folder. If your online PrestaShop install already has a module of the same name, try to only keep the most recent version of the two (the one with the most recent files). If unsure, keep the version bundled with the theme, as it is the most likely to work best with it.
4. Go to your back office, in the "Themes" page under the "Preferences" menu.
5. Select the new theme in place of the current theme, by clicking on the radio button then clicking "Save".
6. Your theme is now in place.
7. (optional) If the theme came with modules, activate them on the back office's "Modules" page, then configure them if need be.

Many themes come with an accompanying `Install.txt` file, which gives you instructions. Make sure to follow them in order to not forget anything.

Once configuration is complete, be sure to test the theme immediately, every page of it, to confirm that it works as planned. Do try to make a full order, from A to Z – you wouldn't want to miss orders just because you didn't notice the theme was incomplete!

### Exporting a theme <a href="#modulesandthemescatalog-exportingatheme" id="modulesandthemescatalog-exportingatheme"></a>

Exporting a theme is very useful when you want either to back the theme up for safety, and create an archive of the theme for a friend or in order to make it available on the Addons marketplace ([http://addons.prestashop.com/](http://addons.prestashop.com/)). Not only does it generate a complete Zip archive of your theme, but it also adds many information in an XML files, which is very useful both when uploading to Addons, and when importing to another PrestaShop site.

Just as for theme importation, there are two ways to export a theme: using PrestaShop's own exporter, or using the one from the Theme Installator module:

* PrestaShop's exporter: click on the "Export theme" button at the top of the "Themes" page (in the "Preferences" menu).
* Theme Installator's exporter: open the module's configuration page, then go to the "Export a theme" section.

Select a theme and click on "Export this theme". A configuration form appears where you can set the exported themes parameters: author, theme name, compatibility version, attached modules (if any), etc.

Once all the parameters are correctly set, click on "Generate the archive now". You will quickly get a file to download from your browser. Save it on your hard-drive, then give the save file a proper name. From there on, you can easily share this theme, and if it is your own creation, you can start selling it on PrestaShop's Addons website at [http://addons.prestashop.com/](http://addons.prestashop.com/).

### PrestaShop's mobile template

The mobile template enables any PrestaShop merchant to have his or her shop be accessible to mobile devices: from the home page to the payment process, along with product pages and conversion funnel.

#### Installing the mobile template for your shop <a href="#modulesandthemescatalog-installingthemobiletemplateforyourshop" id="modulesandthemescatalog-installingthemobiletemplateforyourshop"></a>

Installing PrestaShop's mobile template is easy:

1. Connect to you PrestaShop's administration.
2. Go to the "Themes" page under the "Preferences" menu.
3. In the "Appearance" section, go to the "Enable mobile theme" part and choose one of the three options other than "I want to disable it".

![](<../../../.gitbook/assets/23789642 (2).png>)

By default, the mobile template is only used for mobiles phones, tablet receiving the same theme as regular devices. With this option, you can choose to have the mobile template be used for tablets ("Both" option"), or even choose to only have it used for tablets (mobile phones receiving the regular theme).

#### Customizing the mobile template <a href="#modulesandthemescatalog-customizingthemobiletemplate" id="modulesandthemescatalog-customizingthemobiletemplate"></a>

The mobile template's files are located in the `/mobile` subfolder of the current theme's folder. This way, if you current theme is the default PrestaShop theme, the mobile template's files are in the `/themes/default/mobile` of your PrestaShop installation.

The template is made of HTML, CSS and JavaScript files: its structure is therefore the same as for the default theme, but its design is radically different, as it was built for the smaller screens of mobile devices.

Therefore, if you wish to change the colors or layout of the mobile template's pages, you must edit the CSS and/or HTML files in order to adapt them to your likings. You must have a good knowledge of web programming languages, or ask for help from a web developer.

#### Using the mobile template with another theme <a href="#modulesandthemescatalog-usingthemobiletemplatewithanothertheme" id="modulesandthemescatalog-usingthemobiletemplatewithanothertheme"></a>

The mobile template is only available if the current theme has a `/mobile` subfolder in its own folder. Hence, numerous PrestaShop themes do not have a proper mobile theme, and these themes' users cannot automatically offer a mobile version of their shop to their visitors

While the theme you are using is being updated with its own mobile template, you can use the default mobile template, thanks to a quick file manipulation: you just have to copy the `/mobile` subfolder from the `/themes/default` folder, and paste this subfolder (and all of its files) in your current theme's folder.

You will therefore use the default mobile template rather than a template with a design that is consistent with your main theme, but nothing is stopping you from editing the HTML, CSS or JavaScript files of the mobile template in order to get it closer to your own theme.
