# Manual update

**Table of content**

* [Manual update](manual-update.md#Manualupdate-Manualupdate)
  * [Quick instructions](manual-update.md#Manualupdate-Quickinstructions)
  * [Step 1 - Save and Backup Your Current Store](manual-update.md#step-1-save-and-backup-your-current-store)
  * [Step 2 - Getting Ready for the New Version](manual-update.md#step-2-getting-ready-for-the-new-version)
  * [Step 3 - Starting the Update](manual-update.md#step-3-starting-the-update)
  * [Step 4 - QA and Testing](manual-update.md#step-4-qa-and-testing)
  * [Step 5 - Starting the Update on your production store](manual-update.md#Manualupdate-Step5-StartingtheUpdateonyourproductionstore)
  * [Step 6 - QA and Testing](manual-update.md#Manualupdate-Step6-QAandTesting)
  * [Step 7 - Activating your store](manual-update.md#Manualupdate-Step7-Activatingyourstore)

**THIS METHOD IS NOW DEPRECATED.**\
**PLEASE USE THE FREE** [**1-CLICK UPGRADE MODULE**](http://addons.prestashop.com/en/administration-tools-prestashop-modules/5496-1-click-upgrade-autoupgrade.html) **INSTEAD.**

Read the [documentation for the automatic upgrade](automatic-update.md), which is the only method that is officially recommended.

## Manual update <a href="#manualupdate-manualupdate" id="manualupdate-manualupdate"></a>

Doing a manual update is a long and detailed process, which should only be used out of necessity – for instance, if you cannot make an automatic update.

Therefore, manual updates should be reserved to experts, meaning those who know how to use development tools such as WAMP, phpMyAdmin, etc. If this is not your case, you should ask a friend or pay a developer to help you. Do anticipate spending one or two hours, maybe more: take the time to do things right.

The idea behind manual update is simple: rather than risking a direct update on your online shop, we are going to do all the work on your computer, using a local PHP/MySQL server such as WAMP or XAMPP. Once the local update is successful, you will have to do it all again, this time online.

From the start of the process, your online shop should be disabled (in "maintenance" mode") so as to make sure that your clients will not lose their carts and orders during the update process. In effect, this means that your shop will be closed for business during the whole process (one to two hours).

### Quick instructions <a href="#manualupdate-quickinstructions" id="manualupdate-quickinstructions"></a>

This short section is aimed at those who are already familiar with installing and updating PHP/MySQL web applications on a server. Should you not feel comfortable with the lack of details, you will find detailed instructions in the sections following this one.

Much of the presented process happens within the confines of a local web server, set up on your own computer. Before you do anything, download and install the local server package of your choice: WAMP, XAMPP, EasyPHP, MAMP, or another. If you have never installed a local server, read the "[What you need to get started](../getting-started/what-you-need-to-get-started.md)" chapter of the Getting Started guide, especially the "[Installing PrestaShop on your computer](../getting-started/installing-prestashop-on-your-computer.md)" section.

The steps of the upgrade process are:

1. Save and Backup Your Current Store:
   * Deactivate your store ("Maintenance" page of the "Preferences" menu).
   * Back up your files to your desktop, using your FTP client in a new "prestashop-prod" folder. This will be a complete copy of your production site.
   * Back up your database ("Advanced Parameters/DB Backup" page, or using phpMyAdmin).
   * Back up your customized translation ("Export a language" section in "Tools/Translations" tab).
2. Getting ready for the new version:
   * Download and unzip the latest version of PrestaShop: [http://www.prestashop.com/en/download](http://www.prestashop.com/en/download), and unpack it in a new "prestashop-prep" folder.
   * Copy your personal files (images, logos, photos, translations, modules, etc.) from "prestashop-prod" to "prestashop-prep" on your computer. A detailed list is available further down in this guide.
   * Copy the "prestashop-prep" folder to the web folder on your local server (`/htdocs`, `/www`, or any other name used by the server package you chose). This is the folder where you will first try to upgrade your PrestaShop, keeping your original backed-up files (prestashop-prod) and the files you prepared (prestashop-prep).
   * Recreate the production database on your local server: using phpMyAdmin, create a local database in which you will put the data from your production shop, using the SQL files that were backed-up at the start of the process.
3. Starting the Local Update:
   * Launch the update script on your local server by accessing it with your browser. In version 1.6, that script is located at `/install/upgrade/upgrade.php`.
   * Verification of all parameters before the update: follow the instructions on screen and make sure your server conforms to the new version technical requirements.
   * Finishing the update: once the updater has finished, delete the `/install` folder and access both your front and back office to make sure it works.
4. QA and Testing:
   * Import your translations ("Import a language pack manually" section in "Localization/Translations" page).
   * Check that your theme is still working as expected. If this is not the case, you will have to edit its files.
   * Test your shop thoroughly: create accounts, buy products, cancel orders, check the invoices, etc.
5. Start the update on your production web server:
   * Using your FTP client, replace the files for your online shop with those from your "prestashop-prep" folder.
   * Launch the update script on your production server by accessing it with your browser. In version 1.6, that script is located at `/install/upgrade/upgrade.php`.
   * Verification of all parameters before the update: follow the instructions on screen and make sure your server conforms to the new version technical requirements.
   * Finishing the update: once the updater has finished, delete the `/install` folder and access both your front and back office to make sure it works.
   * Import your translations ("Import a language pack manually" section in "Localization/Translations" page).
   * Check that the main domain name is correct ("Preferences / SEO & URLs" page, "Shop URL" section).
   * Regenerate your robots.txt files ("Preferences / SEO & URLs" page, "Generate robots.txt" section).
   * Check that your theme still works as expected. If not, you will have to edit its files.
   * Test your store thoroughly: create accounts, buy products, cancel orders, check invoices, etc.
6. Going live with your up-to-date store
   * Activate your store ("Maintenance" page under the "Preferences" menu).

You're done! Enjoy all the new features brought by this update!

### Step 1 – Save and Backup Your Current Store

Caution

Not backing up your store constitutes a very important risk if you encounter any difficulties with the upgrade. You could lose your data and never be able to recover it.

**Do not ever skip this step**. Do not proceed to step 2 unless you are absolutely certain that your backups are completed, successful, and fully functional. Do check several times.

#### Deactivating Your Store <a href="#manualupdate-deactivatingyourstore" id="manualupdate-deactivatingyourstore"></a>

Caution

Disabling your store is **very important**.\
&#x20;By doing so, you make sure that there is no activity on your store while you are updating it. Therefore, if you ever have to revert the update to a backup, however recent, you won't have lost any unfinished carts or orders.

Go to your store's back office, open the "Maintenance" page under the "Preference" menu, then select "No" for the "Enable Shop" option.

If you are updating from PrestaShop 1.4, that setting is directly available in the "Preferences" tab.

In the "Maintenance IP" field, located just below the "Enable Shop" one, enter your own IP address, so that you can keep on using your store during the update. This will allow you to test the front office of your store, while still making sure visitors cannot access the website.\
&#x20;In order to find out your IP address, visit this page: [http://whatismyipaddress.com/](http://whatismyipaddress.com/)

#### Backing Up Your Files <a href="#manualupdate-backingupyourfiles" id="manualupdate-backingupyourfiles"></a>

You must back up all of the files related to your PrestaShop store, and store them on your computer.

There are two main ways of backing up your files:

* **Ask your hosting company to back up your files**.\
  &#x20;Make sure that this backup is fully functional, recent, and more importantly that it reflects the content of your current store.

...or...

* **Copy all of your files from your server to your local computer using an FTP client**.\
  &#x20;This method is only possible if your hosting provider has provided you with an FTP access to your server. Create a "prestashop-prod" folder on the Desktop of your computer, then, using an FTP client (such as the free FileZilla client, which you can download at [http://filezilla-project.org/](http://filezilla-project.org/)), select all the PrestaShop files and folders on your server (use the Ctrl-A command) and copy them to that local "prestashop-prod" folder.

#### Backing Up Your Database <a href="#manualupdate-backingupyourdatabase" id="manualupdate-backingupyourdatabase"></a>

You must absolutely back up the whole database for your PrestaShop store.

There are three different ways to back up your database:

* **Ask you hosting provider to back up your database**.\
  &#x20;Make sure that your database backup is functional, recent, and especially that it contains all of your data for your PrestaShop Store.

...or...

*   **Download a database backup from your PrestaShop back office**.\
    Go to the the "DB Backup" page, then follow the instructions on the page.

    This page is available from:

    * PrestaShop 1.4: under the "Tools" tab, in the "DB Backup" sub-tab.
    * PrestaShop 1.5 and later: under the "Advanced parameters", in the "DB Backup" page.

    This process will take between 1 and 20 minutes depending on the size of your database, after you will see a link appear on the page, titled "Download the Backup file (_size_)". Click it, and make sure this backup is functional, recent, and especially that it contains all the data of your website. Open the zip file and make sure that there are absolutely NO ERRORS in the `.sql` file it contains before proceeding to the next step.

...or...

* **Download a copy of your database via phpMyAdmin**.\
  &#x20;Be sure that your database backup is functional, recent, and especially that it contains all of your data for your PrestaShop Store. If your database is too big, you might receive an error. If that is the case, you will need to contact your hosting provider.

Keep that backup in the "prestashop-prod" folder on your computer, which you should have created in the previous step and should contain your files.

#### Backing up Your Customized Translation <a href="#manualupdate-backingupyourcustomizedtranslation" id="manualupdate-backingupyourcustomizedtranslation"></a>

If you did not edit the available translations or add new ones (either PrestaShop's or your modules'), please proceed to step 2.

To save your translation changes:

1.  Navigate to the "Translations" page in your back office.

    This page is available from:

    * PrestaShop 1.4: under the "Tools" tab, in the "Translations" sub-tab.
    * PrestaShop 1.5 and later: under the "Localization" menu, in the "Translations" page.
2. In the section "Export a Language" select the language to which you have made any modifications, then select your current theme, and click "Export".
3. Save the downloaded file into the "prestashop-prod" folder on your local computer.

Do this for all your custom languages, both those you created/added and those you modified/corrected.

Verify your backup folder

Does the "prestashop-prod" folder contain...

* ...a complete copy of all of the files from your production shop?
* ...a complete and error-less copy of your database?
* ...a copy of your customized translations (optional)?

You have checked the entire backup folder, and made sure that they are all correct and that you would be able to return to your current version / restore all of your data.

If you answered yes to all of the questions above, then proceed to Step 2.

### Step 2 - Getting Ready for the New Version

#### Downloading and Unzipping of the Latest PrestaShop Version <a href="#manualupdate-downloadingandunzippingofthelatestprestashopversion" id="manualupdate-downloadingandunzippingofthelatestprestashopversion"></a>

Visit [http://www.prestashop.com](http://www.prestashop.com) and download the latest version of PrestaShop (click the "Download" button on the homepage, fill in the form then validate).

You now should have a file: `prestashop_1.6.x.zip` (where "x" is a digit of the version number).

Unzip the file to your computer, and place its content in a new "prestashop-prep" that you should level at the same level as your "prestashop-prod" folder (for instance, on your Desktop). This is the folder where you will prepare your files for the coming update.\
&#x20;Caution: make it so that you do not have the `/prestashop` folder from the `.zip` archive at the root of the "prestashop-prep" folder. You should rather directly put the files and folders that it contains, so as to have the same overview for the "prestashop-prod" and "prestashop-prep" folders.

If you do not yet have an unzipping tool, you can download a free one here: [http://www.7-zip.org/](http://www.7-zip.org/).

In that "`/prestashop-prep`" folder, select the "`/admin`" folder and give it the same name as the administration folder of your production store. For instance, if you're "prestashop-prod" uses the name `admin123`, give that same name to the `/admin` folder in your "prestashop-prep" folder.

#### Copying the files that were backed up in "prestashop-prod" to the new "prestashop-prep" folder <a href="#manualupdate-copyingthefilesthatwerebackedupin-prestashop-prod-tothenew-prestashop-prep-folder" id="manualupdate-copyingthefilesthatwerebackedupin-prestashop-prod-tothenew-prestashop-prep-folder"></a>

Now comes the part where you will copy the files that are unique to your production shop into the folders of the new version. In practice, the idea is to build a "prestashop-prep" folder that would contain both the latest version of the standard files for PrestaShop, and all the files that you created and put online since you installed PrestaShop: images, logos, pictures, translations, modules, etc.\
&#x20;This is an important step, because it enables you to safe-keep all the customizations from your store. Take the time to follow these instructions.

You will thus have to browse the folders and files that were stored in the "prestashop-prod" folder in order to access the correct location in the "prestashop-prep" folder.\
&#x20;Answer "Yes" every time the system asks you to replace the existing files.

The following folders must be copied from your "prestashop-prod" folder to the recently unzipped "prestashop-prep" folder:

* **`/mails`**. Has all the mails templates, including those that you have modified.\
  &#x20;If you have never made any mail template modification, do not worry about this folder.
* **`/img`**. Contains your logo and all the pictures of your store (categories, products, etc.). Take good care of these specific files and folders:
  * `logo.jpg` - your store's logo
  * `favicon.ico` - your store's favicon
  * `logo_stores.gif` - your store's logo for the Store Locator's map
  * `/c` - your categories' images
  * `/cms` - your CMS page's images
  * `/co` - your attributes textural colors
  * `/m` - your manufacturers' logos
  * `/p` - your products pictures
  * `/scenes` - your categories' image-maps
  * `/st` - your physical stores' photos
  * `/su` - your suppliers' logos
  * ...basically, copy all folders except `/img/admin` and `/img/jquery-ui`.
* **`/modules`**. Only copy the modules that you have added since you installed PrestaShop for the first (and which where therefore not part of the default installation).
  * Some of these modules might not be currently enabled or even installed: it is up to you to determine whether they are still useful to you, and thus deserve to be copied to the updated installation.
  * Also, do note that you will most probably have to update the modules that were not built with the new PrestaShop version in mind.
* **`/themes/themeName`**. Only copy your current theme.
  * If you use the default theme from PrestaShop (unchanged), do not copy its folder (`/themes/prestashop`): you must use the one from the new version (`/themes/default`).
  * If you have made changes to the default theme, do copy its folder.
* **`/download`** and **`/upload`**. Contain all the downloadable products, the attached files and the customizable products. If you do no use any of these functionalities, do not copy these folders.
*   **`/classes`**. In case you have added customized classes to this folder, copy them to the new `/classes`folder.

    When updating from a version below 1.4, you must manually edit these classes that you have customized. **You do not have to edit classes that you didn't customize**. In order to function properly with the latest version of PrestaShop, all these class files need to have their class name suffixed with "Core". _Do not attempt these if you are not comfortable with PHP files_.\
    &#x20;Here is how to you should edit the customized files that you want to keep:

    1. Copy the class files that you have customized into the `/classes` folder in "prestashop-prep".
    2. Open each and every one of the class files, and find the ones where the class name is not `Core`-suffixed. If you are upgrading from PrestaShop 1.4.x, you shouldn't have any (except for custom classes).
    3. Rename the class name, adding the "Core" suffix. For instance, "`MyClass`" becomes "`MyClassCore`".\
       &#x20;Only change the name in the PHP class within file, not the name of the file itself!
    4. If all the files already have "Core" in their classname (such as "`class AttributeCore extends ObjectModel`"), then you do not need to change anything.
    5. Save the edited files.
* **`/config`**. You only have to copy one file, but **it is essential**: the `settings.inc.php` file.
* `/translations` - if you are using another language than the ones available in the default installation, you will have to copy that language's folder in the `/translations` folder of the new installation. Failing that, the update will not work properly.

Your "prestashop-prep" folder is now ready. You are not to touch it again, and will only work using a copy of it from now on.

#### Moving the "prestashop-prep" folder to your local server <a href="#manualupdate-movingthe-prestashop-prep-foldertoyourlocalserver" id="manualupdate-movingthe-prestashop-prep-foldertoyourlocalserver"></a>

The "prestashop-prep" folder, which you initially unzipped from the archive of the latest PrestaShop version, now contains all of your customizations from the "prestashop-prod" folder (and therefore, from your shop, which is currently running online – and should still be in maintenance mode). In this next step, you will copy this folder to your local web server, in order to test that the update does run without any issue.

Start your local server (WAMP, XAMPP, EasyPHP, MAMP or any other), and make sure that the Apache and MySQL are running.

The main idea here is to locally check that you shop can be update without problem on a local server, in order to minimize the risk of failure when starting the update on your production store. For this reason, you should try to replicate your online environment on your local server, so as to reduce the risk of receiving a bad surprise once you try the update online.

Contact your web host in order to get information about the Apache, PHP and MySQL configuration of your web server, and edit the `httpd.conf` (Apache), `php.ini` (PHP) and/or `my.ini` (MySQL) accordingly, if you can. In the most extreme of cases, you will have to change the version of each of your local server's components in order to replicate the ones from your host.\
&#x20;Once this is done, restart your local server in order for it to take your changes into account.

If you cannot edit the configuration files of your local server, then do note that the differences with your online server can have a huge impact on the smooth running of the update, as that what works in one environment could not work anymore in another. Typically, memory limits and having absolute paths rather than relative ones.

Open the web folder for your local server (`/htdocs`, `/www`, `/web` or another name, depending on the server), and copy the "prestashop-prep" folder into it.

Caution

Do not just move the "prestashop-prep" folder to your local web folder!\
&#x20;Do make sure to copy it, in order to keep the "prestashop-prep" folder untouched.

This way, in case of a problem with the local update, you will be able to open the "prestahop-prep" folder and make the necessary changes, before copying it again into the local web folder and try to update another time.

Put the "prestashop-prep" at the root of the web folder of your local web server.

#### Recreating the production database locally <a href="#manualupdate-recreatingtheproductiondatabaselocally" id="manualupdate-recreatingtheproductiondatabaselocally"></a>

The local files should now be up to date, but the database also needs to be updated. This is what the update script is for. It is part of the files from the new PrestaShop 1.6 version.

You must have a working knowledge of phpMyAdmin before applying the steps of this section.

We are now going to make use of the `.sql` file that you backed up in the "prestashop-prod" folder earlier. Using this file, you will recreate the production database on your local server. In order to do that, simply follow these steps:

1. Open the phpMyAdmin tool, which should be available on your local server. Most of the time, it is located at [http://127.0.0.1/phpmyadmin](http://127.0.0.1/phpmyadmin), or sometimes [http://127.0.0.1/mysql](http://127.0.0.1/mysql).
2. If it is not already the case, create a new database especially for this project. Give it a distinctive name, like "prestashop\_update" or even the database name for your production store, for instance.\
   &#x20;If you have already created a database for a previous local update test, just delete all of its tables.
3. Open de database, and click on the "Import" tab, located at the top of the screen.
4.  Click on the "Browse" button and select the backup `.sql` file from your production store, which should be in the "prestashop-prod" folder.\
    &#x20;Check that the "Max." value displayed by phpMyAdmin is higher than the `.sql` file's size. If not, you will have to edit your local server's `php.ini`, particularly the `upload_max_filesize` value, the `post_max_size` value or even the `memory_limit`value as a last resort. This being done, restart the local Apache and MySQL servers in order to apply your modifications.

    Instead of changing the server settings, you can also try compressing the `.sql` the file using a Zip tool, such as [http://www.7-zip.org/](http://www.7-zip.org/). phpMyAdmin should accept `.sql.zip` files, and will take care of uncompressing the file before importing the data.
5. Click on the "Go" button to import the SQL file's content.

Wait while phpMyAdmin is uploading the file and adding tables to the database. Once it is done, you will see the tables appear in phpMyAdmin's left sidebar.

All that's left to do now is to link your PrestaShop PHP files to the local server's data. To that end, you will have to edit PrestaShop's database information in order to make them target the local database.

Open the `/config/settings.inc.php` file, and edit the following lines:

* `_DB_SERVER_`: replace the MySQL server's address for your production store, with the one for your local server. It should be "localhost" or "127.0.0.1".
* `_DB_NAME_`: replace the name of your production database by the one for the local database in which you have imported your production data tables.
* `_DB_USER_`: replace the username for your production database by the one for your local server. It should probably be "root".
* `_DB_PASSWD_`: replace the MySQL user's password for your production database by the one for your local server's user. It should probably be an empty field: "".

PrestaShop can now access your production database on your local server, all you have to do is to start the update script.

#### Checking everything before going any further <a href="#manualupdate-checkingeverythingbeforegoinganyfurther" id="manualupdate-checkingeverythingbeforegoinganyfurther"></a>

Did you follow these steps?

1. You have downloaded the latest version of PrestaShop.
2. You have unzipped that version, and have stored its files in a new local "prestashop-prep" folder.
3. You have copied your custom files from your local back up ("prestashop-prod") into that "prestashop-prep" folder.
4. You have copied the "prestashop-prep" folder in the web folder on your local server.
5. You have imported the data from your production store in your local MySQL server.
6. You have put the correct local database information in the configuration file.

If you did do all that, then you can continue to Step 3.

### Step 3 – Starting the Update

#### Launching the update script <a href="#manualupdate-launchingtheupdatescript" id="manualupdate-launchingtheupdatescript"></a>

Visit your store's update script URL; for instance: [http://127.0.0.1/prestashop-prep/install/upgrade/upgrade.php](http://127.0.0.1/prestashop-prep/install/upgrade/upgrade.php) (Replace "prestashop-prep" with the actual name of the folder that you have copied in your local server's web folder).

If it returns a 404, then you might not have copied all the files from the latest PrestaShop 1.6 version. Go through this previous step again.

If the address returns a 404 error, you might have forgotten some files from the latest version of PrestaShop 1.6. Do the various steps again: delete the folder which you have copied in the local web folder (but set aside the `settings.inc.php` file so that you won't have to edit it again), edit the content of the "prestashop-prep" folder according to the issue you discovered, and copy "prestashop-prep" again into the local server's web folder.

Once the script is started, **leave your browser alone!** Do not close it or click the "Back" button: the upgrade script is working, it can take several minutes. Let it do the work for you!

For the most part, the update script takes care of updating the SQL database, which can prove a very arduous task in itself. It also handles the update of the `config/settings.inc.php` configuration file, depending on your configuration and environment, as well as other aspects of PrestaShop's inner working.

#### Finishing the local update <a href="#manualupdate-finishingthelocalupdate" id="manualupdate-finishingthelocalupdate"></a>

Once the update is finished, a XML file should be displayed in your browser. This is expected, but can surprise you, since it doesn't look like any regular web page, and each browser has its own way of displaying it. For instance, Firefox will first display a warning message, "This XML file does not appear to have any style information associated with it. The document tree is shown below", above the content of the XML file itself. This will be improved in later versions of the script.

It should begin with the following line:

```
<action result="ok" error="">
```

The "ok" is the important art: it worked! The hardest part is now behind you, now come the final details.

On your local web server, inside the `/prestashop-prep` folder, you should delete:

* The `/install` folder, which contains the install script.
* The `README` files, which contain information about the PrestaShop install.
* The `CHANGELOG` file, which contains information about the latest changes in PrestaShop.

You can now access your local store's address (in our example [http://127.0.0.1/prestashop-prep/](http://127.0.0.1/prestashop-prep/)), which should display the maintenance page with your logo. This is expected, since your store should be in maintenance mode.

If your store's theme does not display, but you instead see a white page with a warning, such as "Your '_theme name_' theme is not available. Please check the name and permissions of the theme folder", then you have forgotten the step where you were supposed to copy your theme over to the `/prestashop-prep` folder.

Go to your "prestashop-prod" folder's `/themes` folder, and copy your theme's folder to the `/themes` in "pretashop-prep". Reload the page to see the maintenance page – or your theme.

If your store's logo does not display, but instead you see a "YourLogoHere" logo, then you have forgotten the step where you were supposed to copy your customized images from the "prestashop-prod" folder over to the "prestashop-prep" folder.

Go to read Step 2 of this chapter ("Step 2 - Getting Ready for the New Version") in order to copy the right files and folders.

Now go to your store's administration page, using your customized `/admin` folder name. You will have to log in using your usual credentials. Browse through the various administration page and check if the content is indeed there and that all the back office pages do work, then take the store out of maintenance mode in order to explore the front office pages the way a regular visitor would, and make sure that they all work.

**If the update fails**

All of the updates do not run smoothly, and for very different reasons. In order to help you, the update script displays an error code at the beginning of the XML result. In case of an error, the page starts like so:

```
<action result="fail" error="27" />
```

As you can see, the "result" attribute does not contain "ok" anymore, but "fail".

Here are some of the most frequent errors:

| Error code | Meaning                                          | Possible solution                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| ---------- | ------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 5          | The configuration file cannot be read.           | Edit the access rights for the `/config/settings.inc.php` files.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| 6          | The configuration file cannot be written.        | Edit the access rights for the `/config/settings.inc.php` files.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| 27         | The installation is too old.                     | You should use the latest version of PrestaShop.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| 28         | You are already using the target version.        | <p>The version to which you are updating is the same as the one that is already installed.<br>If you were trying to update to the latest version of PrestaShop, then do not bother updating. If not, download the latest version.<br><br>This error can also be triggered when you are starting the update test again, after having already tried once. If that's the case, check that the administration does work and indicates the latest version number. If not, use your old backups (files and database) to start anew, and go back to step 1 of the update process.</p> |
| 29         | There is no older version.                       | Have you copied the `config/settings.inc.php` file as is?                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| 31         | SQL update files cannot be found.                | Check that the `/install/upgrade/sql` folder is not empty. If it is, get the SQL update files from the archive of the latest version.                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| 32         | Unable to update.                                | Some files might be missing or badly copied. Restart the whole process from the start.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| 33         | Error while trying to read the SQL update files. | Check that the files are indeed in the `/install/upgrade/sql` folder, and can be read.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| 34         | Internal SQL error.                              | The SQL update files might be corrupted. Download the new version's archive again, and use its files from the `/install/upgrade/sql`.                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| 35         | Cache is enabled.                                | Disable PrestaShop's cache before you start the update script: open the `config/settings.inc.php` file, and check that `define('`_`PS_CACHE_ENABLED`_`', '0');` is indeed set to 0.                                                                                                                                                                                                                                                                                                                                                                                            |

When the update script fails, it is difficult to see if it has been able to make even part of the update. Before you try the update again, you should reset the files and database to their backup state:

* Delete all the files from the local web folder, and replace them with those from the "prestashop-prep" folder, which are pristine because they were kept untouched.
* Delete all the tables from the test database, and replace them with those from the original installation.

### Step 4 - QA and Testing

#### Import your Translations <a href="#manualupdate-importyourtranslations" id="manualupdate-importyourtranslations"></a>

If you did export your custom translations during step 1 (Backups), import them back into your new store by going to the "Localization" menu, then the "Translations" page, then use the "Import a language pack manually" section.

#### Tests to be done on your local test store <a href="#manualupdate-teststobedoneonyourlocalteststore" id="manualupdate-teststobedoneonyourlocalteststore"></a>

To make sure that everything is working properly on your updated local store, you should perform a few tests:

* Make sure all page types load properly (home, categories, products, comparison, CMS, etc.)
* Create a customer account
* Place an order (add to cart and order)
* Verify that payments work properly (credit card, PayPal, etc.)
* In the Back Office, check that the order was properly placed and received
* Send an email from the contact page or "Forgot my password"
* Check the resulting invoice
* Check all the modules that you have activated

This is not a complete list, you should perform as many tests as possible.

If you notice that some aspects of the updated store do not work properly:

1. Edit the content of the "pretashop-prep" folder in order to correct the issues (missing files, wrong configuration, etc.),
2. Restart the process for the local update:
   1. Delete the test sub-folder in the local web folder,
   2. Delete the MySQL tables for your test update,
   3. Copy the "prestashop-prep" files in the local web folder,
   4. Import the backup SQL file from "prestashop-prod" into the local MySQL server,
   5. Restart the update script.

If every test is successful, congratulations! Proceed to step 5.

### Step 5 - Starting the Update on your production store <a href="#manualupdate-step5-startingtheupdateonyourproductionstore" id="manualupdate-step5-startingtheupdateonyourproductionstore"></a>

Now that you've reached this stage, you should have succeeded in updating your shop on your local server. In doing so, you get a better guarantee that performing the update on your web hosting will go smoothly. Your "prestashop-prep" folder contains all the necessary files, because you have changed its content based on issues noticed during your tests from the previous step.

This "guarantee" can never be 100%, as both environments (local server and web hosting) may differ. Your best bet is to set up your local server so that it matches your production server as best as it can.

Your online shop has been in maintenance mode since the beginning of your process, so that you do not lose orders, carts or even new clients during the update. If this is not already the case, turn the store into maintenance mode now, and repeat the process from the beginning - unless you do not fear losing the changes that you made since the beginning.

Other than putting your files online rather than on your local server, the online process varies little from the one that you tested locally:

1. Using your FTP client, replace the files in your online store with those from your "prestashop-prep" folder.\
   &#x20;You should have nothing to worry about, because all your files have been backed up at the beginning of the process in the "prestashop-prod" folder, so you can return to this backup at any time. Ditto for your database, which has also been saved in the "prestashop-prod" folder as `.sql` file.
2. Run the update script on your production shop, by accessing it using your browser. In version 1.6, the script is located at `/install/upgrade/upgrade.php`.
3. Check all settings before updating: Follow the on-screen instructions and make sure that your server meets the technical requirements of the new version.
4. End of update: Once the update is complete, remove the `/install` and browse your front office and your back office to make sure everything works.

### Step 6 - QA and Testing <a href="#manualupdate-step6-qaandtesting" id="manualupdate-step6-qaandtesting"></a>

You need to again perform all the tests already carried out locally, to ensure that nothing fails despite the change from a local environment to a production environment.

#### Import your translations <a href="#manualupdate-importyourtranslations" id="manualupdate-importyourtranslations"></a>

If you did export your custom translations during step 1 (Backups), import them back into your new store by going to the "Localization" menu, then the "Translations" page, then use the "Import a language pack manually" section.

#### Check the main Domain Name <a href="#manualupdate-checkthemaindomainname" id="manualupdate-checkthemaindomainname"></a>

You should verify that the domain name assigned in the database is indeed the one that you are working with. To do so, visit the "Preferences" menu, then the "SEO & URLs" page.

You must check the following information, from the "Set shop URL":

* "Shop domain": This should be the domain name to which you are currently connected. Otherwise, all your links will be invalid and will use an incorrect domain name.
* "Base URI": This folder should be the one that you have transferred onto your FTP server; in this tutorial, it would be `/prestashop/`

If you cannot reach the administration interface, you will have to go through the database management tool used by your web host, such as phpMyAdmin:

1. Open the database for your production store,
2. Open the `ps_shop_url`,
3. Edit the `domain`, `domain_ssl` and `physical_uri` columns so that they match the location of your production store.

As you can see, the address and path to your store are no longer stored in the `/config/settings.inc.php` file from version 1.6, but in the database.

Therefore, you can open the `/config/settings.inc.php` and delete the `define('_`_`PS_BASE_URI`_`_', '/le_chemin_de_la_boutique/');` if the update hasn't taken care of that.

#### Tests to perform on your updated production store <a href="#manualupdate-teststoperformonyourupdatedproductionstore" id="manualupdate-teststoperformonyourupdatedproductionstore"></a>

You must make sure that everything is working properly on your update store. These are a few tests to perform:

* Make sure all page types load properly (home, categories, products, comparison, CMS, etc.)
* Create a customer account
* Place an order (add to cart and order)
* Verify that payments work properly (credit card, PayPal, etc.)
* In the Back Office, check that the order was properly placed and received
* Send an email from the contact page or "Forgot my password"
* Check the resulting invoice
* Check all the modules that you have activated

This is not a complete list; you should perform as many tests as possible.

If you notice that some aspects of the updated store do not work properly:

1. Edit the content of the "pretashop-prep" folder in order to correct the issues (missing files, wrong configuration, etc.),
2. Restart the process for the local update:
   1. Delete the test sub-folder in the local web folder,
   2. Delete the MySQL tables for your test update,
   3. Copy the "prestashop-prep" files in the local web folder,
   4. Import the backup SQL file from "prestashop-prod" into the local MySQL server,
   5. Restart the update script.

If every test is successful, congratulations!

### Step 7 - Activating your store <a href="#manualupdate-step7-activatingyourstore" id="manualupdate-step7-activatingyourstore"></a>

Great! You are now at the end of the update process!

All that's left to do is to re-enable your stop. Go to the "Maintenance" page from the "Preferences" menu, and choose "Yes" for the "Enable Shop".

Go the your store's home page, and browse the pages as if you were a regular visitor, in order to check one final time that everything is working correctly.

You are done! Congratulations on upgrading to the latest and best version of PrestaShop!
