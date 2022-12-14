# Logs Parameters

Errors happen. Most of the time, you are not aware of them because PrestaShop handles them silently. But you might want to know about them, in order to be able to correct the most regular ones, and ensure a better stability for your shop.

![](<../../../.gitbook/assets/43417626 (1).png>)

The "Logs" page is where you can have a look at the PHP errors which plague your shop. They are listed in the page's central table, and are presented in 4 levels:

* **1: Informative only**. Run-time notices. Indicate that the script encountered something that could indicate an error, but could also happen in the normal course of running a script.
* **2: Warning**. Run-time warnings (non-fatal errors). Execution of the script is not halted.
* **3: Error**.
* **4: Major issue (crash)!**. Fatal run-time errors. These indicate errors that cannot be recovered from, such as a memory allocation problem. The execution of the script is halted.

These explanations are the official ones from the PHP manual. Read more: [http://www.php.net/manual/en/errorfunc.constants.php](http://www.php.net/manual/en/errorfunc.constants.php).

## Logs by e-mail <a href="#logsparameters-logsbye-mail" id="logsparameters-logsbye-mail"></a>

The error levels also serve as values for the "Logs by e-mail" feature.\
PrestaShop adds one last value, 5, which indicates that the administrator does not want to receive any notification, either for minor or major errors.

![](<../../../.gitbook/assets/23789888 (1).png>)

The error logging tool enables you to receive an e-mail notification when an error occurs. Notifications are sent to the shop owner's e-mail address, and you can configure the degree of importance at which you should start receiving such e-mails:

* "1" if you want to know about everything, even the tiniest information.
* "3" if you only want to know about issues (errors and major issues).
* "4" if you only want to keep the major issues.
* "5" is the default, meaning that no notification is sent.
