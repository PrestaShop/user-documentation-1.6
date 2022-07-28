# Updating PrestaShop

**Table of contents**

* [Updating PrestaShop](./#UpdatingPrestaShop-UpdatingPrestaShop)
  * [Backup and issues](./#UpdatingPrestaShop-Backupandissues)
  * [PrestaShop support](./#UpdatingPrestaShop-PrestaShopsupport)
  * [Checking the requirements for the new version](./#UpdatingPrestaShop-Checkingtherequirementsforthenewversion)
  * [For those upgrading from a version below 1.4.x](./#UpdatingPrestaShop-Forthoseupgradingfromaversionbelow1.4.x)

## Updating PrestaShop <a href="#updatingprestashop-updatingprestashop" id="updatingprestashop-updatingprestashop"></a>

New versions of PrestaShop come every few months, sometimes even weeks apart. Some are major, most are minor, but they all bring a slew of innovations, improvements and bug fixes. It is therefore highly advised to keep up with the latest version.

There are two ways to upgrade PrestaShop:

* [Automatic](automatic-update.md)
* [Manual](manual-update.md)

The automatic upgrade simply uses the free [1-Click Upgrade module](http://addons.prestashop.com/en/administration-tools-prestashop-modules/5496-1-click-upgrade-autoupgrade.html).

The manual upgrade has been deprecated, but its documentation is kept for historical purposes – and for those who cannot use the automatic upgrade.

The update process will affect all files and folders included in the main PrestaShop installation. This includes all the core files used to run PrestaShop, all default modules and the default theme. If you have made any modifications to those files, your changes will be lost.

Done well, the whole update process described within these pages should not take more than half an hour. Do not try to skip a step in order to be done with it faster, as all steps are crucial.

### Backup and issues <a href="#updatingprestashop-backupandissues" id="updatingprestashop-backupandissues"></a>

In case anything goes wrong, you should learn how to [backup your data and how to restore it](making-and-restoring-your-own-backup.md).

If you need help for other issues, [read this page](in-case-of-issues.md).  &#x20;

### PrestaShop support <a href="#updatingprestashop-prestashopsupport" id="updatingprestashop-prestashopsupport"></a>

For any **support request** or **help to setup your website**, contact us and discover our support offers:

* By e-mail: use the contact form at [https://www.prestashop.com/en/support](https://www.prestashop.com/en/support)
* By phone ([9 am – 6 pm Central European Time (Paris)](http://www.timeanddate.com/worldclock/france/paris)):
  * \+33.1 40 18 30 04 if you need advices on how to improve your store (free)
  * \+33.8 90 03 23 20 if you have support questions (0.80€ / min)
* Learn more about our support offers: [http://addons.prestashop.com/en/388-support](http://addons.prestashop.com/en/388-support)
* And the ever-helpful [community forums](http://www.prestashop.com/forums/)

### Checking the requirements for the new version <a href="#updatingprestashop-checkingtherequirementsforthenewversion" id="updatingprestashop-checkingtherequirementsforthenewversion"></a>

Before you do anything to your current installation of PrestaShop, you should check that your server configuration matches or exceeds the minimum requirements for the latest version of PrestaShop, which are indicated on this page: [http://www.prestashop.com/en/system-requirements](http://www.prestashop.com/en/system-requirements).\
For instance, make sure that your web host does provide you with the required versions of PHP and MySQL. If not, ask your host to update the server configuration. If you are unsure which PHP and MySQL versions you are using, ask your web host.

If you web host won't update your server configuration, then it is time for you to find a better host. Do NOT perform any upgrade unless your server at least meets the system requirements.

### For those upgrading from a version below 1.4.x <a href="#updatingprestashop-forthoseupgradingfromaversionbelow1.4.x" id="updatingprestashop-forthoseupgradingfromaversionbelow1.4.x"></a>

Older versions of PrestaShop might not make it as easy to upgrade to the latest version: the code base is quite different, many files have been moved around, many have been created, and others have been deleted. Therefore, the risk is high, when skipping from a very old version to the latest one, to see errors and mistakes aplenty.

You are also limited to the [manual upgrade process](manual-update.md): the 1-Click Upgrade module can only work with PrestaShop 1.4 and later versions.

You should therefore be even more careful. The older your version is, the more you should pay attention to details: backups, custom files, edited theme, etc.
