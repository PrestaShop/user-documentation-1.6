# Misc. information

**Table of content**

* [Misc. information](misc.-information.md#Misc.information-Misc.information)
  * [Keep a test version at hand!](misc.-information.md#Misc.information-Keepatestversionathand!)
  * [Checking for the GD library](misc.-information.md#Misc.information-CheckingfortheGDlibrary)
  * [Activating PHP5](misc.-information.md#Misc.information-ActivatingPHP5)
    * [1&1](misc.-information.md#Misc.information-1&1)
    * [Free.fr](misc.-information.md#Misc.information-Free.fr)
    * [OVH](misc.-information.md#Misc.information-OVH)
    * [GoDaddy](misc.-information.md#Misc.information-GoDaddy)
    * [Lunarpages shared hosting](misc.-information.md#Misc.information-Lunarpagessharedhosting)

## Misc. information <a href="#misc.information-misc.information" id="misc.information-misc.information"></a>

### Keep a test version at hand! <a href="#misc.information-keepatestversionathand" id="misc.information-keepatestversionathand"></a>

After you have completed setting up your shop to get it just the way you want it, but before officially opening it to the buying public, we **strongly** recommend that you install a local test version on your personal computer (using [WAMP](http://en.wikipedia.org/wiki/Comparison\_of\_WAMPs) for Windows, [MAMP](http://en.wikipedia.org/wiki/MAMP) for Mac, or [LAMP](http://en.wikipedia.org/wiki/LAMP\_\(software\_bundle) for Linux, or [XAMPP](http://www.apachefriends.org/en/xampp.html) for any of those platforms), or elsewhere on your hosting server.

This second instance will be useful as a pre-production environment in which you can carry out all future changes to your PrestaShop online store, without affecting the live version. This way, if an error should occur, your live store remains intact and untouched.

After you have confirmed that your test version works as it should, copy the test version over the live version. It is best to do this after peak usage hours, and with your store properly and temporarily disabled from within the PrestaShop back office.

### Checking for the GD library <a href="#misc.information-checkingforthegdlibrary" id="misc.information-checkingforthegdlibrary"></a>

The [GD library](http://www.boutell.com/gd/) enables PrestaShop to rework images that you upload, especially resizing them.

On a default installation of PHP, the GD Library should be turned on, but if that's not the case for your install, the standard Windows instructions are:

1. In the root directory of your PHP folder, open the `php.ini` file.
2. Uncomment the `extension=php_gd2.dll` line (about half-way through the file, in the middle of a long list of extensions) by deleting the ";" at the start of the line.
3. Restart the PHP services.

If you have no access to the `php.ini` file (which is often the case in shared hosting), contact your host about your hosting needs.

### Activating PHP5 <a href="#misc.information-activatingphp5" id="misc.information-activatingphp5"></a>

Oftentimes, dedicated or shared servers have both PHP 4 and PHP 5 available, but only PHP4 is activated by default.

To install PrestaShop, PHP 5 must be activated. If you attempt to run PrestaShop using PHP 4, you will receive numerous errors, including this very common message:

```
Parse error: parse error, unexpected T_STATIC, expecting T_OLD_FUNCTION or T_FUNCTION or T_VAR or '}' in [php file] on line X.
```

Please do not hesitate to post a bug report concerning the tips needed to make PrestaShop run on your hosting service, on PrestaShop's [Forge](http://forge.prestashop.com/) (you will need an account). We will add them to this guide as we receive them.

The following is a list of procedures of which we are currently aware of...

#### 1&1 <a href="#misc.information-1-and-1" id="misc.information-1-and-1"></a>

Add this line to your `.htaccess` file:

```
AddType x-mapp-php5 .php
```

For URL re-writing, add these lines:

```
Options +FollowSymLinks
RewriteEngine On
```

#### Free.fr <a href="#misc.information-free.fr" id="misc.information-free.fr"></a>

Add this line to your `.htaccess` file:

```
php 1
```

#### OVH <a href="#misc.information-ovh" id="misc.information-ovh"></a>

Add this line to your `.htaccess` file:

```
SetEnv PHP_VER 5
```

To deactivate global registers:

```
SetEnv REGISTER_GLOBALS 0
```

#### GoDaddy <a href="#misc.information-godaddy" id="misc.information-godaddy"></a>

To View Your PHP Version:

1. Log in to your Account Manager.
2. From the Products section, click Web Hosting.
3. Next to the hosting account you want to use, click Launch.

In the Server section, your PHP Version displays.

To Change Your PHP Version:

1. From the Content menu, select Programming Languages.
2. Select the PHP version you want to use, and then click Continue.
3. Click Update.

Changes can take up to 24 hours to complete.

#### Lunarpages shared hosting <a href="#misc.information-lunarpagessharedhosting" id="misc.information-lunarpagessharedhosting"></a>

1. Enter cPanel. It should be located at [http://www.(your\_domain).(com/net/org/etc)/cpanel](http://www.\(your\_domain\).\(com/net/org/etc\)/cpanel)
2. Enter your account username and password in the box that appears.
3. A new page appears. Go to the bottom row of icons in the page and click the icon titled "Enable/Disable PHP 5"
4. A new page appears. Click "Add PHP 5 To Your Account!".

Your language change request is submitted. Please allow up to 24 hours for the change to be processed by the hosting server.
