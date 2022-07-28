# Web service reference

**Table of contents**

* [Web service reference](web-service-reference.md#Webservicereference-Webservicereference)
  * [Using the API](web-service-reference.md#Webservicereference-UsingtheAPI)
    * [Available HTTP methods](web-service-reference.md#Webservicereference-AvailableHTTPmethods)
    * [Available resources](web-service-reference.md#Webservicereference-Availableresources)
  * [Value formats](web-service-reference.md#Webservicereference-Valueformats)
    * [Generic value types](web-service-reference.md#Webservicereference-Genericvaluetypes)
    * [Specific value types](web-service-reference.md#Webservicereference-Specificvaluetypes)
    * [Names](web-service-reference.md#Webservicereference-Names)
    * [Locations](web-service-reference.md#Webservicereference-Locations)
    * [Products](web-service-reference.md#Webservicereference-Products)

## Web service reference <a href="#webservicereference-webservicereference" id="webservicereference-webservicereference"></a>

### Using the API <a href="#webservicereference-usingtheapi" id="webservicereference-usingtheapi"></a>

All methods are to be called through the `/api/` gateway. For instance, [`http://www.mystore.com/api/carriers`](http://www.mystore.com/api/carriers)

#### Available HTTP methods <a href="#webservicereference-availablehttpmethods" id="webservicereference-availablehttpmethods"></a>

Most methods can be accessed in a REST manner, with the 5 main HTTP request methods: GET, POST, PUT, DELETE, HEAD.\
&#x20;The only exceptions are:

* `search`: only GET and HEAD.
* `stock_availables`: only GET, POST, and HEAD.
* `stock_movements`: only GET and HEAD.
* `stocks`: only GET and HEAD.
* `supply_order_details`: only GET and HEAD.
* `supply_order_histories`: only GET and HEAD.
* `supply_order_receipt_histories`: only GET and HEAD.
* `supply_order_states`: only GET and HEAD.
* `supply_orders`: only GET and HEAD.
* `warehouse_product_locations`: only GET and HEAD.
* `warehouses`: only GET, POST, PUT, and HEAD.

All methods have two optional types, which are simply to be added at the end of the URL:

* `?blank`: returns a blank XML tree of the chosen object.
* `?synopsis`: returns a blank XML tree of the chosen object, with the format that is expected for each value (see below) and specific indicators (ie, if the node is required, and its maximum size in number of characters).

#### Available resources <a href="#webservicereference-availableresources" id="webservicereference-availableresources"></a>

This list is current as of v1.5.4.1 of PrestaShop.

| Method                            | Description                                       |
| --------------------------------- | ------------------------------------------------- |
| addresses                         | The Customer, Manufacturer and Customer addresses |
| carriers                          | The Carriers                                      |
| cart\_rules                       | Cart rules management                             |
| carts                             | Customer's carts                                  |
| categories                        | The product categories                            |
| combinations                      | The product combination                           |
| configurations                    | Shop configuration                                |
| contacts                          | Shop contacts                                     |
| content\_management\_system       | Content management system                         |
| countries                         | The countries                                     |
| currencies                        | The currencies                                    |
| customer\_messages                | Customer services messages                        |
| customer\_threads                 | Customer services threads                         |
| customers                         | The e-shop's customers                            |
| deliveries                        | Product delivery                                  |
| employees                         | The Employees                                     |
| groups                            | The customer's groups                             |
| guests                            | The guests                                        |
| image\_types                      | The image types                                   |
| images                            | The images                                        |
| images/general/header             | The shop's logo in the header                     |
| images/general/mail               | The shop's logo in the e-mails                    |
| images/general/invoice            | The shop's logo in the invoice                    |
| images/general/store\_icon        | The shop's logo as a favicon                      |
| images/products                   | The products images.                              |
| images/categories                 | The categories images                             |
| images/manufacturers              | The manufacturers images.                         |
| images/suppliers                  | The suppliers images.                             |
| images/stores                     | The stores images.                                |
| languages                         | Shop languages                                    |
| manufacturers                     | The product manufacturers                         |
| order\_carriers                   | Details of an order                               |
| order\_details                    | Details of an order                               |
| order\_discounts                  | Discounts of an order                             |
| order\_histories                  | The Order histories                               |
| order\_invoices                   | The Order invoices                                |
| order\_payments                   | The Order payments                                |
| order\_states                     | The Order states                                  |
| orders                            | The Customers orders                              |
| price\_ranges                     | Price range                                       |
| product\_feature\_values          | The product feature values                        |
| product\_features                 | The product features                              |
| product\_option\_values           | The product options value                         |
| product\_options                  | The product options                               |
| product\_suppliers                | Product Suppliers                                 |
| products                          | The products                                      |
| search                            | Search                                            |
| shop\_groups                      | Shop groups from multi-shop feature               |
| shops                             | Shops from multi-shop feature                     |
| specific\_price\_rules            | Specific price management                         |
| specific\_prices                  | Specific price management                         |
| states                            | The available states of countries                 |
| stock\_availables                 | Available quantities                              |
| stock\_movement\_reasons          | The stock movement reason                         |
| stock\_movements                  | Stock movements management                        |
| stocks                            | Stocks                                            |
| stores                            | The stores                                        |
| suppliers                         | The product suppliers                             |
| supply\_order\_details            | Supply Order Details                              |
| supply\_order\_histories          | Supply Order Histories                            |
| supply\_order\_receipt\_histories | Supply Order Receipt Histories                    |
| supply\_order\_states             | Supply Order States                               |
| supply\_orders                    | Supply Orders                                     |
| tags                              | The Products tags                                 |
| tax\_rule\_groups                 | Tax rule groups                                   |
| tax\_rules                        | Tax rules entity                                  |
| taxes                             | The tax rate                                      |
| translated\_configurations        | Shop configuration                                |
| warehouse\_product\_locations     | Location of products in warehouses                |
| warehouses                        | Warehouses                                        |
| weight\_ranges                    | Weight ranges                                     |
| zones                             | The Countries zones                               |

### Value formats <a href="#webservicereference-valueformats" id="webservicereference-valueformats"></a>

When displaying a data schema in synopsis mode, the API gives some useful indication of the expected data type.

For instance:

```
<?xml version="1.0" encoding="UTF-8"?>
<prestashop xmlns:xlink="http://www.w3.org/1999/xlink">
  <customer>
    <id_default_group></id_default_group>
    <id_lang format="isUnsignedId"></id_lang>
    <newsletter_date_add></newsletter_date_add>
    <ip_registration_newsletter></ip_registration_newsletter>
    <last_passwd_gen></last_passwd_gen>
    <secure_key format="isMd5"></secure_key>
    <deleted format="isBool"></deleted>
    <passwd required="true" maxSize="32" format="isPasswd"></passwd>
    <lastname required="true" maxSize="32" format="isName"></lastname>
    <firstname required="true" maxSize="32" format="isName"></firstname>
    <email required="true" maxSize="128" format="isEmail"></email>
    ...
  </customer>
</prestashop>
```

Here are the descriptions of the expected value types.

#### Generic value types <a href="#webservicereference-genericvaluetypes" id="webservicereference-genericvaluetypes"></a>

| Format             | Description                                                                 | Expected value, in regexp form |
| ------------------ | --------------------------------------------------------------------------- | ------------------------------ |
| isBool             | A boolean value (true or false).                                            | n/a                            |
| isFloat            | A floating-point value (between -3.4 × 10^38 and +3.4 × 10^38).             | n/a                            |
| isInt              | An integral value (between -2,147,483,648 and 2,147,483,647).               | n/a                            |
| isNullOrUnsignedId | An integral and unsigned value (between 0 and 4294967296), or a NULL value. | n/a                            |
| isSerializedArray  | PHP serialized data.                                                        |                                |
| isString           | A string of characters.                                                     | n/a                            |
| isUnsignedId       | An integral and unsigned value (between 0 and 4294967296).                  | n/a                            |

#### Specific value types <a href="#webservicereference-specificvaluetypes" id="webservicereference-specificvaluetypes"></a>

| Format               | Description                                                                                          | Expected value, in regexp form |
| -------------------- | ---------------------------------------------------------------------------------------------------- | ------------------------------ |
| isBirthDate          | A valid date, in YYYY-MM-DD format.                                                                  |                                |
| isCleanHtml          | Must not contain invalid HTML tags, nor XSS.                                                         |                                |
| isColor              | A valid HTML/CSS color, in #xxxxxx format or text format.                                            |                                |
| isEmail              | A valid e-mail address.                                                                              |                                |
| isImageSize          | A valid image size, between 0 and 9999.                                                              |                                |
| isLanguageCode       | A valid language code, in XX or XX-XX format.                                                        |                                |
| isLanguageIsoCode    | A valid ISO language code, in XX or XXX format.                                                      |                                |
| isLinkRewrite        | A valid link rewrite.                                                                                |                                |
| isMd5                | A valid MD5 string: 32 characters, mixing lowercase, uppercase and numerals.                         |                                |
| isNumericIsoCode     | A valid ISO code, in 00 or 000 format.                                                               |                                |
| isPasswd             | A valid password, in. between 5 and 32 characters long.                                              |                                |
| isPasswdAdmin        | A valid password, between 8 and 32 characters long.                                                  |                                |
| isPhpDateFormat      | A valid PHP date – in fact, a string without '`<`' nor `'>`'.                                        |                                |
| isPriceDisplayMethod | A valid price display method, meaning the value be equals to constants `PS_TAX_EXC` or `PS_TAX_INC`. | n/a                            |
| isReference          | A valid product reference.                                                                           |                                |
| isUrl                | A valid URL.                                                                                         |                                |

#### Names <a href="#webservicereference-names" id="webservicereference-names"></a>

| Format          | Description                       | Expected value, in regexp form |
| --------------- | --------------------------------- | ------------------------------ |
| isCatalogName   | A valid product or category name. |                                |
| isCarrierName   | A valid carrier name.             |                                |
| isConfigName    | A valid configuration key.        |                                |
| isGenericName   | A valid standard name.            |                                |
| isImageTypeName | A valid image type.               |                                |
| isName          | A valid name.                     |                                |
| isTplName       | A valid template name.            |                                |

#### Locations <a href="#webservicereference-locations" id="webservicereference-locations"></a>

| Format          | Description                                                 | Expected value, in regexp form |
| --------------- | ----------------------------------------------------------- | ------------------------------ |
| isAddress       | A valid postal address.                                     |                                |
| isCityName      | A valid city name.                                          |                                |
| isCoordinate    | A valid latitude-longitude coordinates, in 00000.0000 form. |                                |
| isMessage       | A valid message.                                            |                                |
| isPhoneNumber   | A valid phone number.                                       |                                |
| isPostCode      | A valid postal code.                                        |                                |
| isStateIsoCode  | A valid state ISO code.                                     |                                |
| isZipCodeFormat | A valid zipcode format.                                     |                                |

#### Products <a href="#webservicereference-products" id="webservicereference-products"></a>

| Format        | Description                                                                            | Expected value, in regexp form |
| ------------- | -------------------------------------------------------------------------------------- | ------------------------------ |
| isAbsoluteUrl | A valid absolute URL.                                                                  |                                |
| isDniLite     | A valid DNI (_Documento Nacional de Identidad_) identifier. Specific to Spanish shops. |                                |
| isEan13       | A valid barcode (EAN13).                                                               |                                |
| isLinkRewrite | A valid friendly URL.                                                                  |                                |
| isPrice       | A valid price display method (either `PS_TAX_EXC` or `PS_TAX_INC`).                    | n/a                            |
| isUpc         | A valid barcode (UPC).                                                                 |                                |
