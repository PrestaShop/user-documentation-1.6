# Algemene concepten

## Algemene concepten <a href="#algemeneconcepten-algemeneconcepten" id="algemeneconcepten-algemeneconcepten"></a>

Om verwarring te voorkomen met het klassieke voorraadbeheer-systeem in PrestaShop versie 1.4 en om de mogelijkheden te zien die geboden worden door het geavanceerd voorraadbeheersysteem in versie 1.5, moet u twee concepten van elkaar onderscheiden: producthoeveelheid dat beschikbaar is voor verkoop en de fysieke hoeveelheid producten.

### Producten beschikbaar voor verkoop <a href="#algemeneconcepten-productenbeschikbaarvoorverkoop" id="algemeneconcepten-productenbeschikbaarvoorverkoop"></a>

Dit is hetzelfde als het voorraadsysteem van PrestaShop 1.4.x. Het is de producthoeveelheid die in de winkel wordt getoond voor elk product en combinatie. Dit is de hoeveelheid die aangeeft hoeveel producten besteld kunnen worden (tenzij de optie "Sta het bestellen van producten toe die niet op voorraad zijn" is ingeschakeld). Deze hoeveelheid kan handmatig worden bijgewerkt voor elk producten en combinatie.

Sinds PrestaShop 1.5.x kan deze hoeveelheid automatisch worden gezet aan de hand van de fysieke voorraad van het product. In een multistore-omgeving kan de hoeveelheid ingesteld worden voor elke winkel.

Bijgevolg is dat wat "voorraad" wordt genoemd in PrestaShop 1.4.x, sinds PrestaShop 1.5.x gelijk aan "hoeveelheid beschikbaar voor verkoop".

### Productvoorraad (fysieke voorraad) <a href="#algemeneconcepten-productvoorraad-fysiekevoorraad" id="algemeneconcepten-productvoorraad-fysiekevoorraad"></a>

Dit is het beheer van de fysieke producten in een magazijn (of meerdere). Dit is het nieuwe concept dat is geïntroduceerd als "voorraad" in PrestaShop 1.5.x.

Dit nieuwe voorraadbeheersysteem bevat voorraadverplaatsing, voorraaddekking, voorraadverplaatsing tussen magazijnen, integratie met de multistore-mogelijkheid en leveranciersbestellingen.

Het wordt ook mogelijk gemaakt om de actuele voorraad bij te houden. Op een gegeven moment kan een product nog steeds beschikbaar zijn vanwege de fysieke voorraad, maar niet langer beschikbaar voor verkoop, omdat sommige bestellingen nog steeds verzonden moeten worden. Ook kan er voor hetzelfde product een bestelling zijn geplaatst bij de leverancier en dus nog niet beschikbaar in de fysieke voorraad.

De daadwerkelijke voorraad bestaat daarom uit de voorraad die beschikbaar is in het magazijn, waar de de hoeveelheid van leveranciersbestellingen bij optellen en waar we de verkochte voorraad weer van aftrekken.

## Het nieuwe voorraadsysteem gebruiken <a href="#algemeneconcepten-hetnieuwevoorraadsysteemgebruiken" id="algemeneconcepten-hetnieuwevoorraadsysteemgebruiken"></a>

### Moet ik het nieuwe systeem gebruiken? <a href="#algemeneconcepten-moetikhetnieuwesysteemgebruiken" id="algemeneconcepten-moetikhetnieuwesysteemgebruiken"></a>

Er is geen verplichting om het nieuwe voorraadsysteem te gebruiken, net zoals er geen verplichting bestaat om de functie "beschikbare hoeveelheid voor verkoop" te gebruiken.

Om zowel de "beschikbare hoeveelheid voor verkoop" als het gewone voorraadbeheer te activeren gaat u naar de configuratiepagina "Producten" onder het menu "Instellingen", scrolt u omlaag naar de sectie "Producten voorraad" en kiest u "Ja" bij beide voorraadbeheeropties. U moet eerst het basisvoorraadbeheersysteem activeren voordat u de uitgebreide variant kunt inschakelen.

Het geavanceerde voorraadsysteem of zelfs het basissysteem en uw magazijnen zijn onafhankelijk van de multistore-mogelijkheid. Als gevolg daarvan maakt het niet uit voor welke winkel u de instellingen configureert in de PrestaShop backoffice wanneer u gebruik maakt van voorraadbeheer. Ook kunt u nog altijd de instellingen wijzigen in de "globale" context.

### Ik wil niets veranderen aan mijn instellingen in PrestaShop 1.4/1.5. Wat moet ik doen? <a href="#algemeneconcepten-ikwilnietsveranderenaanmijninstellingeninprestashop1.4-1.5.watmoetikdoen" id="algemeneconcepten-ikwilnietsveranderenaanmijninstellingeninprestashop1.4-1.5.watmoetikdoen"></a>

Als u liever niet het geavanceerde voorraadbeheersysteem van PrestaShop 1.5 en 1.6 gebruikt, maar tevreden bent met de "klassieke" manier, dan hoeft u enkel de oude manier te activeren en niet de geavanceerde variant: ga naar de pagina "Producten" onder het menu "Instellingen" en kies "Ja" bij de optie "Schakel voorraadbeheer in" en "Nee" bij de optie "Schakel geavanceerd voorraadbeheer in".

De functie "beschikbare hoeveelheid voor verkoop" is nu gecentraliseerd op het tabblad "Aantal" van de productconfiguratiepagina: maak een nieuw product aan of bewerk een huidige, en het tabblad aantal verschijnt aan de linkerkant van de pagina.

### Is het nieuwe voorraadbeheersysteem geschikt voor mij? <a href="#algemeneconcepten-ishetnieuwevoorraadbeheersysteemgeschiktvoormij" id="algemeneconcepten-ishetnieuwevoorraadbeheersysteemgeschiktvoormij"></a>

Het nieuwe voorraadsysteem maakt het mogelijk voor u om de voorraad van producten bij te houden. Deze feature is handig voor uw bedrijf als:

* U een voorraad bij moet houden van producten die u in uw winkel verkoopt.
* U minstens één magazijn gebruikt die u zelf in beheer heeft.
* U bestelt uw producten bij minstens één leverancier.
* U hebt statistieken nodig van uw voorraadstatus en uw magazijn(en).

Deze feature is niet geschikt voor u wanneer:

* U uw producten niet zelf beheert.
* U al een beheersysteem in gebruik hebt waarmee u tevreden bent, en die u liever blijft gebruiken zonder iets te veranderen.
