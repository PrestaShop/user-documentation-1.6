# Troubleshooting

**Table of contents**

* [Troubleshooting](troubleshooting.md#Troubleshooting-Troubleshooting)
  * [Turning the error message display on in case of unexpected and persistent blank pages](troubleshooting.md#Troubleshooting-Turningtheerrormessagedisplayonincaseofunexpectedandpersistentblankpages)
  * [Hosted at 1&1: Solving the memory allocation issue](troubleshooting.md#Troubleshooting-Hostedat1&1:Solvingthememoryallocationissue)
  * [It is impossible to connect anymore](troubleshooting.md#Troubleshooting-Itisimpossibletoconnectanymore)
  * [Regenerating a password manually](troubleshooting.md#Troubleshooting-Regeneratingapasswordmanually)
  * [PrestaShop does not send me my new password](troubleshooting.md#Troubleshooting-PrestaShopdoesnotsendmemynewpassword)
  * [Logging in after mistakenly deleting the default language pack](troubleshooting.md#Troubleshooting-Logginginaftermistakenlydeletingthedefaultlanguagepack)

## Troubleshooting <a href="#troubleshooting-troubleshooting" id="troubleshooting-troubleshooting"></a>

### Turning the error message display on in case of unexpected and persistent blank pages <a href="#troubleshooting-turningtheerrormessagedisplayonincaseofunexpectedandpersistentblankpages" id="troubleshooting-turningtheerrormessagedisplayonincaseofunexpectedandpersistentblankpages"></a>

Module

For PrestaShop 1.6 and higher you can use a module: [https://www.prestashop.com/forums/topic/513401-free-module-enable-debug-mode-from-back-office/](https://www.prestashop.com/forums/topic/513401-free-module-enable-debug-mode-from-back-office/)

If your back office and/or front office start displaying a blank or incomplete page regularly without any error message, it is necessary to activate the display of the PHP errors in order to understand the problem.

This is done in your PrestaShop installation's `/config/defines.inc.php` file. You should edit the following line:

```
define('_PS_MODE_DEV_', false);
```

...and change it into:

```
define('_PS_MODE_DEV_', true);
```

Now browse your store's pages again. PrestaShop will display all the relevant error messages (if any), which should help you solve the issue.

Once the issue has been fixed, you must revert your changes: edit the `/config/defines.inc.php` file again and put false back as the value for the `_PS_MODE_DEV_` constant.

### Hosted at 1&1: Solving the memory allocation issue <a href="#troubleshooting-hostedat1-and-1-solvingthememoryallocationissue" id="troubleshooting-hostedat1-and-1-solvingthememoryallocationissue"></a>

Some people may encounter memory allocation issues, particularly when the back office tries to display images which are quite big in the disk (over 800 Kb). You should know that even if you manually increase the hosting memory limit to 128 Mb, some web hosts, such as 1&1, will keep the limit at 32 Mb. See this FAQ from 1&1: [http://faq.oneandone.co.uk/scripting/php/10.html](http://faq.oneandone.co.uk/scripting/php/10.html).

There are only two solutions, and they are both drastic:

* Decrease the size of your pictures in pixels, and thus their size on the disk. This will also most probably improve the overall performance.
* Change host for one that support memory increase.

### It is impossible to connect anymore <a href="#troubleshooting-itisimpossibletoconnectanymore" id="troubleshooting-itisimpossibletoconnectanymore"></a>

There are cases when PrestaShop will not recognize a user's e-mail or password, making it impossible to connect to either the back office and the front office. The user is simply sent back to the login screen. Some reports tend to point that IE10 is the only browser where this happens.

This is most probably an issue with the user's browser cookie for your store: when the user repeatedly logs in and out of the store, the cookie's encryption keys can get mixed up.

In any case, one easy way to fix this and to be able to log in again is to clear the browser's cache and cookies. Here is page explaining how to do just that, depending on the browser: [https://support.google.com/mail/answer/32050?hl=en](https://support.google.com/mail/answer/32050?hl=en).

### Regenerating a password manually <a href="#troubleshooting-regeneratingapasswordmanually" id="troubleshooting-regeneratingapasswordmanually"></a>

There are situations where nothing happens when you request a new password, and it doesn't work. There can be a number of reasons why this would happen, but the important thing is to be able to log in again.

This is will require you to access your database, using phpMyAdmin for instance.

You will have to follow the following procedure:

1. Open the `/config/settings.inc.php` file, from your shop's root directory. Find the line containing "`_COOKIE_KEY`\_". Copy the cookie content (without the quotes): it is the MD5 for your original password.
2. You now need to generate a new MD5 hash for your password:
   1. Go to [http://www.miraclesalad.com/webtools/md5.php](http://www.miraclesalad.com/webtools/md5.php).
   2. Paste the value of "`_COOKIE_KEY`\_" in the text-field, and right after it, add your desired password. For instance, xykxB41JrEacRIoZxDioPNRmKeuO3ixCLygNxBAkeOkAHf2YUVESuT9jMYPASSWORD, where the cookie ends with T9j, and the desired password is MYPASSWORD (it can be anything you want).
   3. Click on the "md5" button: this will produce a MD5 hash of the text-field's content. Copy it.
3. You now need to put this hash into your database:
   1. Open you shop's database using phpMyAdmin. If you don't know how to use phpMyAdmin, ask your webmaster, or your host.
   2. Open the `pw_employee` table, find the row corresponding to your account (it should feature your first name, last name, and e-mail address), and click its "Edit" button.
   3. Find the `passwd` field, and paste in the MD5 that you just generated.
4. Log in to your back office with the email listed in the same table, and the desired password that you used above (MYPASSWORD). This will generate a new cookie key.

If it still doesn't work, use phpMyAdmin to access the `ps_shop_url` table and check the value of the main shop, whose `id` is 1. It should contain the shop's file path:

* If your shop is at the root of the server, this variable should contain "`/`".
* If your shop is in a sub-directory, it should contain it. For instance, if it's at "[http://www.mywebsite/shop/](http://www.mywebsite/shop/)", then the variable should contain "/shop/".

If all fails, contact the PrestaShop support team at [http://support.prestashop.com/en/](http://support.prestashop.com/en/).

### PrestaShop does not send me my new password <a href="#troubleshooting-prestashopdoesnotsendmemynewpassword" id="troubleshooting-prestashopdoesnotsendmemynewpassword"></a>

The request to reset the password only works if the SMTP server has been configured so that PrestaShop is able to send emails.

Two solutions present themselves to you:

1. **Configure the SMTP server to send emails**:\

   1. Get information for SMTP connection from your hosting provider.
   2. Go to your back office (either you or an administrator who can still log) "E-Mails" page, in the "Advanced parameters" menu.
   3. Select the "Use my own SMTP settings" option. A form will appear: fill it with the information given by your host.
   4. Save your changes.
   5. Request a new password once again. You should receive it.
2. **Follow these steps**:
   1. Choose a new password. In our example, "\$$$rabbit$159\$$$".
   2. Using your FTP client, open the `login.php` file, located in your administration folder online (the name of which depends on your installation).\
      &#x20;At the bottom of the file, add the following line:\
      &#x20;`echo md5( PSQL( _COOKIE_KEY_ . 'newpassword' ) );`\
      &#x20;So with our example password:\
      &#x20;`echo md5( PSQL( _COOKIE_KEY_ . '$$$rabbit$159$$$' ) );`\
      &#x20;Remember to put your own new password!
3. Go to the login screen to the back office, as if you wanted to log in, and copy the text that appears at the bottom of the page (e.g.: a0ee884b507dd4624ce51968cfbb19a9).
4. Go to the PrestaShop database, for example using phpMyAdmin. In the `ps_employee` table, replace the existing value in the `passwd` column for the employee of which you want to change the password with the value obtained in the previous step. Save your changes.
5. You can now connect with the usual username and new password.

### Logging in after mistakenly deleting the default language pack <a href="#troubleshooting-logginginaftermistakenlydeletingthedefaultlanguagepack" id="troubleshooting-logginginaftermistakenlydeletingthedefaultlanguagepack"></a>

In the event that you deleted the default language pack from your shop install, you can have issues connecting to your back office again.

Here how to solve this if the default language was English:

1. Go to phpMyAdmin. If you cannot access it, ask your host to perform these actions.
2. Select your shop's database, and select the `ps_lang` table.
3. Click the "Insert" button at the top, and create a new entry with these values:
   * `id_lang` -> 1
   * `name` -> English
   * `active` -> 1
   * `iso_code` -> en
   * `language_code` -> en
   * `date_format_lite` -> Y-m-d
   * `date_format_full` -> Y-m-d H:i:s
   * `is_rtl` -> 0
4. Execute the query.

You should be able to log in again.
