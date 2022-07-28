# PrestaShop bijwerken

**Inhoudsopgave**

* [PrestaShop bijwerken](./#PrestaShopbijwerken-PrestaShopbijwerken)
  * [Backups en problemen](./#PrestaShopbijwerken-Backupsenproblemen)
  * [PrestaShop ondersteuning](./#PrestaShopbijwerken-PrestaShopondersteuning)
  * [Controleer de vereisten van de nieuwe versie](./#PrestaShopbijwerken-Controleerdevereistenvandenieuweversie)
  * [Voor degenene die upgraden vanaf een versie lager dan 1.4.x](./#PrestaShopbijwerken-Voordegenenedieupgradenvanafeenversielagerdan1.4.x)

## PrestaShop bijwerken <a href="#prestashopbijwerken-prestashopbijwerken" id="prestashopbijwerken-prestashopbijwerken"></a>

Nieuwe versies van PrestaShop verschijnen bijna elke maand. Soms zit er slechts een week tussen nieuwe versies. Sommige updates bevatten grote veranderingen, andere weer kleine veranderingen. Een nieuwe update zit in ieder geval boordevol innovaties, verbeteringen en bug-fixes. Er wordt daarom sterk aangeraden om te bijwerken naar de meest recente versie.

Er zijn twee manieren op PrestaShop bij te werken:

* [Automatisch](automatisch-bijwerken.md)
* [Handmatig](handmatig-bijwerken.md)

De automatische update wordt uitgevoerd door middel van de gratis [1-Click Upgrade module](http://addons.prestashop.com/nl/modules-beheertools/5496-1-click-upgrade-autoupgrade.html).

De handmatige methode wordt niet langer ondersteund, maar de documentatie is nog steeds beschikbaar als archief - en voor degenen waarbij het automatisch upgraden niet lukt.

Het updateproces zal alle basisbestanden overschrijven in de PrestaShop-map. Dit zijn de hoofdbestanden op PrestaShop te kunnen draaien, alle standaardmodules en standaarthema. Als u één van deze bestanden hebt aangepast, dan raakt u uw veranderingen kwijt. (Dit geldt niet voor bestanden in de `override` map).

Als het updateproces op de juiste manier wordt uitgevoerd, dan duurt het in totaal niet langer dan een half uur. Probeer geen stap over te slaan om zo tijd te besparen, alle stappen zijn cruciaal.

### Backups en problemen <a href="#prestashopbijwerken-backupsenproblemen" id="prestashopbijwerken-backupsenproblemen"></a>

Als er iets misgaat bij het updaten, dan gaat u naar [Backups aanmaken en terugzetten](backups-aanmaken-en-terugzetten.md).

Als u hulp nodig hebt bij overige problemen dan [heeft u deze pagina nodig](wanneer-er-problemen-optreden.md).  &#x20;

### PrestaShop ondersteuning <a href="#prestashopbijwerken-prestashopondersteuning" id="prestashopbijwerken-prestashopondersteuning"></a>

Voor een **hulpverzoek** of **hulp bij het opzetten van uw website**, kunt u contact met ons opnemen om onze supportopties te verkennen.

Ons support team is beschikbaar voor al uw technische problemen gerelateerd aan het updaten van uw PrestaShop-winkel:

* Via e-mail: gebruik het contactformulier op [https://www.prestashop.com/nl/support](https://www.prestashop.com/nl/support)
* Telefonisch: +33.1 40 18 30 04 (9:00 – 18:00 Midden-Europese Tijdzone \[CET])
* Kom meer te weten over onze supportopties: [http://support.prestashop.com](http://support.prestashop.com/)
* En de altijd zeer behulpzame community: [community forums](http://www.prestashop.com/forums/)

### Controleer de vereisten van de nieuwe versie <a href="#prestashopbijwerken-controleerdevereistenvandenieuweversie" id="prestashopbijwerken-controleerdevereistenvandenieuweversie"></a>

Voordat u iets veranderd aan uw PrestaShop-installatie, controleert u dan of uw serverconfiguratie gelijk is aan of hoger dan de minimale vereisten voor de meest recente versie van PrestaShop. Deze zijn terug te vinden op deze pagina: [https://www.prestashop.com/nl/systeem-vereisten](https://www.prestashop.com/nl/systeem-vereisten).\
Voorbeeld: zorg ervoor dat uw hostingprovider u kan voorzien in de vereiste versies van PHP en MySQL. Zo niet, vraag uw host dan om uw serverconfiguratie te verbeteren. Wanneer u niet zeker weet welke versies van PHP en MySQL zijn geïnstalleerd, vraag dan uw hostingprovider om hulp.&#x20;

Als uw hostingprovider uw serverconfiguratie niet kan wbijwerken, dan is het tijd om een betere host te vinden! Voor een update NIET uit, tenzij u kunt voldoen aan de minimumvereisten.

### Voor degenene die upgraden vanaf een versie lager dan 1.4.x <a href="#prestashopbijwerken-voordegenenedieupgradenvanafeenversielagerdan1.4.x" id="prestashopbijwerken-voordegenenedieupgradenvanafeenversielagerdan1.4.x"></a>

Het is lastiger om oudere versies van PrestaShop te updaten naar de meest recente versie: de codebasis verschilt enorm, veel bestanden bevinden zich op een andere plek, velen zijn erbij gekomen sindsdien en anderen weer verwijderd. Daarom, is de kans groot, dat bij het overslaan van een oude versie naar een nieuwere er veel problemen ontstaan.

U kunt ook geen automatische upgrade uitvoeren en zit vast aan het [handmatige updateproces](handmatig-bijwerken.md): de 1-Click upgrade module werkt alleen met versie 1.4 en hoger.

U moet daarom nóg voorzichtiger te werk gaan. Hoe ouder de versie, hoe meer aandacht u moet schenken aan details als: backups, aangepaste bestanden, bewerkte thema's, etc...
