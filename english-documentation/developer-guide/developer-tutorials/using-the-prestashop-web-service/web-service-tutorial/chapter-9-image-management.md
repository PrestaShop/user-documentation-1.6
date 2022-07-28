# Chapter 9 - Image management

Accessing the images is done through the `images` entity.

Several types of images are available.

* General shop images
* Product images
* Category images
* Customization images
* Manufacturer images
* Supplier images
* Store images

They can be reach using the following links:

* /api/images/general
* /api/images/products
* /api/images/categories
* /api/images/customizations
* /api/images/manufacturers
* /api/images/suppliers
* /api/images/stores\
  \


Various image size are available, depending on the image types. They are available as XLink links in the links above, encapsulated in the `image_types` node.

For instance, in order to retrieve the image with the id 10 for the product with id 5, we would use the following path: `/api/images/products/5/10`.

## Changing the images <a href="#chapter9-imagemanagement-changingtheimages" id="chapter9-imagemanagement-changingtheimages"></a>

In order to change the available images, we have to use a `POST` request, with the new image as its parameter.

For instance, here is how to **change** the image for category 2:

* HTTP method: POST ( /!\ not PUT)
* URL: /images/categories/2
* POST content: \[binary content for the new image]

...and here is how to **add** a new image to the product with id '1':

* HTTP method: POST
* URL: /images/products/1
* POST content: \[binary content for the new image]

Here is an HTML form enabling images to be sent:**Adding new image**

```
<form enctype="multipart/form-data" method="POST" action="http://eWURcnNJ6mbLUHB10EEIzTZsTShs33IX@myprestahop.com/api/images/products/1">
  <fieldset>
    <legend>Add image for products No 1</legend>
    <input type="file" name="image">
    <input type="submit" value="Execute">
  </fieldset>
</form>
```

**Update existing image**

```
<form action="http://eWURcnNJ6mbLUHB10EEIzTZsTShs33IX@myprestahop.com/api/images/products/1/2" method="POST" enctype="multipart/form-data">
<fieldset>
	<legend>Update product image 1/2</legend>
	<input name="ps_method" value="PUT" type="hidden">
	<input name="image" type="file">
	<input value="Execute" type="submit">
</fieldset>
</form>
```

If you would rather use cURL:

```
$url = 'http://myprestashop.com/api/images/products/1';
/**
 * Uncomment the following line in order to update an existing image
 */
//$url = 'http://myprestashop.com/api/images/products/1/2?ps_method=PUT';
 
$image_path = 'C:\\my_image.png';
$key = 'My web service key';

$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, $url);
curl_setopt($ch, CURLOPT_POST, true);
curl_setopt($ch, CURLOPT_USERPWD, $key.':');
curl_setopt($ch, CURLOPT_POSTFIELDS, array('image' => '@'.$image_path));
curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
$result = curl_exec($ch);
curl_close($ch);
```
