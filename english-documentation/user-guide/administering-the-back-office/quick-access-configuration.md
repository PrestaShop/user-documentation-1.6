# Quick Access Configuration

PrestaShop has handy shortcuts to your most important pages, which can be accessed through the "Quick Access" menu, at the top right of every page of the PrestaShop back office (right next to the username).

The "Quick Access" administration page enables you to create customized shortcuts, and make your navigation within the administration area even more relevant to you and your team.

![](<../../../.gitbook/assets/41418943 (1).png>)

The page displays all the shortcuts that have already been created. By default, they are:

* **New category**. This special link takes you directly to the category creation form.
* **New product**. This special link takes you directly to the product creation page.
* **New voucher**. This special link takes you directly to the voucher/cart rule creation page.

Pages that open in a new tab/window will have a green "Enabled" in the "New window" column.

You can create as many shortcuts as needed – just do not overdo it, obviously, since this would render the "Quick access" menu slower to read.

## Adding a new link <a href="#quickaccessconfiguration-addinganewlink" id="quickaccessconfiguration-addinganewlink"></a>

Let's create a shortcut the order creation page, from which you can create a new order, and even add new customers and their addresses on the fly.

![](<../../../.gitbook/assets/41418944 (1).png>)

As usual, clicking the "Add New" button takes you to the creation form:

* **Name**. Give the shortcut a unique name. Make it short and descriptive.
* **URL**. Indicate the page's address. Here is how you can use even pages with complex links as quick links:
  1. While keeping the link creation page open, go to the "Orders" page under the "Orders" menu in a new browser tab.
  2. Copy its web address from the browser's address bar. For instance, http://www.myprestashop.com/admin8945/index.php?controller=AdminOrders\&token=f326b0419984706791c03f7e96599147.
  3. Remove the whole `&token=xxx` part and keep the specific bits (i.e., do not keep the domain and `/admin8945` folder). In our case: `index.php?controller=AdminOrders`.
  4. Paste the result in the "URL" field of the creation form.
* **Open in new window**. Indicate whether you want to have this tab open in a new window or not. In general, link to the back office should be kept within the same tab/window, and links leading outside of the back office (front office, other site altogether) should open in a new window/tab.

Note that you can create links to other websites, for instance your PayPal account or your webmail. Simply paste the complete URL in the "URL" field, including the `http://` prefix.
