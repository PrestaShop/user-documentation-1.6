# Statuses

Having different order or return statuses enables you to easily manage your orders and returns, and keep your customers informed of the evolution of their purchase.

The various available statuses are visible and editable in the "Statuses" page, under the "Orders" menu.

![](<../../../.gitbook/assets/38109199 (1).png>)

The page displays a list of the currently registered order statuses, along with:

* Their distinctive colors: existing status have colors that help quickly decide if there's an issue with the order or if it all goes well.
* Their icons.
* Their ties to three PrestaShop behaviors (more are available):
  * Should the customer receive e-mail when the order gets this status?
  * Is this a delivery status?
  * Does this status allow the customer to download and view a PDF version of the order's invoice?
* The name of their e-mail template: you can edit these templates, language by language, in the "Translations" page under the "Localization" menu. In the "Modify translations" section of that page, choose "E-mail template translations" in the drop-down menu, and then click on the language code of the language in which you wish to edit these templates.
* Their action icons: "edit" and "delete".

The return status list features less information, because those statuses are merely labels with no impact on the order.

![](<../../../.gitbook/assets/23038627 (1).png>)

## Creating a new order status <a href="#statuses-creatinganeworderstatus" id="statuses-creatinganeworderstatus"></a>

You can create a new status with the "Add New" button at the top. The creation form opens.

![](<../../../.gitbook/assets/23038625 (1).png>)

Fill out the form:

* **Status name**. Keep it very short and distinctive.
* **Icon**. You can use any 16\*16 icon; for instance, the excellent and free FamFamFam Silk icon set: [http://www.famfamfam.com/lab/icons/silk/](http://www.famfamfam.com/lab/icons/silk/).
* **Color**. You should strive to have the status' color match the existing colors (if relevant). The default color usages are:
  * Red/Orange: canceled or refunded orders,
  * Crimson red: payment error,
  * Blue: orders which are still awaiting payment,
  * Light green: paid orders,
  * Dark green: delivered orders,
  * Purple: shipped orders,
  * Pink: backordered orders.
* Options:
  * **Consider the associated order as validated**. If enabled, this status marks all associated orders as "paid", and puts them in this same status.
  * **Allow a customer to download and view PDF versions of their invoice**. If disabled, you will have to send customers their invoice yourself.
  * **Hide this state in all customer orders**. This enables you to create internal statuses, for you and your team. Customers will never see this in their order status page.
  * **Send an e-mail to customer when his/her order status has changed**. When enabled, a drop-down menu appears to let you choose which mail template to use.
  * **Set the order as shipped**. Be careful: once an order is set as "shipped", it cannot be set back to the previous status.
  * **Set the order as paid**. Same here: once an order is set as "paid", it cannot be set back to the previous status.
  * **Show delivery PDF**. Displays the delivery PDF.

## Creating a new return status <a href="#statuses-creatinganewreturnstatus" id="statuses-creatinganewreturnstatus"></a>

You can create a return status with the "Add New" button at the bottom. The creation form opens.

![](<../../../.gitbook/assets/23038630 (1).png>)

It only features two fields:

* **Status name**. Set your desired status name.
* **Color**. Set its color

Finally, save your creation.
