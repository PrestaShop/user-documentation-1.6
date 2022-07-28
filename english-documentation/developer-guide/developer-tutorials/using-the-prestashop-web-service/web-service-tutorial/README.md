# Web service tutorial

This tutorial explores how to create a small application to perform these four basic operations for customers.

## Prerequisites <a href="#webservicetutorial-prerequisites" id="webservicetutorial-prerequisites"></a>

* PrestaShop 1.6 installed on a server with `mod_rewrite` enabled (Apache only).
* A local xAMP server with PHP5 enabled.

## About CRUD & REST <a href="#webservicetutorial-aboutcrud-and-rest" id="webservicetutorial-aboutcrud-and-rest"></a>

The PrestaShop web service uses the REST architecture in order to be available on as many platforms as possible, since the HTTP protocol and XML files are understood by most platforms, if not all.

[**CRUD**](http://en.wikipedia.org/wiki/Create,\_read,\_update\_and\_delete) is an acronym that stands for "Create, Read, Update, and Delete". These are the four basic operations for managing data in an application.

[**REST**](http://en.wikipedia.org/wiki/REST) defines roughly a style of software architecture, which promotes the use of HTTP methods when building web application, instead of custom methods or protocols such as SOAP or WSDL. It defines several rules, including one that is similar to CRUD, which is described below.

HTTP has several methods that can perform processing on data as defined in the REST architecture, among which are 4 main methods. See this page: [http://en.wikipedia.org/wiki/HTTP#Request\_methods](http://en.wikipedia.org/wiki/HTTP#Request\_methods)

The table below offers a comparison with CRUD and SQL:

| HTTP / REST | CRUD     | SQL    |
| ----------- | -------- | ------ |
| POST        | Create   | INSERT |
| GET         | Retrieve | SELECT |
| PUT         | Update   | UPDATE |
| DELETE      | Delete   | DELETE |

## Chapters in this tutorial <a href="#webservicetutorial-chaptersinthistutorial" id="webservicetutorial-chaptersinthistutorial"></a>

Chapters 1, 2 and 3 are mandatory, as they contain the fundamental knowledge for using the web service.\
The next chapters, explores ways to interact with the web service using each of the REST operations, in order to give you the tools to make a full CRUD application.\
If you only want to retrieve data, for example when developing a web application to notify you of orders, you might only be interested in Chapter 4.\
If you prefer to develop a more complete application, chapters 4 to 7 will interest you.\
Chapters 9 and 10 give you more detail on specific content management.

Finally, a cheat-sheet will give you quick hints and reminders.

Here are the chapters in this tutorial:

* [Chapter 1 - Creating an access to the back office](chapter-1-creating-an-access-to-the-back-office.md)
* [Chapter 2 - Discovery: Testing your access to the web service with the browser](chapter-2-discovery-testing-your-access-to-the-web-service-with-the-browser.md)
* [Chapter 3 - First steps: Accessing the web service and listing customers](chapter-3-first-steps-accessing-the-web-service-and-listing-customers.md)
* [Chapter 4 - Data retrieval: Retrieving a customer](chapter-4-data-retrieval-retrieving-a-customer.md)
* [Chapter 5 - Data modification: Updating a customer](chapter-5-data-modification-updating-a-customer.md)
* [Chapter 6 - Data creation: Creating a remote online form](chapter-6-data-creation-creating-a-remote-online-form.md)
* [Chapter 7 - Data removal: Removing customer accounts from the database](chapter-7-data-removal-removing-customer-accounts-from-the-database.md)
* [Chapter 8 - Advanced use](chapter-8-advanced-use.md)
* [Chapter 9 - Image management](chapter-9-image-management.md)
* [Chapter 10 - Price management](chapter-10-price-management.md)
* [Cheat-sheet - Concepts outlined in this tutorial](cheat-sheet-concepts-outlined-in-this-tutorial.md)
