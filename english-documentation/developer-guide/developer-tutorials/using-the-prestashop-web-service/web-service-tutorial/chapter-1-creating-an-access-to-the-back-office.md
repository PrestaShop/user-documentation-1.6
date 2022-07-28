# Chapter 1 - Creating an access to the back office

Before you can do anything, you first need to create an access to the web service.

## Enabling the web service <a href="#chapter1-creatinganaccesstothebackoffice-enablingthewebservice" id="chapter1-creatinganaccesstothebackoffice-enablingthewebservice"></a>

Go in the PrestaShop back office, open the "Web service" page under the "Advanced Parameters" menu, and then choose "Yes" for the "Enable PrestaShop Webservice" option.

In previous versions of PrestaShop, you had to create a `.htaccess` file (or edit the existing one) in order to make your web service work.

This is no longer the case in PrestaShop 1.5+: the `.htaccess` will automatically be generated, while keeping your custom rules.

## Creating your access <a href="#chapter1-creatinganaccesstothebackoffice-creatingyouraccess" id="chapter1-creatinganaccesstothebackoffice-creatingyouraccess"></a>

Open the "Web service" page under the "Advanced Parameters", and then click the "Add New" button to access the account configuration section. A long form appears:

* **Key**. Click the "Generate" button to generate an authentication key. You can also create your own (which must be 32 characters long), but using a generated key prevents wrong-doers from guessing your key.\
  &#x20;Using this key, you and other selected users will be able to access the web service.
* **Key description**. The description is not public, but make sure to put all the keywords pertaining to its use, so that you can find they key more quickly. For instance, a reminder of who that key is for, and what it gives access to.
* **Status**. You can disable any key at any time. This enables you to only temporarily grant access to your data from a certain key.T
* **Permissions**. This section is very important, as it enables you to assign rights for each resource you want to make available for this key. Indeed, you might want a user to have read and write access on some resources, but only read access on others – and no access to the more important ones.\
  &#x20;In the list of permissions, the left button allows you to define all the rights for a given resource. Select the resources you need to manipulate from your application; in our case check the first check box in the "customers" row and then press "Save".
* **Shop association**. This only appears in multistore mode: you can choose the shop to which the key has access.

If you define your own passkey, make sure it is very secure and that its rights are limited.
