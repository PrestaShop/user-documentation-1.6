# Translations

PrestaShop provides you with full translation tool for your shop. This helps you add and edit your pages translations. This way, you are the master of your shop, and can handle your translated strings without having to wait for official translators to publish their corrections.

Even if you do not want to correct the translators' work, you might want to change the wording they chose to use (less formal, less wordy, etc.), and customize the various available text, thus tailoring your website to your audience; for instance, a hip-hop clothing shop might be better off using different expressions from that of a luxury watches shop.

The process of adapting a program to foreign languages is called _internationalization and localization_, or i18n and L10n for short.\
&#x20;Internationalization is the first step, where developers choose a mechanism for the translation of the software. All the strings of the software are then converted to make use of this mechanism.\
&#x20;Localization is the second step, where bi- or multi-lingual users of the software actually translate the original strings into their own language. Localization may also include providing local data in order to further improve the software for local users.\
&#x20;You can learn more about i18n and L10n at this Wikipedia page: [http://en.wikipedia.org/wiki/Internationalization\_and\_localization](http://en.wikipedia.org/wiki/Internationalization\_and\_localization)

The PrestaShop team has chosen to use its own built-in translation tool, so that anyone with a PrestaShop installation may customize their shop to their needs.\
&#x20;The community translation is done with an online tool, located at [https://crowdin.net/project/prestashop-official](https://crowdin.net/project/prestashop-official).

The official translation packs can be downloaded manually from this address: [http://www.prestashop.com/en/translations](http://www.prestashop.com/en/translations).

## Modifying a Translation <a href="#translations-modifyingatranslation" id="translations-modifyingatranslation"></a>

The most important tool of the "Translation" page is in the "Modify translations" section. This is where you can choose to edit a translation, and completely customize each and every sentence if you wish so.

![](<../../../.gitbook/assets/23789736 (1).png>)

Select the part of the current translation that you wish to edit:

* **Front Office translations**. The text visible to your customers when browsing your store.
* **Back Office translations**. The text visible to you and your team from your store's administration panel.
* **Error message translations**. The error messages that may appear on the front-office.
* **Fields Names translations**. The name of the fields in both the front-office and back office.
* **Module translations**. The terms used by the installed modules. Note that modules which are available but not installed will not appear in the tool.
* **PDF translations**. The terms used in the generated PDF files: invoices, delivery slips, etc.
* **E-mail template translations**. The terms used in the default e-mail templates.

Some categories have a second drop-down list, which lists the available themes. PrestaShop themes have their own strings, but can also have their own modules, PDF templates and e-mail templates. The drop-down list therefore enables you to choose which theme you want to work with.

Once your selection is done, click the language code of the language in which you wish to edit that category of translation.

A long page then appears. It contains the hundreds of available strings for that category, sometimes split in tens of fieldsets.

![](<../../../.gitbook/assets/23789738 (1).png>)

By default, only the fieldsets which have untranslated strings are open. If you wish to open them all, click on the button on the top left twice: once to close all of them, once more to expand them all. You can open and close fieldsets one by one by clicking on its title.

Editing a translation is easy:

* Open a fieldset,
* Edit its content,
* Click on either the "Update Translations and stay" button to save while and keep translating more for this category, or on the "Update translation" button to save and return to the main "Translations" page.

PrestaShop 1.5 introduced a new syntax where strings can contain placeholders, such as `%s`, `%d`, `%1$s`, `%2$d`, etc.

When you find a string with such placeholder, it means that PrestaShop will replace it with an actual dynamic value before displaying the translated string.\
&#x20;For instance, in the string "Your order on %s is complete", `%s` will be replaced by the shop's name. Therefore you should keep it in your final translation; for instance, in French, the translation would be "Votre commande sur %s a bien été enregistrée."

Technically, having placeholders prevents strings from being split in parts. Thereby, in previous version of PrestaShop, "Your order on %s is complete." would have been split in two: "Your order on" and "is complete.". While the literal translation of these worked for some language, it made translation nearly impossible for many other languages, none the less RTL languages such as Arabic or Hebrew. Thanks to the placeholders added in PrestaShop 1.5, such strings are now fully translatable in any language.

Some strings might have a warning icon to their right. This indicates strings with placeholders. You can click on the icon to get more information.\
In case of a string with a placeholder, you should make sure that the content of that placeholder will be placed in the correct flow of the sentence, and avoid literal translation.\
Numbered placeholders (`%1$s`, `%2$d`, etc.) enable translators to rearrange the order of the placeholders in the string while maintaining the information each is replaced with. This way, a French translator could choose to translate "Order #%1$d from %2$s" into "Commande n°%1$s du %2$s" or "Le %2$s, commande n°%1$s".

![](<../../../.gitbook/assets/23789739 (1).png>)

### Specific features <a href="#translations-specificfeatures" id="translations-specificfeatures"></a>

Most translation categories present their strings in the same way: the category's strings are grouped into fieldsets that you can close or expand by clicking on their title. The title indicates the number of expressions that the fieldset contains, and when needed, the number of missing expressions, in brackets and in red.

This is true for most categories, except three:

* **Error messages**. Strings are not group into many fieldset, they are all presented together.
* **PDF templates**. There is only one fieldset, "PDF".
* **E-mail templates**. Strings are split into fieldsets, but they are not simple text fields anymore. Each e-mail has two templates: a HTML one, which is styled and colored, and a text one, when is plain and simple. While the plain text one can be edited directly in the textfield, the HTML one can only be edited by clicking on the "Edit this e-mail template" button at the bottom of the preview. That click turns the preview into a WYSIWYG textfield (what you see is what you get), with a complete editor at the top (based on TinyMCE: [http://www.tinymce.com/](http://www.tinymce.com/)). In addition to editing the text, you can change the design as you see fit, for instance you can change the colors in order to adhere to your shop's design.\
  Note that the e-mail templates feature placeholders, such as `{lastname}` or `{shop_name}`, which PrestaShop replaces with the actual values when sending the e-mail. Make sure to keep them in both your translation.

![](<../../../.gitbook/assets/23789742 (2).png>)

## Add / Update a Language <a href="#translations-add-updatealanguage" id="translations-add-updatealanguage"></a>

PrestaShop translations are available in packs, which combine all the different translation categories into a zip file. Many language packs are available freely for you to download and install, directly from the PrestaShop.com servers. PrestaShop will take care of downloading the language pack, unpacking it and creating the correct sub-folder in your installation's `/translation` folder.

![](<../../../.gitbook/assets/23789747 (1).png>)

You can also update the currently installed languages, likewise directly from the PrestaShop.com servers, but be reminded that any change that you might have made to your own translations will be lost once you update it.

## Import a Language Pack Manually <a href="#translations-importalanguagepackmanually" id="translations-importalanguagepackmanually"></a>

In the case where you do not want to use an official PrestaShop translation pack, but rather a custom one (either provided by someone you know, or one that you exported from another PrestaShop installation), then this tool is for you.

![](<../../../.gitbook/assets/23789748 (1).png>)

Select the Zip file, select the theme to which you want that pack to be applied to, then click the "Import" button, and it will install the pack in the `/translation` folder.

If there is already a language folder with the same ISO 639-1 code, it will be replaced by the files from the pack you are importing.

## Export a Language <a href="#translations-exportalanguage" id="translations-exportalanguage"></a>

You can create your own language pack using this tool, either as a way of making a backup of your customizations, or in order to share your translations with other PrestaShop installation – your own or someone else's.

![](<../../../.gitbook/assets/23789749 (1).png>)

Simply choose the language and the theme of the translation you wish to export, and click the "Export" button.

Note that the pack will contain the theme that your translation is supposed to support.

## Copy <a href="#translations-copy" id="translations-copy"></a>

You can copy the content of one language to another. This is especially useful when you wish to replace a theme's language with the same language from another theme.

![](<../../../.gitbook/assets/23789750 (1).png>)

Choose the source language and theme, then the destination language and theme, then click the "Copy" button. In most case, the language should remain the same in both drop-down lists.

If there is already a language folder for this language in the destination theme, it will be replaced by the files from the language and theme you are copying.

You might prefer to first create a new language for the destination theme before copying the source language to it.
