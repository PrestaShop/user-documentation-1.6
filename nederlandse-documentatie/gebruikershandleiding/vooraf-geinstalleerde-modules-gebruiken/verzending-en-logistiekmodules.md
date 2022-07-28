# Verzending- en logistiekmodules

## Verzendkostenberekening <a href="#verzending-enlogistiekmodules-verzendkostenberekening" id="verzending-enlogistiekmodules-verzendkostenberekening"></a>

Deze module maakt het mogelijk voor klanten om vervoerdersmogelijkheden te vergelijken voordat ze naar de afrekenpagina gaan.

Deze module is vanzelfsprekend: installeer deze om de opties op uw frontoffice te tonen.

De kosten van de vervoerders moeten op de juiste manier zijn ingesteld. Dit kan worden gedaan op de pagina "Vervoerders".

De configuratiepagina van de module heeft slechts één optie "Hoe de verzenderslijst updaten?". Dit maakt het mogelijk om een vervoerder te tonen als alle informatie beschikbaar is of op elk moment.

## Leveringsdatum <a href="#verzending-enlogistiekmodules-leveringsdatum" id="verzending-enlogistiekmodules-leveringsdatum"></a>

Deze module toont de verwachte leverdatum bij het afrekenen.

De configuratiepagina heeft twee secties:

* **Linklijst**. De module is afhankelijk van informatie van uw vervoerders. U moet daarom regels toevoegen voor elke vervoerder, door te klikken op de knop "Nieuwe vervoerdersregel toevoegen".
* **Instellingen**:
  * **Extra tijd wanneer een product niet voorradig is**. Schat de tijd in die het kost om producten weer op voorraad te krijgen. Dit is alleen nuttig wanneer klanten producten kunnen bestellen die niet op voorraad zijn (optie is te vinden op de pagina "Producuten" in de sectie "Producten voorraad").
  * **Extra tijd om order voor te bereiden**. Schat de tijd in die het kost om een bestelling voor te bereiden.
  * **Voorbereidingsoptie**. Als uw inpakteam ook in het weekend werkt, kunt u dit hier aangeven.
  * **Datum formaat**. Het formaat waarin de verwachtte datum wordt getoond. Het gebruik het `PHP date()` formaat: elke letter heeft een betekenis, zoals uitgelegd in de bijbehorende link. De standaard "l j F Y" komt neer op dit formaat: "Zaterdag 21 januari 2012". Er zijn nog meer instellingen die u kunt gebruiken. Bekijk daarvoor deze pagina:  [http://www.php.net/manual/en/function.date.php](http://www.php.net/manual/en/function.date.php).

Een nieuwe vervoerdersregels is eenvoudig:

* **Vervoerder**. Kies de vervoerder voor wie u een nieuwe regel wilt toevoegen. Als de gewenste vervoerder nog niet bestaat moet u deze eerst aanmaken.
* **Leveren tussen**. Stel het tijdsframe in waarbinnen de vervoerder bestellingen belooft te kunnen leveren. U moet deze informatie bij de vervoerder opvragen.
* **Afleveringsopties**. Sommige vervoerders sorteren pakketten ook tijdens het weekend, dus u kunt daarvoor deze opties gebruiken om dit aan te geven.

U moet zoveel vervoerdersregels toevoegen als nodig is.

## Fedex (fedexcarrier) <a href="#verzending-enlogistiekmodules-fedex-fedexcarrier" id="verzending-enlogistiekmodules-fedex-fedexcarrier"></a>

Biedt uw klanten verschillende bezorgmethoden aan met behulp van FedEx.

## Globkurier <a href="#verzending-enlogistiekmodules-globkurier" id="verzending-enlogistiekmodules-globkurier"></a>

**Alleen voor Polen.**

![](../../../.gitbook/assets/23036725.png)

[GlobKurier.pl](http://globkurier.pl) is one of the biggest national leaders in delivering shipments. We provide domestic and international services to more than 200 countries. Our main aims are competitive price, speed and security. With [GlobKurier.pl](http://globkurier.pl) you can be sure that your shipments always come on time. Moreover we offer convenience of using our services.

## GoInterpay <a href="#verzending-enlogistiekmodules-gointerpay" id="verzending-enlogistiekmodules-gointerpay"></a>

![](../../../.gitbook/assets/23038228.png)

U kunt meer dan 200 betaalmethoden toevoegen aan uw webwinkel met één simpele integratie.

## Mondial Relay <a href="#verzending-enlogistiekmodules-mondialrelay" id="verzending-enlogistiekmodules-mondialrelay"></a>

**Alleen voor Frankrijk, Luxemburg, Spanje en België.**

This module enables you to display rates for delivering in Mondial Relay points. This service is available in France, Luxembourg, Spain and Belgium.

You must have a Mondial Relay account in order to use this service. You can reach the sign-up form here: [http://www.mondialrelay.com/](http://www.mondialrelay.com/).\
Then, from the module's configuration page, click on the "Account details" icon and enter the necessary information, as provided by Mondial Relay: Webservice Enseigne, Code marque, Webservice Key, Etiquette's Language and Weight Coefficient. The Etiquette's Language can only use the languages that are enabled on your shop; you can enable more language from the "Languages" page, under the "Localization" menu. Click "Update Settings" in order to connect your shop to the Mondial Relay webservice, and from there on, follow the module's instructions in the "Shipping" and "Advanced settings" screens.

Once the settings are in place, your customers will see the "Mondial Relay" option appear in the shop's front office as part of the available delivery methods.

## So Colissimo <a href="#verzending-enlogistiekmodules-socolissimo" id="verzending-enlogistiekmodules-socolissimo"></a>

**Alleen voor Frankrijk.**

This module enables you to display rates for deliveries via SoColissimo, a service by La Poste, France's historical postal service. This service is available mainly in France.

You must have a SoColissimo account in order to use this module. This is done by calling La Poste from a French phone, using this number: **3634**.\
Then, configure the module with your SoColissimo information: ID So, key, preparation time, overcost, URL So, Fancybox, Supervision and Supervision URL.\
A full documentation is available (in French) as a PDF file, which you can find under the "Documentation" link on the configuration page.

In order to finalize the installation, copy/paste the two final URLs in your SoColissimo back office.

Once the settings are in place, your customers will see the "SoColissimo" option appear in the shop's front office as part of the available delivery methods.

## TNT Express France <a href="#verzending-enlogistiekmodules-tntexpressfrance" id="verzending-enlogistiekmodules-tntexpressfrance"></a>

**Alleen voor Frankrijk.**

This module enables you to display rates for deliveries via TNT express services. This service is available worldwide.

You must have a TNT account in order to use this module. You can reach the sign-up form here: [http://www.tnt.com](http://www.tnt.com/).\
Then, configure the module with your TNT login, password and account number, all in the "Account settings" tab.\
From there on, you can keep configuring the module using the "Shipping Settings" and "Service Settings" tabs. This last tab enables you to be very specific about the delivery service you want to make available for your customers, as well as any additional charge you might require depending on the package's weight.

Once the settings are in place, your customers will see the "TNT Express France" option appear in the shop's front office as part of the available delivery methods.

## Tracking - Front office <a href="#verzending-enlogistiekmodules-tracking-frontoffice" id="verzending-enlogistiekmodules-tracking-frontoffice"></a>

This module completes PrestaShop with an integrated affiliate program feature, which enables your affiliates to access their own statistics.

The affiliate program tool is located in the "Referrers" page, under the "Stats" menu. Once you have installed the "Tracking - Front office" module, these affiliates can access their statistics by going to [http://www.example.com/modules/trackingfront/stats.php](http://www.example.com/modules/trackingfront/stats.php).

To create a new affiliate, click the "Add new" button, and in the creation form, add the affiliate account username and password, then specify the fee they receive per click, per order and per percentage of sales.

Click on the header of the "Help" section to display instructions on how to set up the referrer URLs.

The "Technical information - Expert mode" enables you to use regular expression instead of plain text URLs.

## UPS <a href="#verzending-enlogistiekmodules-ups" id="verzending-enlogistiekmodules-ups"></a>

Biedt uw klanten verschillende bezorgmethoden aan met behulp van UPS.

## USPS <a href="#verzending-enlogistiekmodules-usps" id="verzending-enlogistiekmodules-usps"></a>

**Alleen voor de Verenigde Staten.**

Calculates shipping rates for United States Postal Service for Domestic shipping within the USA
