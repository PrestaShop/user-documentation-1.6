# In case of issues

**In case of issues:**&#x20;

* ****[Administration display is wonky](in-case-of-issues.md#Incaseofissues-Administrationdisplayiswonky)
* [Module page is not updated](in-case-of-issues.md#Incaseofissues-Modulepageisnotupdated)
* [Default theme is not working anymore](in-case-of-issues.md#Incaseofissues-Defaultthemeisnotworkinganymore)
* [Some modules are not working](in-case-of-issues.md#Incaseofissues-Somemodulesarenotworking)
* [Incompatible module](in-case-of-issues.md#Incaseofissues-Incompatiblemodule)
* [Homefeatured module has a broken design](in-case-of-issues.md#Incaseofissues-Homefeaturedmodulehasabrokendesign)
* [Rolling back your database](in-case-of-issues.md#Incaseofissues-Rollingbackyourdatabase)
* [Contact us](in-case-of-issues.md#Incaseofissues-Contactus)

## Administration display is wonky <a href="#incaseofissues-administrationdisplayiswonky" id="incaseofissues-administrationdisplayiswonky"></a>

On first load after making the upgrade, administration pages might look weird: because your web browser caches files, it is probably using the old CSS and JavaScript files instead of the new ones.

You must reload the page several times, or even empty your browser's cache, in order to get the correct interface. Read how to clear your cache here: [http://support.google.com/accounts/bin/answer.py?hl=en\&answer=32050](http://support.google.com/accounts/bin/answer.py?hl=en\&answer=32050).

## Module page is not updated <a href="#incaseofissues-modulepageisnotupdated" id="incaseofissues-modulepageisnotupdated"></a>

Reloading the page twice (press F5) should fix the issue

## Default theme is not working anymore <a href="#incaseofissues-defaultthemeisnotworkinganymore" id="incaseofissues-defaultthemeisnotworkinganymore"></a>

The name of the default theme has been changed from "prestashop" to "default". If you were using the default theme, rename the default theme's folder from "default" to "prestashop", and everything should work again. You can find that folder in your `/themes` folder.

## Some modules are not working <a href="#incaseofissues-somemodulesarenotworking" id="incaseofissues-somemodulesarenotworking"></a>

When an installed module is not giving the expected result, try uninstalling it, then install it again.

## Incompatible module <a href="#incaseofissues-incompatiblemodule" id="incaseofissues-incompatiblemodule"></a>

In some cases, modules may not be compatible with the latest version of PrestaShop. You should contact the company / person that provided you with this module to request a few code changes to bring it up to date.

## Homefeatured module has a broken design <a href="#incaseofissues-homefeaturedmodulehasabrokendesign" id="incaseofissues-homefeaturedmodulehasabrokendesign"></a>

If your home-page is broken because the Feature Products block has its items stacked in a single column, then you should reinstall the Features Products module (from the Front-end Features category of modules).

## Rolling back your database <a href="#incaseofissues-rollingbackyourdatabase" id="incaseofissues-rollingbackyourdatabase"></a>

Only proceed to this step if you have no other way out.

If your update went bad and you do not see any other fix than to roll back to the previous version of your database, there are two main ways of doing so:

* Ask your hosting provider to restore the back up for you.\
  &#x20;Make sure to provide them with the latest backup that you have done during Step 1 of the upgrade process!

...or...

* Import your backed-up data via phpMyAdmin\
  &#x20;This is typically done by the database tools provided to you by your hosting provider, most often phpMyAdmin, with export and import features.\
  &#x20;If the size of your database is too big, you might encounter an error message. If so, you might need to ask your hosting provider for help by changing the size of the database maximum upload.

You will find the backup data under the `/admin/backups` folder.\
&#x20;You can also download the database from within your back office. Open the "DB Backup" page from the "Advanced Parameters" menu. Select your latest database backup and download it to your computer by clicking on it. It should typically take between 1 and 20 minutes to download.

## Contact us <a href="#incaseofissues-contactus" id="incaseofissues-contactus"></a>

For any **support request** or **help to setup your website**, contact us and discover our support offers.

Our support team is at your disposal for any technical detail pertaining to updating your shop to the latest PrestaShop version.

* By e-mail: [support@prestashop.com](mailto:support@prestashop.com)
* By phone: +33.1 83 64 16 54 (9 am – 6 pm Central European Time)
* [http://support.prestashop.com](http://support.prestashop.com)
* And the ever-helping community forums: [http://www.prestashop.com/forums/](http://www.prestashop.com/forums/)
