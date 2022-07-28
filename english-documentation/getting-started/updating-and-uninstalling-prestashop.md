# Updating and Uninstalling PrestaShop

**Table of content**

* [Updating PrestaShop](updating-and-uninstalling-prestashop.md#UpdatingandUninstallingPrestaShop-UpdatingPrestaShop)
* [Uninstalling PrestaShop](updating-and-uninstalling-prestashop.md#UpdatingandUninstallingPrestaShop-UninstallingPrestaShop)

## Updating PrestaShop <a href="#updatinganduninstallingprestashop-updatingprestashop" id="updatinganduninstallingprestashop-updatingprestashop"></a>

We have a dedicated guide for that: [Updating PrestaShop](../updating-prestashop/).

## Uninstalling PrestaShop <a href="#updatinganduninstallingprestashop-uninstallingprestashop" id="updatinganduninstallingprestashop-uninstallingprestashop"></a>

PrestaShop is very easy to uninstall:

1. Delete all of PrestaShop's files and folders on your webserver, using your FTP client.
2. Delete all the `ps_` tables from PrestaShop's database, using phpMyAdmin.

You will lose all information registered to your store: customers, orders, invoices, products, etc.\
&#x20;This cannot be undone, unless you have proper backups of all your data.
