# Chapter 8 - Advanced use

**Table of content**

* [Chapter 8 - Advanced use](chapter-8-advanced-use.md#Chapter8-Advanceduse-Chapter8-Advanceduse)
  * [Rendering Options](chapter-8-advanced-use.md#Chapter8-Advanceduse-RenderingOptions)
    * [Include all fields from the "products" resource](chapter-8-advanced-use.md#include-all-fields-from-the-products-resource)
    * [Include only the ID of all carriers](chapter-8-advanced-use.md#Chapter8-Advanceduse-IncludeonlytheIDofallcarriers)
    * [Only include the "name" and "value" fields from the "configurations" resource](chapter-8-advanced-use.md#only-include-the-name-and-value-fields-from-the-configurations-resource)
  * [Rendering Filters](chapter-8-advanced-use.md#rendering-filters)
    * [Only include the first and last names of customers "customers" whose ids are 1 or 5](chapter-8-advanced-use.md#only-include-the-first-and-last-names-of-customers-customers-whose-ids-are-1-or-5)
    * [Only include the last names of customers "customers" whose ids are between 1 and 10](chapter-8-advanced-use.md#only-include-the-last-names-of-customers-customers-whose-ids-are-between-1-and-10)
    * [Only include the birthday of clients whose name is "John" and whose last name is "Doe"](chapter-8-advanced-use.md#only-include-the-birthday-of-clients-whose-name-is-john-and-whose-last-name-is-doe)
    * [Only include the names of manufacturers "manufacturers" whose name begins with "Appl"](chapter-8-advanced-use.md#only-include-the-names-of-manufacturers-manufacturers-whose-name-begins-with-appl)
  * [Sorting Filters](chapter-8-advanced-use.md#sorting-filters)
    * [Filter the customers "customers" in alphabetical order according to last name](chapter-8-advanced-use.md#filter-the-customers-customers-in-alphabetical-order-according-to-last-name)
  * [Filters to limit rendering](chapter-8-advanced-use.md#filters-to-limit-rendering)
    * [Only include the first 5 states "states"](chapter-8-advanced-use.md#only-include-the-first-5-states-states)
    * [Only include the first 5 elements starting from the 10th element from the states resource "states"](chapter-8-advanced-use.md#only-include-the-first-5-elements-starting-from-the-10th-element-from-the-states-resource-states)

## Chapter 8 - Advanced use <a href="#chapter8-advanceduse-chapter8-advanceduse" id="chapter8-advanceduse-chapter8-advanceduse"></a>

Here are a few sample advanced uses.\


### Rendering Options <a href="#chapter8-advanceduse-renderingoptions" id="chapter8-advanceduse-renderingoptions"></a>

#### Include all fields from the "products" resource

URL: (Store URL)/api/products/?display=full

PHP:

```
$opt = array(
	'resource' => 'products', 
	'display'  => 'full'
);
```

#### Include only the ID of all carriers <a href="#chapter8-advanceduse-includeonlytheidofallcarriers" id="chapter8-advanceduse-includeonlytheidofallcarriers"></a>

URL: (Store URL)/api/carriers/?display=\[id]

PHP :

```
$opt = array('resource' => 'carriers', 'display' => '[id]');
```

#### Only include the "name" and "value" fields from the "configurations" resource

URL: (Store URL)/api/configurations/?display=\[name,value]

PHP:

```
$opt = array(
	'resource' => 'configurations', 
	'display'  => '[name,value]'
);
```

### Rendering Filters

#### Only include the first and last names of customers "customers" whose ids are 1 or 5

URL: (Store URL)/api/customers/?display=\[firstname,lastname]\&filter\[id]=\[1|5]

PHP:

```
$opt = array(
	'resource'   => 'customers', 
	'display'    => '[firstname,lastname]', 
	'filter[id]' => '[1|5]'
);
```

#### Only include the last names of customers "customers" whose ids are between 1 and 10

URL: (Store URL)/api/customers/?display=\[lastname]\&filter\[id]=\[1,10]

PHP:

```
$opt = array(
	'resource'   =>'customers', 
	'display'    => '[lastname]', 
	'filter[id]' => '[1,10]'
);
```

#### Only include the birthday of clients whose name is "John" and whose last name is "Doe"

URL: (Store URL)/api/customers/?display=\[birthday]\&filter\[firstname]=\[John]\&filter\[lastname]=\[DOE]

PHP:

```
$opt = array(
	'resource'          =>'customers', 
	'display'           => '[birthday]', 
	'filter[firstname]' => '[John]', 
	'filter[lastname]'  => '[DOE]'
);
```

#### Only include the names of manufacturers "manufacturers" whose name begins with "Appl"

URL: (Store URL)/api/manufacturers/?display=\[name]\&filter\[name]=\[appl]%

PHP:

```
$opt = array(
	'resource'     => 'manufacturers', 
	'display'      => '[name]', 
	'filter[name]' => '[appl]%'
);
```

### Sorting Filters

#### Filter the customers "customers" in alphabetical order according to last name

URL: Store URL/api/customers?display=full\&sort=\[lastname\_ASC]

PHP:

```
$opt = array(
	'resource' => 'customers', 
	'display'  => 'full', 
	'sort'     => '[lastname_ASC]'
);
```

### Filters to limit rendering

#### Only include the first 5 states "states"

URL: (Store URL)/api/states/?display=full\&limit=5

PHP:

```
$opt = array(
	'resource' => 'states', 
	'display'  => 'full', 
	'limit'    => '5'
);
```

#### Only include the first 5 elements starting from the 10th element from the states resource "states"

URL: (Store URL)/api/states/?display=full\&limit=9,5

PHP:

```
$opt = array(
	'resource' => 'states', 
	'display'  => 'full', 
	'limit'    => '9,5'
);
```
