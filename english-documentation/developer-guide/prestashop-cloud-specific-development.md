# PrestaShop Cloud-specific development

PrestaShop Cloud uses the same core architecture as PrestaShop 1.6, so your modules should work as-is.

For information purposes, here are a few tips and information that you might want to know about...

**PrestaShop Cloud-specific development:**

* ****[Validate!](prestashop-cloud-specific-development.md#PrestaShopCloud-specificdevelopment-Validate!)
* [PrestaShop Cloud or not?](prestashop-cloud-specific-development.md#PrestaShopCloud-specificdevelopment-PrestaShopCloudornot?)
* [Dev mode](prestashop-cloud-specific-development.md#PrestaShopCloud-specificdevelopment-Devmode)
* [Read-accessible core files and folders](prestashop-cloud-specific-development.md#PrestaShopCloud-specificdevelopment-Read-accessiblecorefilesandfolders)
* [Read- and write-accessible per-store files and folders:](prestashop-cloud-specific-development.md#PrestaShopCloud-specificdevelopment-Read-andwrite-accessibleper-storefilesandfolders:)
* [Read- and write-accessible per-store files and folders through FTP](prestashop-cloud-specific-development.md#PrestaShopCloud-specificdevelopment-Read-andwrite-accessibleper-storefilesandfoldersthroughFTP)
* [Core modification](prestashop-cloud-specific-development.md#PrestaShopCloud-specificdevelopment-Coremodification)
* [Overrides installation and custom classes](prestashop-cloud-specific-development.md#PrestaShopCloud-specificdevelopment-Overridesinstallationandcustomclasses)
* [Using defines for folders](prestashop-cloud-specific-development.md#PrestaShopCloud-specificdevelopment-Usingdefinesforfolders)
* [Including JavaScript and CSS files](prestashop-cloud-specific-development.md#PrestaShopCloud-specificdevelopment-IncludingJavaScriptandCSSfiles)
* [Using the right protocol](prestashop-cloud-specific-development.md#PrestaShopCloud-specificdevelopment-Usingtherightprotocol)

## Validate! <a href="#prestashopcloud-specificdevelopment-validate" id="prestashopcloud-specificdevelopment-validate"></a>

As always, make sure your module passes the PrestaShop validator before you submit it to Addons!

[https://validator.prestashop.com/](https://validator.prestashop.com/)

## PrestaShop Cloud or not? <a href="#prestashopcloud-specificdevelopment-prestashopcloudornot" id="prestashopcloud-specificdevelopment-prestashopcloudornot"></a>

You can let your module know if it's running on a PrestaShop Cloud store or a regular store:

```
if (defined('_PS_HOST_MODE_'))
	// PrestaShop Cloud store.
else
	// Regular store.
```

## Dev mode <a href="#prestashopcloud-specificdevelopment-devmode" id="prestashopcloud-specificdevelopment-devmode"></a>

To put your store in Dev mode, open the `.htaccess` file and put the `HTTP_PS_MODE_DEV_` constant to `true`. Put it back to `false` once in production.

## Read-accessible core files and folders <a href="#prestashopcloud-specificdevelopment-read-accessiblecorefilesandfolders" id="prestashopcloud-specificdevelopment-read-accessiblecorefilesandfolders"></a>

Here are the files and folders that each PrestaShop Cloud store can read:

* `/backoffice`
* `/classes`
* `/config`
* `/controllers`
* `/css`
* `/docs`
* `error500.html`
* `footer.php`
* `header.php`
* `images.inc.php`
* `/img`
* `index.php`
* `init.php`
* `/js`
* `/tools`
* `/webservice`

## Read- and write-accessible per-store files and folders: <a href="#prestashopcloud-specificdevelopment-read-andwrite-accessibleper-storefilesandfolders" id="prestashopcloud-specificdevelopment-read-andwrite-accessibleper-storefilesandfolders"></a>

Here are the files and folders that each PrestaShop Cloud store can read and edit:

* `/backoffice`
* `/backups`
* `/cache`
* `/config`
* `/download`
* `/export`
* `/import`
* `index.php`
* `init.php`
* `/localization`
* `/log`
* `/mails`
* `/modules`
* `/override`
* `/pdf`
* `/themes`
* `/translations`
* `/upload`

## Read- and write-accessible per-store files and folders through FTP <a href="#prestashopcloud-specificdevelopment-read-andwrite-accessibleper-storefilesandfoldersthroughftp" id="prestashopcloud-specificdevelopment-read-andwrite-accessibleper-storefilesandfoldersthroughftp"></a>

Here are the files and folders than you can access and change through an FTP account:

* `/modules`
* `/override`
* `/themes`
* `.htaccess`

## Core modification <a href="#prestashopcloud-specificdevelopment-coremodification" id="prestashopcloud-specificdevelopment-coremodification"></a>

PrestaShop's core is shared among all the PrestaShop Cloud stores, is only read-accessible for each store. Therefore, it is impossible to modify it.

## Overrides installation and custom classes <a href="#prestashopcloud-specificdevelopment-overridesinstallationandcustomclasses" id="prestashopcloud-specificdevelopment-overridesinstallationandcustomclasses"></a>

_Only use overriding code when really necessary._

Each store has its own `/override` folder. Still, you should not use it for override files that come from a module you wish to install.\
Just follow the regular way of adding overriding classes: [Overriding default behaviors](developer-tutorials/overriding-default-behaviors.md).\
When a module update is available, the override files will be updated as well.

If you wish to manually add a new class for your script (not a module), you can copy it into the correct folder.

## Using defines for folders <a href="#prestashopcloud-specificdevelopment-usingdefinesforfolders" id="prestashopcloud-specificdevelopment-usingdefinesforfolders"></a>

To access the various folders available to core, you have to use the constants listed in `/config/defines.inc.php` and `/config/defines_uri.inc.php`.

## Including JavaScript and CSS files <a href="#prestashopcloud-specificdevelopment-includingjavascriptandcssfiles" id="prestashopcloud-specificdevelopment-includingjavascriptandcssfiles"></a>

Use the methods that are available to core in order to include the various JS and CSS files that are useful to your module:

```
$this->context->controller->addCSS($this->_path.'css/admin.css');
$this->context->controller->addJS($this->_path.'js/admin.js');
```

## Using the right protocol <a href="#prestashopcloud-specificdevelopment-usingtherightprotocol" id="prestashopcloud-specificdevelopment-usingtherightprotocol"></a>

Make sure you use the right protocol to build your URL:

```
Tools::getShopProtocol();
```
