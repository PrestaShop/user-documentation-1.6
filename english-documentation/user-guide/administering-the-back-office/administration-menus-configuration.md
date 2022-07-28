# Administration Menus Configuration

PrestaShop's back office menu organization is not set in stone: while the default arrangement is built in order to have the most useful pages readily available, you might have a different opinion, and may want to change the organization, in part or in full.

This administration page enables you to move, edit, disable and even create pages.

![](<../../../.gitbook/assets/43417616 (1).png>)

## Moving menus <a href="#administrationmenusconfiguration-movingmenus" id="administrationmenusconfiguration-movingmenus"></a>

Menus can be moved directly from the list. You can either click on the arrows in the "Position" column, or drag the row itself and drop it in the position you want it to have. As soon as you drop the row, PrestaShop saves the location automatically. You can drag the row when the mouse cursor is over the "Position" column.

You can disable a menu simply by clicking on the green "Yes" in the "Enabled" column. Note that this will disable the menu for all back office users. If you want to hide a menu from a specific set of users, edit their profile's permissions, in the "Permissions" administration page.

## Moving pages <a href="#administrationmenusconfiguration-movingpages" id="administrationmenusconfiguration-movingpages"></a>

To access a menu's pages, click the "Details" action in the action menu. A new list appears with the pages in that menu, with the same columns.

Pages can be moved within a menu directly from the list. You can either click on the arrows in the "Position" column, or drag the row itself and drop it in the position you want it to have. As soon as you drop the row, PrestaShop saves the location automatically. You can drag the row when the mouse cursor is over the "Position" column.

You can also move a page to a different menu altogether. This cannot be done directly from the list; you must open the page's editing form, where you will find the "Parent" option. Change that option to another menu name, save your changes, and when returning to the "Menus" page, the page will have moved menu.

You can disable a page simply by clicking on the green "Yes" in the "Enabled" column. Note that this will disable the page for all back office users. If you want to hide a page from a specific set of users, edit their profile's permissions, in the "Permissions" administration page.

## Creating a new page or menu <a href="#administrationmenusconfiguration-creatinganewpageormenu" id="administrationmenusconfiguration-creatinganewpageormenu"></a>

Click on the "Add New Menu" button to reach the page creation form.

![](<../../../.gitbook/assets/43417617 (1).png>)

This form has a handful option, some of which might prove complicated:

* **Name**. Give it a unique name, because it will serve as an internal identifier.
* **Class**. In short, a PrestaShop back office page is based on specific internal PHP files, which are called "admin controllers", and are most often stored in the `/controllers/admin` folder of your PrestaShop installation. When creating a new page, you must know which controller to target, and most importantly the name of its class – which is the name of its PHP file.\
  &#x20;For instance, if you want to create a page displaying PrestaShop's backup administration page, you must first find its controller name (in this case, `AdminBackupController`), and copy it in the "Class" field.
* **Module**. In some cases, the administration controller for which you want to create a page comes from a module. In that case, you must also indicate the identifier for the module (in most cases, its folder name) and copy it in the "Module" field, in lowercase. This way, PrestaShop will know that it should not look for the controller in the `/controllers/admin` folder, but rather in the `/modules/NAME-OF-THE-MODULE/` folder.
* **Status**. You can disable a page at any time, but do note that it affects all the back office users.
* **Parent**. You can choose any menu, but for consistency's sake, make sure to pick one to which the page you are creating is relevant.

If you want to create a new menu page, choose "Home" as the parent.
