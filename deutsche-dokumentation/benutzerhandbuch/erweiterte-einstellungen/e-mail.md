# E-Mail

Ihr Shop sendet viele Nachrichten, über die Registrierung bis zur Bestellung. Hier können Sie festlegen, wie diese Nachrichten gesendet werden sollen, und sehen, welche Mails gesendet wurden.

PrestaShop Cloud user?

Wenn Sie die PrestaShop Cloud für Ihren Online-Shop benutzen, gibt es einige spezifische Informationen, die Sie über Ihre E-Mail-Konfiguration kennen müssen. Besuchen Sie hierzu diese Seite: [http://doc.prestashop.com/display/CLOUD/Managing+your+email+domain+name](http://doc.prestashop.com/display/CLOUD/Managing+your+email+domain+name).

## E-Mail <a href="#e-mail-e-mail" id="e-mail-e-mail"></a>

Der erste Abschnitt der Seite zeigt Ihnen eine Liste aller E-Mails, die von PrestaShop geschickt wurden, mit dem Empfänger, der verwendeten Vorlage, der Sprache der Nachricht, der Betreffzeile der E-Mail und dem Status der Aktion.

![](<../../../.gitbook/assets/38469764 (1).png>)

## E-Mail <a href="#e-mail-e-mail.1" id="e-mail-e-mail.1"></a>

Hier können Sie entscheiden, wie Ihre E-Mails gesendet und empfangen werden.

Das Formular besteht aus drei Gruppen von Optionen:

![](<../../../.gitbook/assets/38469765 (1).png>)

* **E-Mail senden an**. Dies ist eine Front-End-Einstellung. Am Ende des Bestellvorgangs kann ein Kunde eine Nachricht an Ihre Mitarbeiter verfassen. Sie können wählen, an wen diese Nachricht gesendet wird, indem Sie aus der Dropdown-Liste wählen.
* E-Mail-Einstellungen: wie E-Mails auf technischer Ebene versendet werden. Wählen Sie zwischen den drei Optionen. Siehe unten für weitere Informationen.
* E-Mail-Format: wie E-Mails visuell geschickt werden. Wählen Sie zwischen den drei Optionen. Siehe unten für weitere Informationen.
* **E-Mails protokollieren**. Deaktivieren Sie diese Optionen, wenn Sie keinen Überblick mehr über die geschickten E-Mails von Ihrem Shop haben wollen.

### Technische Konfiguration <a href="#e-mail-technischekonfiguration" id="e-mail-technischekonfiguration"></a>

Konfigurieren Sie PrestaShop E-Mail, um Nachrichten an Ihre Kunden versenden zu können. Wir empfehlen Ihnen dringend, Ihren Web-Host zu konsultieren, um herauszufinden, welche Optionen Sie wählen sollten. Die Optionen sind:

* **Niemals Mails versenden**. Nutzen Sie diese Einstellung für Testzwecke. Sobald Ihr Shop öffentlich gemacht wurde, sollten Sie diese Einstellung vermeiden.
* **PHP-Funktion mail() verwenden**. Diese Option ist standardmäßig ausgewählt und empfohlen. Für den Fall, dass dies nicht funktioniert, verwenden Sie die Option SMTP unten.
* **Meine eigenen SMTP-Einstellungen verwenden**. In diesem Fall wird ein neuer Abschnitt mit mehreren Feldern angezeigt. Die Informationen für diese Felder sollten von Ihrem Web-Host zur Verfügung gestellt werden: Mail-Domain, SMTP-Server, SMTP-Benutzername usw. Achten Sie darauf, genau zu kopieren, was Ihr Web-Host Ihnen an Informationen gibt.

Die SMTP-Konfigurationsinformationen können Ihnen von folgenden Instanzen zur Verfügung gestellt werden:

* Ihr System-Administrator,
* Ihr Host,
* Ihr ISP
* Ihr E-Mail-Anbieter.

![](<../../../.gitbook/assets/23789857 (1).png>)

Ihr Web-Host kann Ihnen sagen, ob Ihr Benutzername obligatorisch ist, sowie das Passwort und die Verschlüsselung übermitteln.

Im Fall von Google Mail (E-Mail-Service von Google) müssen Sie möglicherweise Informationen wie die folgende eingeben:

* SMTP-Server: [smtp.gmail.com](http://smtp.gmail.com)
* Benutzer: [my.user.name@gmail.com](mailto:my.user.name@gmail.com) (Beispiel)
* Kennwort: RT22UE87 (Beispiel)
* Verschlüsselung: SSL
* Port: 465

### Visuelle Konfiguration <a href="#e-mail-visuellekonfiguration" id="e-mail-visuellekonfiguration"></a>

Es stehen zwei Formate für E-Mails zur Verfügung: HTML ist schön anzusehen, aber funktioniert vielleicht nicht überall; Text ist langweilig anzusehen, aber funktioniert garantiert überall.

Sie können wählen, ob Sie nur eines der beiden nutzen möchten, oder beide. Beide ist die empfohlene Methode.

## Test Ihrer E-Mail-Einstellungen <a href="#e-mail-testihrere-mail-einstellungen" id="e-mail-testihrere-mail-einstellungen"></a>

Nachdem Sie Ihre E-Mails mit einer der beiden Methoden eingestellt haben, geben Sie Ihre eigene E-Mail-Adresse in diesem Abschnitt an und klicken auf die "Test-E-Mail senden".\
Überprüfen Sie nun Ihren Posteingang, um sicherzustellen, dass Sie die Test-E-Mail erhalten haben, im richtigen Format. Wenn Sie sie nicht erhalten haben, aktualisieren Sie Ihre Konfiguration mit den richtigen Informationen.

![](<../../../.gitbook/assets/38469768 (1).png>)
