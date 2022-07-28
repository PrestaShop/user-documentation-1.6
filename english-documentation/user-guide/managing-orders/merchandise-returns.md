# Merchandise Returns

The "Merchandise Returns" page gives you a list of all the RMA process (Return merchandise authorization).

At the bottom of the page, you have the possibility of enabling customers to send products back to you ("Enable returns" option). Simply make a choice, indicate the number of days during which a return request can be made, and save your settings: customers now have the ability to ask for a return authorization. You can also edit the prefix for the return number, or chose not to have any.

![](<../../../.gitbook/assets/38109196 (1).png>)

## Return process: how the customer sees it <a href="#merchandisereturns-returnprocess-howthecustomerseesit" id="merchandisereturns-returnprocess-howthecustomerseesit"></a>

Once you have activated the RMA option in your back office, the customer can choose to return an item (provided the order is still in the time of validity). In order to do this, s/he must do the following:

1. Access the "Orders History" section of his or her account.
2. Select the order from which he wants to return an item.
3. Select the product(s) that s/he wishes to return by checking the box next to its name(s).
4. (optional) Add an explanation, in order for the shop team to better understand why the customer wants to return this product.

![](<../../../.gitbook/assets/23038595 (1).png>)

When is it possible to return an order?

1. Returns have to be enabled ("Enable returns" option).
2. The order has to be in the time of validity.
3. The orders needs to have had at least the following statuses:

*

    * At least two statuses of which one has the option "Set the order as paid" enabled and the other has the option "Set the order as shipped" enabled.\
      Or
    * One status which has both options ("Set the order as paid" and "Set the order as shipped") enabled.

    Statuses can be edited on the "Statuses" page under the "Orders" menu.

Once the form is complete, the customer clicks on "Make an RMA slip", and the request is sent to the store manager (you). The request appears as "Waiting for confirmation" in the customer's "Return Merchandise Authorization" page, accessible from the account page.

![](<../../../.gitbook/assets/23038597 (1).png>)

## Return process: how you see it <a href="#merchandisereturns-returnprocess-howyouseeit" id="merchandisereturns-returnprocess-howyouseeit"></a>

The return request appears in your back office. At first, the RMA has the "Waiting for confirmation" status.

![](<../../../.gitbook/assets/23038598 (1).png>)

The refund process can take several steps, which are indicated by the RMA status. There is just a handful of statuses, which can follow the whole RMA process:

* Waiting for confirmation.
* Waiting for package.
* Package received.
* Return denied.
* Return completed.

![](<../../../.gitbook/assets/23038601 (1).png>)

It is now up to you to accept it or deny it:

1. Click on the name of the return request to see more details.
2. Change the status to continue with the return process or stop it.
   * If you want to stop the return process (and deny the customer a refund), simply choose the "Return denied" status.
   * If you agree with the product being returned and the customer being refunded, follow each step precisely:
     1. Choose the next step in the process: "Waiting for package". This will send an e-mail to the customer indicating that the product can be sent back to you.
     2. Once you have received the package, change the RMA's status to "Package received".
     3. Finally, once the whole process is over (either the customer has been refunded or you have issued a credit slip), change the RMA's status to "Return completed".
3. Validate.

## Refunding a customer <a href="#merchandisereturns-refundingacustomer" id="merchandisereturns-refundingacustomer"></a>

An order can be refunded, either partially or totally. This is done using two actions buttons located in the top bar of the order's page itself rather than in the RMA page**.**

The action buttons change depending on the order's status. For instance, once the order is in the "Delivered" state, the "Add a product" and "Remove products" turn into two new buttons: "Return products" and "Partial refund".

Product return is not activated by default. To activate it, go to the "Product returns" page under the "Orders" menu, and activate the option in the option section at the bottom of the page. This will apply to all products and all orders.

![](<../../../.gitbook/assets/23038603 (1).png>)

* **Return products**. To be used only when the customer has effectively returned products: once the returned product has been received, you can mark it as returned directly in the order form. Click the "Return products" button and a new column will appear in the product list, titled "Return". Check the box of the affected products, indicate the quantity of items that were returned, and click the "Return products" button at the bottom of the table.
* **Partial refund**. To be used when you need to refund only part of the order and not the whole order, either because the customer returned the ordered product, or simply as a sign of goodwill for a damaged product that the customer chose to keep anyway. Click the "Partial refund" button and a new column will appear in the product list, titled "Partial refund". Set the amount and quantity for each of the affected products, choose one of the option at the bottom of the list (see below), and click the "Partial refund" button at the bottom of the table.

When you set a product as returned or to be refunded, four options are available below the list of products:

* **Re-stock products**. When checked, PrestaShop will consider that the returned product as available for sale again, and will therefore increase the stock for this product. You should not click this when a product is return due to it being broken...
* **Generate a credit slip**. When checked, a credit slip will be created for the selected items. A credit slip is an acknowledgment from your shop that merchandise has been returned and that a refund has been issued. The customer can then use it as a credit slip for his or her next purchase.
* **Generate a voucher**. When checked, a voucher will be created for the amount of the selected items. A voucher takes the form of a discount code that the customer can enter during the checkout process.\
  You can edit the customer's existing vouchers by viewing the customer's page: from the current order's page, click on the link under the customer's name in the "Customer information" section; once in the customer's page, reach the "Vouchers" section. You can edit each voucher by clicking on the "Edit" icon.
* **Repay shipping cost**. You can also choose to refund the shipping cost of the returned product, which is always an appreciated gesture.

If the customer paid the order using a credit card, the payment system may refund the cart automatically, or you may have to do it yourself. If the order was paid using a check or a bank transfer, you have to issue the refund yourself, then mark the order as having been refunded manually in the back office (in the order's page).
