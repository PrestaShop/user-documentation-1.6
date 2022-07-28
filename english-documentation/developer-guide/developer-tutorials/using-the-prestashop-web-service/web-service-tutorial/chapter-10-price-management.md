# Chapter 10 - Price management

## Description <a href="#chapter10-pricemanagement-description" id="chapter10-pricemanagement-description"></a>

It is possible to retrieve the customer prices for a given product, simply by passing parameters to a web service query.

These custom prices are available for the following entities:

* products
* combinations

Custom prices have an alias that you must indicate.

## Example <a href="#chapter10-pricemanagement-example" id="chapter10-pricemanagement-example"></a>

Let's say we want to retrieve the price for combination '25' of the product '1', with tax, in a web service field name "my\_price".

The query: `/api/products/1?price[my_price][use_tax]=1&price[my_price][product_attribute]=25`

Before PrestaShop 1.6.0.10, this query retrieved the price **without** tax. The behavior has been changed to make it more on par with needs.

### Parameters <a href="#chapter10-pricemanagement-parameters" id="chapter10-pricemanagement-parameters"></a>

Here is the list of available parameters when needing to define a custom price:

* country
* state
* currency
* group
* quantity
* decimals
* product\_attribute
* use\_tax
* use\_reduction
* use\_ecotax
* only\_reduction
