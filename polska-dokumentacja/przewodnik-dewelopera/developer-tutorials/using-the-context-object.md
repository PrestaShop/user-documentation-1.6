# Using the Context Object -

**Table of contents**

/\*\<!\[CDATA\[\*/\
div.rbtoc1597140224437 {padding: 0px;}\
div.rbtoc1597140224437 ul {list-style: disc;margin-left: 0px;}\
div.rbtoc1597140224437 li {margin-left: 0px;padding-left: 0px;}\
\
/\*]]>\*/

* [Using the Context Object](using-the-context-object.md#UsingtheContextObject--UsingtheContextObject)
  * [What is the Context object?](using-the-context-object.md#UsingtheContextObject--WhatistheContextobject?)
  * [What is stored by the Context?](using-the-context-object.md#UsingtheContextObject--WhatisstoredbytheContext?)
  * [How to access the Context?](using-the-context-object.md#UsingtheContextObject--HowtoaccesstheContext?)
  * [How is the Context initialized?](using-the-context-object.md#UsingtheContextObject--HowistheContextinitialized?)
  * [How to use the Context?](using-the-context-object.md#UsingtheContextObject--HowtousetheContext?)
  * [More examples of Context use](using-the-context-object.md#UsingtheContextObject--MoreexamplesofContextuse)
  * [Using the Context in a PrestaShop 1.4 module](using-the-context-object.md#UsingtheContextObject--UsingtheContextinaPrestaShop1.4module)

## Using the Context Object <a href="#usingthecontextobject-usingthecontextobject" id="usingthecontextobject-usingthecontextobject"></a>

### What is the Context object? <a href="#usingthecontextobject-whatisthecontextobject" id="usingthecontextobject-whatisthecontextobject"></a>

The Context is a technical feature introduced with version 1.5 of PrestaShop. Its two goals are:

* preventing developers from using global variables.
* enabling them to change the context of some methods.

The Context is a registry for PHP variables that were previously accessed as globals. It aims to standardize the way these variables are accessed, and to make the code more robust by getting rid of global vars.\
It is a light implementation of the Registry design pattern: it is a class that stores the main PrestaShop information, such as the current cookie, the customer, the employee, the cart, Smarty, etc.

Before version 1.5, you had to rely on the cookie in order to access this data:**PrestaShop 1.4 code**

```
$cookie->id_lang;
```

Now that the Context is available, the same data can be accessed more cleanly:**PrestaShop 1.5 code**

```
$this->context->language->id;
```

### What is stored by the Context? <a href="#usingthecontextobject-whatisstoredbythecontext" id="usingthecontextobject-whatisstoredbythecontext"></a>

These objects are always accessible through the context:

* **Language**. Set with the customer or employee language.
* **Country**. Default country.
* **Currency**. Set with the customer currency or the shop's default currency.
* **Shop**. Current shop.
* **Cookie**. Cookie instance.
* **Link**. Link instance.
* **Smarty**. Smarty instance.

These objects are only accessible for the customer Context:

* **Customer**. Existing customer retrieved from the cookie or default customer.
* **Cart**. Current cart.
* **Controller**. Current controller instance.

These objects are only accessible for the administrator Context:

* **Employee**. Current employee.

### How to access the Context? <a href="#usingthecontextobject-howtoaccessthecontext" id="usingthecontextobject-howtoaccessthecontext"></a>

From inside a `Controller` subclass, an `AdminTab` subclass or a `Module` subclass, the Context should be called with this shortcut: `$this->context`.

From anywhere else, you can get the Context instance by calling `Context::getContext()`.

### How is the Context initialized? <a href="#usingthecontextobject-howisthecontextinitialized" id="usingthecontextobject-howisthecontextinitialized"></a>

The context is initialized with data coming from the cookie or from the database. For example, to create the `Language` object, the context looks for an `id_lang` value in the cookie. If it doesn't find one, it will retrieve the default language `id` from the database.

### How to use the Context? <a href="#usingthecontextobject-howtousethecontext" id="usingthecontextobject-howtousethecontext"></a>

Whenever you would have accessed the cookie to retrieve a variable, or used a global statement, you will probably want to access the Context instead.

A few common replacements:

*   Static shortcuts in `FrontController`subclasses are deprecated:**PrestaShop 1.4 code**

    ```
    $id_cart = self::cart->id;
    ```

    ...is to be replaced with...**PrestaShop 1.5 code**

    ```
    $id_cart = $this->context->cart->id;
    ```
*   Do not recreate an object that already exists:**PrestaShop 1.4 code**

    ```
    $language = new Language($cookie->id_lang);

    $iso_code = $language->iso_code;
    ```

    ...is to be replaced with...**PrestaShop 1.5 code**

    ```
    $iso_code = $this->context->language->iso_code;
    ```

### More examples of Context use <a href="#usingthecontextobject-moreexamplesofcontextuse" id="usingthecontextobject-moreexamplesofcontextuse"></a>

| Old way                                                                     | New way                                       |
| --------------------------------------------------------------------------- | --------------------------------------------- |
| $cookie->id\_lang;                                                          | $this->context->language->id;                 |
| if ($cookie->isLogged())                                                    | if ($this->context->customer->isLogged())     |
| if ($cookie->isLoggedBack())                                                | if ($this->context->employee->isLoggedBack(); |
| $cart->getProducts();                                                       | $this->context->cart->getProducts();          |
| <p>$language = new Language($cookie->id_lang);<br> $language->iso_code;</p> | $this->context->language->iso\_code;          |
| new Currency($cookie->id\_lang);                                            | $this->context->currency;                     |
| $defaultCountry->id\_zone;                                                  | $this->context->country->id\_zone;            |
| new Link();                                                                 | $this->context->link;                         |
| $smarty->assign(...);                                                       | $this->context->smarty->assign(...);          |

### Using the Context in a PrestaShop 1.4 module <a href="#usingthecontextobject-usingthecontextinaprestashop1.4module" id="usingthecontextobject-usingthecontextinaprestashop1.4module"></a>

Modules written for PrestaShop 1.5, and which therefore rely on the Context object, can be made to gracefully degrade its Context use in order to work in PrestaShop 1.4.

Add this method to the module's main class:

```
// Retrocompatibility 1.4/1.5+
private function initContext()
{
  if (class_exists('Context'))
    $this->context = Context::getContext();
  else
  {
    global $smarty, $cookie;
    $this->context = new StdClass();
    $this->context->smarty = $smarty;
    $this->context->cookie = $cookie;
  }
}

```

Then, add this line in the module's constructor method:

```
// Retrocompatibility
$this->initContext();
```

Additionally, when rewriting you v1.5+ module in work to work in v1.4, you should use the older hook names, such as `displayProductTab` or `displayProductTabContent`. These two example hooks are respectively registered using the `productTab` and `productTabContent` calls, which are compatible for both v1.4 and v1.5+, but will not work in the next major version.
