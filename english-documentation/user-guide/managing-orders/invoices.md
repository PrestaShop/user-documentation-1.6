# Invoices

Each time an order from your shop is validated, an invoice is sent out to the customer. You can download the invoices for a single order from the order's page. The "Invoices" page under the "Orders" menu enables you to download a selection of invoices from past orders in PDF format, all at the same time (in the same PDF file).

![](<../../../.gitbook/assets/30245492 (1).png>)

You can get a PDF file containing several invoices depending on two main criteria:

* **By date**. Very useful when you need to print all invoices for a given month or a given quarter. Select the start and end date, and click on the "Generate PDF file by date" button in the top bar.
* **By order status**. A must-have when you need to print precisely which orders are canceled, refunded or on backorder. PrestaShop helpfully indicates the number of invoices tied to each status in parentheses.

In both cases, the invoices are generated into a single PDF file, each with their own pages. You cannot get a single PDF file for each invoice of the given period or statuses using this page.

If you want to customize the look of your store's invoices, you must change its template files.

PDF template files are located in the `/pdf` folder. Open the `invoice.tpl` file and edit it to your likings: it is an HTML file with Smarty tags.

## Invoice Options <a href="#invoices-invoiceoptions" id="invoices-invoiceoptions"></a>

You can choose whether or not invoices should available to your customers as soon as the order is made, as well as the Invoice Prefix and the invoice number you want listed on the printed version of the invoice. This feature can help you simplify the management of your account.

![](<../../../.gitbook/assets/38109193 (1).png>)

* **Enable invoices**. When disabled, your customer will not receive an invoice after their purchase. You will be responsible for handling the invoices, if your customers ask for one.
* **Enable tax breakdown**. _New in 1.6_. When enabled, the invoice lists all the various taxes that were applied to the order, instead of just one percentage.
* **Enable product image**. _New in 1.6.1._ When enabled, it will add the product's image next to the product name in the invoice.
* **Invoice prefix**. By default, PrestaShop has language-adapted invoice prefixes: "IN" in English, "FA" in French (for "_facture_"), "CU" in Spanish (for "_cuenta_"), etc. You could choose to have language codes instead: "EN", "FR", "SP", etc. Of course, you can also choose to have a single prefix for every language, or to not have a prefix at all.\
  &#x20;PrestaShop will then generate the invoices number according to you settings: "#IN000001", "#FA000002", etc.
* **Invoice number**. If your business has already had orders and invoices before you started using PrestaShop, you can use this option to start your invoice number from a higher number.
* **Legal free text.** _New in 1.6.1.0_. This field allows you to add some extra content to the invoice, in case your local legislation require you to display additional information. On the invoice, it will appear below the payment methods summary. Of course, you can use this free text to display any text you deem necessary.
* **Footer text**. You can use this to have a custom text at the bottom of all your invoices. The text will appear below the name of your shop in the invoice.
* **Invoice model**. Depending on your themes, you might be able to use more than one style of invoice. Test them with a fake order, in order to choose the one you prefer. If you know how to code in HTML, you can add your own invoice models or edit the existing ones: they are located in the `/pdf/` folder of your PrestaShop installation.
* **Use the disk as cache for PDF invoices**. You can choose to store generated invoices on PrestaShop's server disk rather than in its server cache. While it saves on memory usage, it slows down the PDF generation itself, so use it knowingly.

Do not forget to save your changes.

When your customers ask for their invoices, you can redirect them to the "Order History" section of their user accounts, which keeps all of their invoices available for them.
