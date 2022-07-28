# Making and restoring your own backup

**Table of contents**

* [Making and restoring your own backup](making-and-restoring-your-own-backup.md#Makingandrestoringyourownbackup-Makingandrestoringyourownbackup)
  * [Making your own backup](making-and-restoring-your-own-backup.md#Makingandrestoringyourownbackup-Makingyourownbackup)
    * [Backing up your files](making-and-restoring-your-own-backup.md#backing-up-your-files)
    * [Backing up your database](making-and-restoring-your-own-backup.md#backing-up-your-database)
      * [Using PrestaShop's DB Backup tool](making-and-restoring-your-own-backup.md#backing-up-your-database)
      * [Using phpMyAdmin](making-and-restoring-your-own-backup.md#backing-up-your-database)
      * [Using your host database tool](making-and-restoring-your-own-backup.md#backing-up-your-database)
  * [Restoring your backup](making-and-restoring-your-own-backup.md#Makingandrestoringyourownbackup-Restoringyourbackup)
    * [Cleaning your server](making-and-restoring-your-own-backup.md#Makingandrestoringyourownbackup-Cleaningyourserver)
      * [Creating a maintenance page](making-and-restoring-your-own-backup.md#Makingandrestoringyourownbackup-Cleaningyourserver)
      * [Deleting files](making-and-restoring-your-own-backup.md#Makingandrestoringyourownbackup-Cleaningyourserver)
      * [Deleting data](making-and-restoring-your-own-backup.md#Makingandrestoringyourownbackup-Cleaningyourserver)
    * [Restoring your files and data](making-and-restoring-your-own-backup.md#Makingandrestoringyourownbackup-Restoringyoufilesanddata)
      * [Restoring your files](making-and-restoring-your-own-backup.md#Makingandrestoringyourownbackup-Restoringyoufilesanddata)
      * [Restoring your data](making-and-restoring-your-own-backup.md#Makingandrestoringyourownbackup-Restoringyoufilesanddata)

## Making and restoring your own backup <a href="#makingandrestoringyourownbackup-makingandrestoringyourownbackup" id="makingandrestoringyourownbackup-makingandrestoringyourownbackup"></a>

Whether you are upgrading your installation of PrestaShop using the automatic method or the manual, you must make sure you have your own set of backup data, one you can rely on and to which you can get back on your own terms.

When performing an upgrade to the store, it is highly advisable to make the backup only after the store has been put in maintenance mode. This way, you are certain that no customer data is lost if you have to revert the upgrade to that backup. Do not perform the upgrade before both files and data have been properly backed up on your computer.

The processes described in this chapter will have you transfer files using an FTP client, download SQL data from a web server using online tools, and even delete all your online files and data. Do not attempt this if you do not have a good grasp of these tools and technologies. If you must (for instance, if your store is broken after a failed upgrade), get assistance from a technical friend, and take the time to perform each step completely. If not, you might lose your store forever.

### Making your own backup <a href="#makingandrestoringyourownbackup-makingyourownbackup" id="makingandrestoringyourownbackup-makingyourownbackup"></a>

First, create a folder on your computer, where you will store both your PrestaShop files and data. Put the current date in the folder's name, in order to know exactly from when that backup is.

#### Backing up your files

This is really easy:

1. Connect to your web server using any FTP client, such as FileZilla.
2. Download all files from PrestaShop's online folder into your local backup folder.

This process may take some time, depending on your server's speed. PrestaShop 1.6 has roughly 10,000 files in 2,500 folders, and that's not counting your own files (product images, themes, modules, etc.), or your visitor's custom images. Let the process go to completion; do not touch your FTP client until it is done.

#### Backing up your database

While the files are being downloaded, you can take the time to back up your data. You have a couple of ways to do that...

**Using PrestaShop's DB Backup tool**

PrestaShop 1.6 has its own backup tool, named "DB Backup" and located in the "Advanced parameters" menu. That tool is explained in details in the "Understanding The Advanced Parameters" chapter of the PrestaShop 1.6 User Guide, but here is the gist of it:

1. Read the disclaimer, and click on the "I have read the disclaimer - Create a new backup". PrestaShop creates a zip archive of all your database tables.
2. Click on the latest backup file in the table below the disclaimer. This should make your browser download the backup archive, typically named like "`1349964600-71d48cfe.sql.bz2`". Save that file in your backup folder.

**Using phpMyAdmin**

If you prefer to trust phpMyAdmin's backup feature rather than PrestaShop's tool, you can! Here is the process to follow:

1. Log into phpMyAdmin on your web server.
2. From the main login screen, select "Databases".
3. Click the name of PrestaShop's database to open it.
4. In the database screen, click the "Export" tab on the top set of tabs.
5. In the export screen:
   1. Make sure all of PrestaShop's tables are selected, and only these. They should start with the `ps_` prefix (or any prefix you have chosen to use when installing PrestaShop).
   2. Make sure the "SQL" radio button is selected.
   3. In the "Structure" section, tick the following boxes:
      * "Structure".
      * "Add DROP TABLE / VIEW / PROCEDURE / FUNCTION".
      * "Add IF NOT EXISTS".
      * "Add AUTO\_INCREMENT".
      * "Enclose table and field names with backquotes".
   4. In the "Data" section, tick at least the following box:
      * "Data".
   5. In the "Save as file" section:
      * Tick "Save as file".
      * Leave the template alone (usually, "`__DB__`").
      * Tick the "zipped" or "gzipped" box, in order to compress the file before downloading it.
   6. Click the "Go" button.
6. The browser should start downloading the data file. Save that file in your computer's backup folder.

If your server is too weak to let you export all your tables at once, break down your backup in several files. For instance, choose the first 20 `ps_` data tables and export those, indicating clearly in the file name that it is the first of several. Once theses tables are backed up and safe on your computer, do the same for the next 20 tables, and so on, not forgetting to indicate their position in the file name.

**Using your host database tool**

Your host might not make phpMyAdmin available to you, and instead might have you use either a custom tool, or any other less known tool, such as the one integrated in cPanel. Read your webhost's documentation. The goal is to get an export if your data in SQL format, either compressed or not.

### Restoring your backup <a href="#makingandrestoringyourownbackup-restoringyourbackup" id="makingandrestoringyourownbackup-restoringyourbackup"></a>

After an automatic upgrade failed (which is the only reason why you should revert said upgrade), if you can still access PrestaShop's administration page and use the 1-Click Upgrade module, use that module's "Revert" tool in order to start the process of restoring both the files and data that it backed up when you started the automatic upgrade. Read the "Automatic update" of this guide for more information on that process.\
If you cannot access the administration or the module, or if you simply did not use the 1-Click Upgrade module to upgrade to the latest version of PrestaShop, then follow the instructions in this section.

One issue with the 1-click Upgrade module is that you have to be connected to the PrestaShop administration if you want to start rolling back to the previous version – and in some unpredictable configurations, the upgrade can prevent you from logging back again, or even render the administration unusable (note: empty the browser's cache and reload the administration several times before you deem it unusable... It might simply be a temporary CSS issue).

This is why the 1-Click Upgrade module insists that you perform your own backups: before attempting any upgrade, you should have on your hard drive an exact copy of your shop. In short:

* A folder (or a zip archive), containing all of PrestaShop's files, especially those specific to your installation: configuration files, themes, modules, images, users uploads, PDF and e-mail templates, custom classes, etc.
* A complete copy of your database, in a raw SQL file or in a zip archive.

This local copy of your site should be extremely recent: at best, it should have been made right after you put PrestaShop in maintenance, and before you started any upgrade script (either automatically or manually). This way, you ensure that you can get back to the most recent version of your shop, and not lose any data (users, sales, stats, etc.).

#### Cleaning your server <a href="#makingandrestoringyourownbackup-cleaningyourserver" id="makingandrestoringyourownbackup-cleaningyourserver"></a>

Now, you have a complete and recent local copy of your shop in its previous version, and your attempt at bringing your online site the latest version of PrestaShop has failed, resulting in a useless administration (the front-end should be inaccessible, since your shop should be in maintenance mode). Going back to the previous version means restoring your local copy on your online server, and that implies starting from a clean slate in order prevent old and new data to mix and further break your site.

This means deleting all the files on your server, and deleting all the data tables in your database.

Do not worry: since all these files and data are already safe and sound on your computer, you will be able to restore them quickly. But since visitors will keep coming to your shop, you have to display a custom maintenance page while you are working to restore your shop.

**Creating a maintenance page**

Reverting your shop to its previous version can take quite some time, depending on how big your store is, and thus on the number of files and the quantity of data you have to transfer. It is therefore important to have a maintenance page that does not depend on PrestaShop.

Indeed, the existing maintenance page relies heavily on PrestaShop to display some information: shop name, shop logo, translation, CSS file, meta data, etc. Even if your shop is currently in maintenance mode, and is therefore displaying the maintenance page to visitors, that page will not work anymore as soon as you delete your data... and it won't even be here as soon as you delete your files, as that page is from the current theme, under the `maintenance.tpl` name.

Hence, the need for a custom maintenance page. It does not have to be fancy or anything, as its role is simply to have a quick message asking visitors to come back later.

Here is a basic example:**Sample maintenance page**

```
<!DOCTYPE html>
<html>
  <head>
    <title>Our shop is under maintenance</title>    
  </head>
  <body>
    <p>In order to perform site maintenance, our online shop has shut down temporarily.</p>
    <p>We apologize for the inconvenience and ask that you please try again later.</p>
  </body>
</html>
```

Copy this code into a `index.html` text file, and upload it in PrestaShop's folder using your FTP client. On most servers, the `index.html` file takes precedence over the `index.php` file, so as you soon as you upload `index.html` to PrestaShop's root folder, your shop should display this maintenance page instead of PrestaShop's one. Check your server's settings to make sure it is so.

**Deleting files**

Connect to your hosting space using your FTP client. Go to PrestaShop's folder (if it is not located at the root), select all the files and folders in PrestaShop's folder (except `index.html`, your custom maintenance page), and delete them all. Obviously, you should only do this if you are certain that you have an exact copy of your files backed up on your computer.

This can take a couple minute, as PrestaShop has more than 7 000 files. While they are being deleted, go delete the data tables (next section).

**Deleting data**

Open your database's manager – usually, your host will provide you with phpMyAdmin or any custom tool. Reach the database for your installation of PrestaShop. Select all the tables which start with `ps_` (or the table prefix you chose when installing PrestaShop); if PrestaShop is the only tool using this database, you can simply click the "Check All" link at the bottom of the tables in order to select all tables quickly.

Then, open the "With selected:" drop down menu at the bottom of the tables, and select "Drop". On the next screen, phpMyAdmin will ask you for a confirmation: click the "Yes" button. Again, you should only do this if you are certain that you have an exact copy of your data tables backed up on your computer.

Let the process happen. Finally, phpMyAdmin will display the database, devoid of any table.

Your server is now empty of any PrestaShop file and data, except for the `index.html` maintenance file. It is now time to put your store back up again, this time with replacement file and data that you know do work!

#### Restoring your files and data <a href="#makingandrestoringyourownbackup-restoringyoufilesanddata" id="makingandrestoringyourownbackup-restoringyoufilesanddata"></a>

As soon as your FTP client is done deleting online files, start uploading the ones that were stored on your computer! As this process can take some time, it is important to not lose some precious minutes (and therefore potential sales) by keeping your shop offline for more time than necessary.

**Restoring your files**

This process is as easy as the one that you followed when backing up your files:

1. Connect to your web server using any FTP client, such as FileZilla.
2. Upload all files from your local backup folder into PrestaShop's online folder.

PrestaShop's online folder should be empty, so as to make sure new and old files do not conflict. If you didn't delete all online files (after you backed them up, of course), you must tell your FTP client to overwrite any existing file. You must not keep any trace of the files from the upgrade that failed.

**Restoring your data**

The process described here uses phpMyAdmin, which is a standard web tool. If you web host makes you use another tool for managing your databases, you will have to adapt this process to that tool. Check your webhost's documentation on the matter.

The data restoration process is as easy as the one you would follow when backing up data:

1. Log into phpMyAdmin on your web server.
2. From the main login screen, select "Databases".
3. Click the name of PrestaShop's database to open.
4. In the database screen, click the "Import" tab on the top set of tabs.
5. In the import screen:
   1. In the "File to import" section, click the "Browse..." button and find your backup file from your data. It can be either the raw SQL text file (`.sql`), or a compressed version of it (`.sql.zip`, `.sql.gzip`, `.sql.tar.gz`, etc.).
   2. In the "Format" section, make sure the "SQL" format is selected.
   3. Click the "Go" button.
6. The browser should start uploading the backup file.

If you have more than one backup data file, import them one after the other.

Finally, remove your maintenance page (named `index.html`). There you go: your shop is back online!
