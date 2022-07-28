# Using the PrestaShop Web Service

**Table of content**

* [Using the PrestaShop Web Service](./#UsingthePrestaShopWebService-UsingthePrestaShopWebService)
  * [Learning how to use the web service](./#UsingthePrestaShopWebService-Learninghowtousethewebservice)
  * [Implementations](./#UsingthePrestaShopWebService-Implementations)
  * [Files](./#UsingthePrestaShopWebService-Files)

## Using the PrestaShop Web Service <a href="#usingtheprestashopwebservice-usingtheprestashopwebservice" id="usingtheprestashopwebservice-usingtheprestashopwebservice"></a>

PrestaShop enables merchants to give third-party tools access to their shop's database through a CRUD API, otherwise called a web service.

### Learning how to use the web service <a href="#usingtheprestashopwebservice-learninghowtousethewebservice" id="usingtheprestashopwebservice-learninghowtousethewebservice"></a>

#### Documentation <a href="#usingtheprestashopwebservice-documentation" id="usingtheprestashopwebservice-documentation"></a>

The quickest way to learn the intricacies of the PrestaShop web service is to use the [web service one-page documentation](web-service-one-page-documentation.md).

#### Tutorial <a href="#usingtheprestashopwebservice-tutorial" id="usingtheprestashopwebservice-tutorial"></a>

The slowest but most complete way to learn about the web service is to [follow the tutorial](web-service-tutorial/).

It demonstrates how to use the PrestaShop web service by creating a CRUD application using the dedicated PHP library.

### Implementations <a href="#usingtheprestashopwebservice-implementations" id="usingtheprestashopwebservice-implementations"></a>

* Manage your PrestaShop website through Open ERP: [Prestashop OpenERP Connector](https://launchpad.net/prestashoperpconnect/) by Akretion & CampToCamp (GNU Affero GPLv3)
* A Scala library to access the PrestaShop web service: [prestasac](https://github.com/orderly/prestashop-scala-client) by Alex Dean (GNU Affero GPLv3)
* A Python library to access the PrestaShop web service: [prestapyt](https://github.com/guewen/prestapyt) by Guewen Baconnier (GNU Affero GPLv3)

### Files <a href="#usingtheprestashopwebservice-files" id="usingtheprestashopwebservice-files"></a>

#### Web service library <a href="#usingtheprestashopwebservice-webservicelibrary" id="usingtheprestashopwebservice-webservicelibrary"></a>

The latest version of the **PSWebServiceLibrary.php** file can be found on our code repository: [https://github.com/PrestaShop/PrestaShop-webservice-lib/blob/master/PSWebServiceLibrary.php](https://github.com/PrestaShop/PrestaShop-webservice-lib/blob/master/PSWebServiceLibrary.php)\
To download the file:

1. Click here to view the raw file: [https://raw.github.com/PrestaShop/PrestaShop-webservice-lib/master/PSWebServiceLibrary.php](https://raw.github.com/PrestaShop/PrestaShop-webservice-lib/master/PSWebServiceLibrary.php)
2. Copy/paste the file into an empty text local file, using for instance Notepad.
3. Save the file as `PSWebServiceLibrary.php`

You can also directly download a zip archive of all the files in this repository, including the example files, by clicking here: [https://github.com/PrestaShop/PrestaShop-webservice-lib/archive/master.zip](https://github.com/PrestaShop/PrestaShop-webservice-lib/archive/master.zip)

#### Examples files <a href="#usingtheprestashopwebservice-examplesfiles" id="usingtheprestashopwebservice-examplesfiles"></a>

All the example files can be found on our code repository: [https://github.com/PrestaShop/PrestaShop-webservice-lib/tree/master/examples](https://github.com/PrestaShop/PrestaShop-webservice-lib/tree/master/examples)
