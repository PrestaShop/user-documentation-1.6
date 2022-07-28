# Customer Groups

PrestaShop enables you to give your customers certain privileges, by assigning them to Groups. You can create as many customer groups as needed, and assign a user to as many groups as you like.

This is all done from the "Groups" page, under the "Customers" menu.

![](<../../../.gitbook/assets/23038771 (1).png>)

By default, three special groups are available:

* **Visitor**. All persons without a customer account or unauthenticated.
* **Guest**. All persons who placed an order with the Guest Checkout – that option needs to be enabled.
* **Customer**. All persons who created an account on your shop, and are authenticated.

These three groups cannot be deleted.

To create more groups, click the "Add New" button: you will get a creation form.

![](<../../../.gitbook/assets/23038774 (1).png>)

* **Name**. Use a short and descriptive name.
* **Discount (%)**. The discount that you set for members of this group applies to all products on your shop.\
  &#x20;You may prefer to not set any discount value, and create cart rules. You can learn more about cart rules in the next chapter of this guide, "Creating Price Rules and Vouchers".
* **Price display method**. PrestaShop is frequently used in the Business to Business (B2B) sector. You can create a group of customers who can buy products without paying the tax. The drop-down list gives you a choice between "tax included" and "tax excluded".
* **Show prices**. By default, all users of your shop can view the prices. You may prefer some to not have access to your product prices. For instance, you could make it so users can only view prices if they have an account: from the groups list, click on the green "Yes" in the "Show prices" column for the "Visitors" group to turn it into a red "No".

Once these settings are in place, you can save the group as-is, or add per-category and/or per-module settings. In that second case, after the group has been saved, open it again: the form will load with two more options:

* **Category discount**. Click on the "Add a category discount" to bring up a new window, which contains a list of all your categories. You can pick one, and apply a specific discount which will apply for that group of customers only, and to that category only.\
  Note that:
  * Only products which have this category as their default category will be affected by the discount. Products which have this category as a secondary category will not be affected.
  * This category discount will replace any other discount that members of this group would otherwise enjoy on this category.
  * You can add as many category discounts for this customer group as you need – thereby enabling to entirely give this group a whole set of different discounts if you feel the need.
* **Authorized modules**. This section enables you to block members of this group to access and use some of your shop's modules. For instance, you might prefer some customers to not be able to see your top-sellers or to your specials.&#x20;

![](<../../../.gitbook/assets/23038775 (1).png>)

You can add a customer to a group of your choice by editing the customer's details: from the list of customers (in the "Customers" page under the "Customers" menu), click on the Edit button on the customer's row. Then, in the "Group access" table, select the group(s) to which you want your customer to belong. If you assign the customer to more than one group, remember to set their main group with the "Default customer group" option.

![](<../../../.gitbook/assets/23038778 (1).png>)
