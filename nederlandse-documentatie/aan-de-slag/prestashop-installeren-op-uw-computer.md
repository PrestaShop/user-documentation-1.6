# PrestaShop installeren op uw computer

U kunt PrestaShop installeren op uw eigen lokale computer, om uit te proberen, voordat u besluit te investeren in een server en domeinnaam, of om uw winkel lokaal aan te passen, voordat u uw wijziging naar toepast op de PrestaShop-installatie die u al online hebt staan.

Het lokaal installeren van een webapplicatie vereist dat u een adequate omgeving beschikbaar hebt, namelijk de Apache Webserver, PHP, MySQL-database server en optioneel de software phpMyAdmin. Deze stack is ook bekend als AMP: Apache+MySQL+PHP. Het is te installeren op veel verschillende besturingssystemen. Afhankelijk van het systeem ontstaan de volgende acroniemen: WAMP (Windows+Apache+MySQL+PHP), MAMP (Mac OS X+...) en LAMP (Linux+...)

## Een AMP-pakket kiezen <a href="#prestashopinstallerenopuwcomputer-eenamp-pakketkiezen" id="prestashopinstallerenopuwcomputer-eenamp-pakketkiezen"></a>

Dit vereist normaal gesproken dat u vrij technisch bent; gelukkig bestaan er veel vooraf samengestelde pakketten die u met gemakt kunt installeren. Het voorkomt niet dat het af en toe een beetje technisch wordt, maar ze zijn heel erg handig om mee te beginnen. Aangezien de pakketten open source zijn, zijn de meeste gratis te downloaden. Hier zijn een aantal gratis AMP-installers:

* EasyPHP: [http://www.easyphp.org/](http://www.easyphp.org/) (Windows)
* MAMP: [http://www.mamp.info/](http://www.mamp.info/) (Mac OS X)
* WampServer: [http://www.wampserver.com/en/](http://www.wampserver.com/en/) (Windows)
* XAMPP: [http://www.apachefriends.org/en/xampp.html](http://www.apachefriends.org/en/xampp.html) (Windows, Mac OS X, Linux, Solaris)

EasyPHP heeft een speciaal alles-in-één-pakket. Deze heeft een installatieprogramma voor PrestaShop 1.6 gereed! Het is de gemakkelijkste manier om de nieuwste versies van PrestaShop uit te proberen en, voor ontwikkelaars, om thema's en modules te ontwikkelen.

Download het hier: [http://www.easyphp.org/prestashop.php](http://www.easyphp.org/prestashop.php)

Kies het pakket waarmee u het beste kunt werken, start deze,&#x20;

## Controleren of alles werkt <a href="#prestashopinstallerenopuwcomputer-controlerenofalleswerkt" id="prestashopinstallerenopuwcomputer-controlerenofalleswerkt"></a>

Zorg ervoor dat alle onderdelen van uw AMP-pakket werken, voordat u verder gaat met deze sectie:

*   **De webserver moet draaien.** U zou deze moeten kunnen bereiken met uw browser door `127.0.0.1` in de adresbalk te typen.

    [`http://127.0.0.1`](http://127.0.0.1/) is de "localhost", oftewel "uw computer": het is een zogeheten loopback adres welke uw browser naar uw lokale webserver stuurt.\
    Vaak zijn [`http://127.0.0.1`](http://127.0.0.1/) en [`http://localhost`](http://localhost/) synoniem aan elkaar: u kunt beide gebruiken, beide sturen u naar de hoofdmap van uw lokale webserver.

    Soms kan een webserver niet gestart worden omdat de lokale poort (meestal poort 80) al in gebruik is door een andere applicatie.

    Dit gebeurt vaak wanneer Skype is gestart. Om te voorkomen dat Skype deze poort bezet houdt, gaat u naar de geavanceerde instellingen van Skype (Extra > Verbindingsinstellingen... > Verbinding) en zorg ervoor dat "Poort 80 en 443 gebruiken voor extra inkomende verbindingen" is uitgevinkt. Start de webserver opnieuw op.
* **De database-server moet draaien.** De MySQL-server is waar PrestaShop al zijn data bewaart. Het AMP-pakket zou duidelijk moeten aangeven of MySQL is gestart of niet.
* **Het programma phpMyAdmin moet toegankelijk** **zijn.** Dit is de webapplicatie waarmee de MySQL-database beheerd kan worden. De locatie is afhankelijk van welk AMP-pakket u gekozen hebt: het kan gevonden worden op [`http://127.0.0.1/phpmyadmin`](http://127.0.0.1/phpmyadmin) (XAMPP, WampServer, MAMP), [`http://127.0.0.1/mysql`](http://127.0.0.1/mysql) (EasyPHP) of wellicht een andere locatie. Bekijk de documentatie van uw pakket - het programma kan zelfs een kopn hebben waarmee u gelijk de juiste URL opent in uw browser.

## De hoofdmap van uw lokale server vinden <a href="#prestashopinstallerenopuwcomputer-dehoofdmapvanuwlokaleservervinden" id="prestashopinstallerenopuwcomputer-dehoofdmapvanuwlokaleservervinden"></a>

Zodra u heeft gecontroleerd of het pakket juist is geïnstalleerd en dat alle onderdelen draaien, moet u op zoek gaan naar de hoofdmap van uw lokale webserver.

Dat is de map waar u alle bestanden van PrestaShop gaat plaatsen en is vergelijkbaar met het hoofdadres van bijvoorbeeld uw online-server. Het verschil is dat de lokale content bereikt wordt met [`http://127.0.0.1`](http://127.0.0.1/).

De echte locatie van de map hangt af van het AMP-pakket wat u gebruikt en is aanpasbaar:

* EasyPHP: `C:\easyphp\www`
* MAMP: `/Applications/MAMP/htdocs/`
* WampServer: `C:\wamp\www`
* XAMPP: `C:\xampp\htdocs` or `/Applications/xampp/htdocs`

## MySQL gebruikersinformatie vinden <a href="#prestashopinstallerenopuwcomputer-mysqlgebruikersinformatievinden" id="prestashopinstallerenopuwcomputer-mysqlgebruikersinformatievinden"></a>

Als laatste, moet u op zoek gaan naar de gebruikersnaam en wachtwoord van de 'root'-gebruiker, om PrestaShop te kunnen installeren.

**De meeste pakketten hebben de gebruikersnaam "root" met een leeg wachtwoord,** inclusief EasyPHP, MAMP, WampServer en XAMPP.

Lees de documentatie van uw pakket.

## Tot slot <a href="#prestashopinstallerenopuwcomputer-totslot" id="prestashopinstallerenopuwcomputer-totslot"></a>

Met de webserver helemaal klaar voor gebruik, kunt u de rest van deze Aan de slag gids volgen en beginnen met de installatie van PrestaShop.

Wanneer u PrestaShop lokaal installeert, denkt u dan aan de volgende punten:

* Bestanden worden niet FTP-software (zoals FileZilla) naar een webserver: kopieer ze simpelweg naar de juiste lokale map, zoals hierboven aangegeven.
* U hoeft geen lokale domeinnaam aan te maken: PrestaShop is beschikbaar via het loopback adres zoals hierboven aangegeven. Deze is of [`http://localhost`](http://localhost/)`,` [`http://127.0.0.1`](http://127.0.0.1/) `of allebei`. PrestaShop zelf is beschikbaar via dit adres door de map van PrestaShop toe te voegen, bijvoorbeeld [`http://localhost/prestashop`](http://localhost/prestashop) of [`http://127.0.0.1/prestashop`](http://127.0.0.1/prestashop) als PrestaShop zich in de `/prestashop/` submap bevindt. Wanneer de URL voor het eerst wordt aangesproken, wordt u direct begeleid naar het installatieprogramma van PrestaShop ([`http://localhost/prestashop/install`](http://localhost/prestashop/install) of [`http://127.0.0.1/prestashop/install`](http://127.0.0.1/prestashop/install)).

Heeft u alles gelezen? Volg dan weer het normale gedeelte van de installatie gids. U kunt gelijk verder met de sectie [Database aanmaken voor uw winkel](prestashop-installeren.md#PrestaShopinstalleren-Databaseaanmakenvooruwwinkel).
