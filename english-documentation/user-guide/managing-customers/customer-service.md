# Customer Service

PrestaShop enables you to centralize all the customers' request within its confines. This helps you keep track of which discussion threads needs answering, rather than having to check with all the recipients of the mail to see if someone did answer it.

In practice, the contact form of your shop, available under the "Contact us" link at the bottom of your front office, presents the customer with two contacts by default: "Webmaster" and "Customer Service". The customer only has to choose who to contact, and then fill the rest of the fields. The message is then recorded in PrestaShop's customer service tool.

![](<../../../.gitbook/assets/30670851 (1).png>)

Discussion threads are only included in the customer service tool if the contact has the "Save Message?" option enabled. You can change this setting, or add more contacts, by going to the "Contact" page, under the "Customers" menu. This page is explained in detail in the next section of this chapter of the PrestaShop User Guide.

If the option is disabled for the contact that the customer chooses, the message is simply sent to the contact's e-mail address, and is not stored in PrestaShop.

You also need to properly configure your IMAP settings, so that PrestaShop can retrieve the customer's answers to e-mail that were sent from the customer service tool. This is done in the "Customer service options" section, at the bottom of the screen.

On this page, each contact has its own box, where you can quickly see if a there are new messages (meaning, those that have not yet been read). By default there are two, and adding more contacts will move the "Meaning of status" and "Statistics" boxes further to the left and down.

These two last boxes are handy when you need to handle new messages daily:

* **Meaning of status**. A simple reminder of the color codes that your team can apply to a discussion thread.
* **Customer service: statistics**. An overview of the global activity of your customer service since the beginning.

Further below is the list of received messages, both old and new.

You can edit a couple options at the bottom of the page, which apply to all contacts:

* **Allow file uploading**. Whether the customer can attach a file to the message. This can be useful in case of visual issues on the front-page, as the customer can send you screen captures.
* **Pre-defined message**. The default template for your employees' answer. Keep it simple, so that it can adapt to many situations, even if it needs a little editing for each case.

Finally, the bottom of the page features the "Customer service options" section, where you can set many options pertaining to your mail (IMAP) server.

## Handling Customer Service Messages <a href="#customerservice-handlingcustomerservicemessages" id="customerservice-handlingcustomerservicemessages"></a>

Each conversation with a customer can be entirely handled through PrestaShop's complete interface, without having to use an e-mail client such as Outlook or Thunderbird.

![](<../../../.gitbook/assets/23038786 (1).png>)

In the conversation list, click on a row to view the conversation's details:

* You can apply a handful of actions to a discussion, in order to quickly sort them and thus handle them quicker. There are 4 available actions:\

  * **Mark as "handled"** or **"Re-open"**. Changes the discussion's status to "Closed" or "Open".
  * **Mark as "pending 1"** and **Mark as "pending 2"**. These two statuses are internal: their meaning is up to your team. You may even choose to not use them, and only rely on "Closed" and "Open".
  * **Forward this discussion to another employee**. From the moment an employee has started replying to a customer message, he becomes in charge of the customer's request. If during the discussion it turns out another employee should handle it instead of you, you can use that button to attribute it through a drop-down list. That other employee will receive a notification about it. If the person you want to forward this discussion to is not available in the list, choose "Someone else" in the dropdown list and two options will appear, enabling you to indicate the email address of the recipient and a comment about your message.
* **Reply to the next unanswered message in this thread**.

Essential details are available:

* Customer name and email, which you can click on to access the customer's information
* Number of orders, total amount spent and date of registration for the customer.
* Time and date of the message.
* Finally, the message itself.

To reply to this thread, simply use the form with your default message (as set in "Contact options" section of the "Customer service" page), and click "Send".

At the bottom of the page, the "Orders and messages timeline" gives you a clear chronological view of the events pertaining to this discussion thread.

![](<../../../.gitbook/assets/23789570 (1).png>)

## Customer Service Options <a href="#customerservice-customerserviceoptions" id="customerservice-customerserviceoptions"></a>

This section basically enables you to precisely configure PrestaShop's access to your e-mail server through its IMAP interface. You should make sure all fields are filled in order for the customer service tool to work properly. Most of this information should be provided by your webhost.

![](<../../../.gitbook/assets/23789573 (1).png>)

* **IMAP URL**, **IMAP port**, **IMAP user** and **IMAP password**. Essential details to access the e-mail server using the IMAP protocol.
* **Delete message**. If enabled, messages on the server will be deleted as soon as PrestaShop has retrieved them. Use with caution: this would make your messages unavailable to other e-mail clients.
* **/norsh**. If enabled, the connection to your e-mail server will not pre-authenticated. Not recommended.
* **/ssl**. If enabled, the connection to your e-mail server will not be encrypted. Not recommended.
* **/validate-cert**. If enabled, PrestaShop will force the validation of the server's TLS/SSL certificate.
* **/novalidate-cert**. If enabled, PrestaShop will never try to validate the server's TLS/SSL certificate. Essential for servers with self-signed certificates.
* **/tls**. If enabled, PrestaShop will force use of StartTLS to encrypt the connection. Servers that do not support StartTLS will be rejected.
* **/notls**. If enabled, PrestaShop will not use StartTLS to encrypt the session, even with servers that support it.
