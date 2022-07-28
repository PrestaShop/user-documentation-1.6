# How to write a commit message

When you contribute code to the PrestaShop project ([through Github](https://github.com/PrestaShop/PrestaShop/)), we ask that you strictly use the PrestaShop way of writing a commit name. This way, when building the code history, your commit message will fit nicely with the ones from others contributors and from the PrestaShop developers.

The conventions were changed [on May 5th, 2016](http://build.prestashop.com/news/prestashop-coding-standards/), and are now much simpler.

* How to write a commit message
  * [Commit naming convention](how-to-write-a-commit-message.md#Howtowriteacommitmessage-Commitnamingconvention)
    * [Category](how-to-write-a-commit-message.md#Howtowriteacommitmessage-Category)
    * [Short description](how-to-write-a-commit-message.md#Howtowriteacommitmessage-Shortdescription)
  * [Description of the commit / pull request](how-to-write-a-commit-message.md#Howtowriteacommitmessage-Descriptionofthecommit/pullrequest)
  * [Sample commit message](how-to-write-a-commit-message.md#Howtowriteacommitmessage-Samplecommitmessage)
  * [Adding the correct license to new files](how-to-write-a-commit-message.md#Howtowriteacommitmessage-Addingthecorrectlicensetonewfiles)

## Commit naming convention <a href="#howtowriteacommitmessage-commitnamingconvention" id="howtowriteacommitmessage-commitnamingconvention"></a>

The commit's name must be in English, and should be formatted like this:

```
category: short description
```

The title of the pull request should simply describe its content (whether it contains one or several commits), in the clearest way possible. The title should reflect the overall change of the pull request.

### Category <a href="#howtowriteacommitmessage-category" id="howtowriteacommitmessage-category"></a>

The category is the portion of the project to which your changes apply to.

| Category | Meaning                                                                                  |
| -------- | ---------------------------------------------------------------------------------------- |
| FO       | Front office (theme, front controller, images, CSS, JavaScript, module's FO, PDF, etc.). |
| BO       | Back office (theme, admin controller, images, CSS, JavaScript, module's BO, etc.).       |
| CO       | The core of the software itself: classes, controllers, etc.                              |
| IN       | All the files in the `/install` folder.                                                  |
| WS       | Web Service.                                                                             |
| LO       | Localization pack.                                                                       |
| TE       | Unit tests or functional test.                                                           |

### Short description <a href="#howtowriteacommitmessage-shortdescription" id="howtowriteacommitmessage-shortdescription"></a>

Use the description to explain what your commit does in a few words. Try to be concise!

If you fixed a ticket from the Forge, please add a link to that ticket in the first comment and specify the bug's Forge number in the description (eg: #PSCFV-007).

## Description of the commit / pull request <a href="#howtowriteacommitmessage-descriptionofthecommit-pullrequest" id="howtowriteacommitmessage-descriptionofthecommit-pullrequest"></a>

You can put more details in the commit description.

If your code change requires a lot of explanation, please [open a Forge ticket](http://forge.prestashop.com/) explaining your intent with this code change, so that the Product team can discuss it with you. Once the ticket is created, link to it from the PR's comment, and give a link to the PR from the ticket, in order to bridge the two.

## Sample commit message <a href="#howtowriteacommitmessage-samplecommitmessage" id="howtowriteacommitmessage-samplecommitmessage"></a>

Here are a few sample messages:

```
BO: Fixed bug while updating images in AdminProduct
FO: You can now buy products without TVA
MO: New RSS Feed module
```

## Adding the correct license to new files <a href="#howtowriteacommitmessage-addingthecorrectlicensetonewfiles" id="howtowriteacommitmessage-addingthecorrectlicensetonewfiles"></a>

By submitting your code to the PrestaShop project, you are releasing it under a Open Source license: either OSL or AFL.

If you add new files, they need to have the "NOTICE OF LICENSE" and the "DISCLAIMER" sections at the start of the file.

* For general PrestaShop files: the notice should mention the [OSL 3.0 license](http://opensource.org/licenses/OSL-3.0).
* For module files: the notice should mention the [AFL 3.0 license](http://opensource.org/licenses/AFL-3.0).

You can copy/paste from existing files in the project.

You can also use this for general files:

```
<?php
/**
* 2007-2017 PrestaShop
*
* NOTICE OF LICENSE
*
* This source file is subject to the Open Software License (OSL 3.0)
* that is bundled with this package in the file LICENSE.txt.
* It is also available through the world-wide-web at this URL:
* http://opensource.org/licenses/osl-3.0.php
* If you did not receive a copy of the license and are unable to
* obtain it through the world-wide-web, please send an email
* to license@prestashop.com so we can send you a copy immediately.
*
* DISCLAIMER
*
* Do not edit or add to this file if you wish to upgrade PrestaShop to newer
* versions in the future. If you wish to customize PrestaShop for your
* needs please refer to http://www.prestashop.com for more information.
*
*  @author PrestaShop SA <contact@prestashop.com>
*  @copyright  2007-2016 PrestaShop SA
*  @version  Release: $Revision: 6844 $
*  @license    http://opensource.org/licenses/osl-3.0.php  Open Software License (OSL 3.0)
*  International Registered Trademark & Property of PrestaShop SA
*/
```

...or for modules...

```
/**
* 2007-2017 PrestaShop
*
* NOTICE OF LICENSE
*
* This source file is subject to the Academic Free License (AFL 3.0)
* that is bundled with this package in the file LICENSE.txt.
* It is also available through the world-wide-web at this URL:
* http://opensource.org/licenses/afl-3.0.php
* If you did not receive a copy of the license and are unable to
* obtain it through the world-wide-web, please send an email
* to license@prestashop.com so we can send you a copy immediately.
*
* DISCLAIMER
*
* Do not edit or add to this file if you wish to upgrade PrestaShop to newer
* versions in the future. If you wish to customize PrestaShop for your
* needs please refer to http://www.prestashop.com for more information.
*
*  @author PrestaShop SA <contact@prestashop.com>
*  @copyright  2007-2016 PrestaShop SA
*  @license    http://opensource.org/licenses/afl-3.0.php  Academic Free License (AFL 3.0)
*  International Registered Trademark & Property of PrestaShop SA
*/
```
