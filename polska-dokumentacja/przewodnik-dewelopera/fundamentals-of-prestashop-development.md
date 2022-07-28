# Fundamentals of PrestaShop Development -

/\*\<!\[CDATA\[\*/\
div.rbtoc1597140222038 {padding: 0px;}\
div.rbtoc1597140222038 ul {list-style: disc;margin-left: 0px;}\
div.rbtoc1597140222038 li {margin-left: 0px;padding-left: 0px;}\
\
/\*]]>\*/

* [Fundamentals of PrestaShop Development](fundamentals-of-prestashop-development.md#FundamentalsofPrestaShopDevelopment--FundamentalsofPrestaShopDevelopment)
  * [Concepts](fundamentals-of-prestashop-development.md#FundamentalsofPrestaShopDevelopment--Concepts)
  * [PrestaShop's technical architecture](fundamentals-of-prestashop-development.md#FundamentalsofPrestaShopDevelopment--PrestaShop%27stechnicalarchitecture)
  * [Database schema](fundamentals-of-prestashop-development.md#FundamentalsofPrestaShopDevelopment--Databaseschema)

## Fundamentals of PrestaShop Development <a href="#fundamentalsofprestashopdevelopment-fundamentalsofprestashopdevelopment" id="fundamentalsofprestashopdevelopment-fundamentalsofprestashopdevelopment"></a>

PrestaShop was conceived so that third-party modules could easily build upon its foundations, making it an extremely customizable e-commerce software.

PrestaShop's customization is based on three possibilities:

* Themes,
* Modules,
* Overriding.

Themes are explored in full in the Design Guide: [http://doc.prestashop.com/display/PS16/Designer+Guide](http://doc.prestashop.com/display/PS16/Designer+Guide).\
Modules and the override system are explored in this Developer Guide, starting with the "Concepts" section below. You can learn more about each in the following chapters:

* [http://doc.prestashop.com/display/PS16/Creating+a+PrestaShop+module](http://doc.prestashop.com/display/PS16/Creating+a+PrestaShop+module)
* [http://doc.prestashop.com/display/PS16/Overriding+default+behaviors](http://doc.prestashop.com/display/PS16/Overriding+default+behaviors)

By default, PrestaShop is provided with more than 100 modules, enabling you to launch your online business quickly and for free.

More than 2300 modules are also available at the official [add-ons site](http://addons.prestashop.com/).\
&#x20;These additional modules were built by the PrestaShop company or members of the PrestaShop community, and are sold at affordable prices.\
&#x20;As a developer, you can also share your modules on this site, and receive 70% of the amounts associated with the sale of your creations. [Sign up now](http://addons.prestashop.com/en/authentication.php#createnow)!

### Concepts <a href="#fundamentalsofprestashopdevelopment-concepts" id="fundamentalsofprestashopdevelopment-concepts"></a>

You should be familiar with PHP and Object-Oriented Programming before attempting to write your own module.

You can learn PHP here:

* [http://www.php.net/manual/en/getting-started.php](http://www.php.net/manual/en/getting-started.php)
* [http://www.codecademy.com/tracks/php](http://www.codecademy.com/tracks/php)

You can learn Object-Oriented programming here:

* [http://en.wikipedia.org/wiki/Object-oriented\_programming](http://en.wikipedia.org/wiki/Object-oriented\_programming)
* [http://net.tutsplus.com/tutorials/php/object-oriented-php-for-beginners/](http://net.tutsplus.com/tutorials/php/object-oriented-php-for-beginners/)

A module is an extension to PrestaShop that enables any developer to add the following:

* Provide additional functionality to PrestaShop.
* View additional items on the site (product selection, etc.).
* Communicate with other e-commerce services (buying guides, payment platforms, logistics, etc.).
* etc.

Overriding is a system in itself. PrestaShop uses completely object-oriented code. One of the advantages of this is that, with the right code architecture, you can easily replace or extend parts of the core code with your own custom code, without having to touch the core code. Your code thus overrides the core code, making PrestaShop behave as you prefer it to.\
It is not recommended to use an override in a module that you intend to distribute (for instance through the PrestaShop Addons marketplace), and they are forbidden in partner modules. Keep them for your own shop.

### PrestaShop's technical architecture <a href="#fundamentalsofprestashopdevelopment-prestashopstechnicalarchitecture" id="fundamentalsofprestashopdevelopment-prestashopstechnicalarchitecture"></a>

PrestaShop is based on a [3-tier architecture](http://en.wikipedia.org/wiki/Multitier\_architecture#Three-tier\_architecture):

* **Object/data**. Database access is controlled through files in the "classes" folder.
* **Data control**. User-provided content is controlled by files in the root folder.
* **Design**. All of the theme's files are in the "themes" folder.

![](<../../.gitbook/assets/13697026 (1).png>)

This is the same principle as the Model–View–Controller (MVC) architecture, only in a simpler and more accessible way.

Our developer team chose not to use a PHP framework, such as Zend Framework, Symfony or CakePHP, so as to allow for better readability, and thus faster editing.\
This also makes for better performances, since the software is only made of the lines of code it requires, and does not contain a bunch of supplemental generic libraries.

A 3-tier architecture has many advantages:

* It's easier to read the software's code.
* Developers can add and edit code faster.
* Graphic designer and HTML integrators can work with the confines of the `/themes` folder without having to understand or even read a single line of PHP code.
* Developers can work on additional data and modules that the HTML integrators can make use of.

#### Model <a href="#fundamentalsofprestashopdevelopment-model" id="fundamentalsofprestashopdevelopment-model"></a>

A model represents the application's behavior: data processing, database interaction, etc.

It describes or contains the data that have been processed by the application. It manages this data and guarantees its integrity.

#### View <a href="#fundamentalsofprestashopdevelopment-view" id="fundamentalsofprestashopdevelopment-view"></a>

A view is the interface with which the user interacts.

Its first role is to display the data that is been provided by the model. Its second role is to handle all the actions from the user (mouse click, element selection, buttons, etc.), and send these events to the controller.

The view does not do any processing; it only displays the result of the processing performed by the model, and interacts with the user.

#### Controller <a href="#fundamentalsofprestashopdevelopment-controller" id="fundamentalsofprestashopdevelopment-controller"></a>

The Controller manages synchronization events between the Model and the View, and updates both as needed. It receives all the user events and triggers the actions to perform.

If an action needs data to be changed, the Controller will "ask" the Model to change the data, and in turn the Model will notify the View that the data has been changed, so that the View can update itself.

### Database schema <a href="#fundamentalsofprestashopdevelopment-databaseschema" id="fundamentalsofprestashopdevelopment-databaseschema"></a>

![](<../../.gitbook/assets/27623429 (1).png>)

You can download the PrestaShop 1.6 SQL schema [in PDF form (3.90 Mb)](http://doc.prestashop.com/download/attachments/21463263/mpd16.pdf?version=1\&modificationDate=1411054893000\&api=v2), or [in the original MySQL Workbench file format](http://doc.prestashop.com/download/attachments/21463263/mpd16.mwb?version=1\&modificationDate=1411054954000\&api=v2) (you will need [MySQL Workbench](http://wb.mysql.com/) to view it).
