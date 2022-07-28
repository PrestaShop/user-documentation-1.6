# Chapter 7 - Data removal: Removing customer accounts from the database

**Objective**: A Web application for listing and deleting customers.\
**Difficulty**: \*

## Preparation <a href="#chapter7-dataremoval-removingcustomeraccountsfromthedatabase-preparation" id="chapter7-dataremoval-removingcustomeraccountsfromthedatabase-preparation"></a>

Duplicate file `list_the_customers.php` from Chapter 3, rename it to `D-CRUD.php` and put it at the root of your Web server.

For this last part of our tutorial, we will learn how to delete a resource.

Here is the complete, detailed code you need in order to remove a customer:

```
try {
    // Create an instance
    $webService = new PrestaShopWebservice('http://example.com/' , 'ZR92FNY5UFRERNI3O9Z5QDHWKTP3YIIT' , false); 
	$opt['resource'] = 'customers';            // Resource to use
	opt['id'] = 3;                             // ID to use
	$webService->delete($opt);                 // Delete
    // If we can see this message, that means we have not left the try block
	echo 'Customer '.opt['id'].' successfully deleted!'; 
}
catch (PrestaShopWebserviceException $ex) {
	$trace = $ex->getTrace();                // Retrieve all info on this error
	$errorCode = $trace[0]['args'][0];       // Retrieve error code 
	if ($errorCode == 401) 
		echo 'Bad auth key';   
	else 
		echo 'Other error: <br />'.$ex->getMessage(); 
	// Display error message{color}
}
```

This code enables you to remove a customer whose ID is "3". As you can see, deleting the customer differs only slightly from retrieving a resource. In fact the only thing different in the code lies in the method called: We will no longer call this method `get()` but instead simply `delete()`!

You must now replace the customer ID by a dynamically-defined ID.

Now create all the script that will display a list of customer IDs and delete a customer of your choice.

Again, if you have trouble, look at the code from the `4-delete.php` sample file.
