# Administratiemodules

/\*\<!\[CDATA\[\*/\
div.rbtoc1597237794030 {padding: 0px;}\
div.rbtoc1597237794030 ul {list-style: disc;margin-left: 0px;}\
div.rbtoc1597237794030 li {margin-left: 0px;padding-left: 0px;}\
\
/\*]]>\*/

* [Administratiemodules](administratiemodules.md#Administratiemodules-Administratiemodules)
  * [1-Click Upgrade - AutoUpgrade](administratiemodules.md#Administratiemodules-1-ClickUpgrade-AutoUpgrade)
  * [Geavanceerde naleving van EU-regels](administratiemodules.md#Administratiemodules-GeavanceerdenalevingvanEU-regels)
    * [Labelopties](administratiemodules.md#Administratiemodules-Labelopties)
    * [Functies](administratiemodules.md#Administratiemodules-Functies)
    * [Juridische content management](administratiemodules.md#Administratiemodules-Juridischecontentmanagement)
    * [Extra e-mailcontent ](administratiemodules.md#Administratiemodules-Extrae-mailcontent)
  * [Cron taakmanager](administratiemodules.md#Administratiemodules-Crontaakmanager)
  * [CSV export voor nieuwsbrief](administratiemodules.md#Administratiemodules-CSVexportvoornieuwsbrief)
    * [Exporteer klanten](administratiemodules.md#Administratiemodules-Exporteerklanten)
  * [PrestaShop Opschoner](administratiemodules.md#Administratiemodules-PrestaShopOpschoner)
  * [E-mail notificaties](administratiemodules.md#Administratiemodules-E-mailnotificaties)
    * [Klantnotificaties](administratiemodules.md#Administratiemodules-Klantnotificaties)
    * [Notificaties voor winkeliers](administratiemodules.md#Administratiemodules-Notificatiesvoorwinkeliers)
  * [Google Analytics API](administratiemodules.md#Administratiemodules-GoogleAnalyticsAPI)
  * [Watermerk](administratiemodules.md#Administratiemodules-Watermerk)
  * [Verkoopervaring](administratiemodules.md#Administratiemodules-Verkoopervaring)
  * [NVD3 Charts](administratiemodules.md#Administratiemodules-NVD3Charts)
  * [Instappen](administratiemodules.md#Administratiemodules-Instappen)
  * [Eenvoudige HTML tabel weergave](administratiemodules.md#Administratiemodules-EenvoudigeHTMLtabelweergave)

## 1-Click Upgrade - AutoUpgrade <a href="#administratiemodules-1-clickupgrade-autoupgrade" id="administratiemodules-1-clickupgrade-autoupgrade"></a>

Deze module maakt het erg eenvoudig om PrestaShop bij te werken tot de laatste versie.

Bekijk het hoofdstuk [Automatisch bijwerken](../../prestashop-bijwerken/automatisch-bijwerken.md) om meer over deze module te weten te komen.

## Geavanceerde naleving van EU-regels <a href="#administratiemodules-geavanceerdenalevingvaneu-regels" id="administratiemodules-geavanceerdenalevingvaneu-regels"></a>

_Nieuw in PrestaShop 1.6.1.0._

De module "Geavanceerde naleving van EU-regels" helpt winkeliers bij het naleven van recente EU-wetten.

Deze module is noodzakelijk voor Europese winkels.

De meeste opties zijn bedoeld om meer transparantie te bieden aan klanten, met:

* Meer gedetailleerde prijslabels ("Van"-prijs, belasting, verzendkosten en levertijd, productgewicht, etc.)
* Geavanceerde afrekenpagina
* Juridische content toevoegen aan e-mails

Niet alle opties zullen even nuttig zijn in alle landen, maar ze helpen uw winkel wel bij het voldoen aan e-commercewetten van de EU.\
De standaardinstellingen zijn de aanbevolen instellingen; u bent vrij om opties in- of uit te schakelen.

### Labelopties <a href="#administratiemodules-labelopties" id="administratiemodules-labelopties"></a>

Zorg ervoor dat u alle tekstvelden vertaald in de beschikbare talen.

* **Label voor geschatte levertijd (producten op voorraad)**. Geeft de geschatte levertijd aan voor producten die op voorraad zijn. Laat dit veld leeg om de optie uit te schakelen. De standaardtekst is "Levertijd: 1 tot 3 weken".
* **Label voor geschatte levertijd (producten niet op voorraad)**. Geeft de geschatte levertijd aan voor producten die niet op voorraad zijn. Laat dit veld leeg om de optie uit te schakelen. De standaardtekst is "Levertijd: 3 tot 6 weken".
* **'Van' Basisprijs-label**. Als een product in de aanbieding is dan wordt de basisprijs getoond met het label 'Van' erbij.
* **'Incl./excl. btw label**. Toont of er belasting wordt toegepast naast de productprijs.
* **'Incl./excl. verzendkosten' -label**. Toont of de verzendkosten zijn toegevoegd, naast de productprijs.\
  Zodra u dit hebt ingeschakeld, moet u ervoor zorgen dat de optie "Verzending en betaling", in de sectie "Juridische content management", naar een CMS-pagina leidt. De label linkt naar deze content.
* **Productgewicht-label**. Toont het gewicht van het product (als de informatie beschikbaar is en het product meer dan 1kg weegt).
* **Aantal decimalen voor het productgewicht**. Helpt u om de nauwkeurigheid van de gewichtweergave in te stellen (bijv. 1kg / 1.01kg). De waarde kan niet negatief zijn.
* **Herroepingsrecht bevindt zich in de Algemene voorwaarden**. De inhoud van de CMS-pagina "herroepingsrecht" wordt toegevoegd aan de algemene voorwaarden.\
  Wanneer u dit inschakelt, zorgt u er dan voor dat de opties "Herroepingsrecht" is gekoppeld met een CMS-pagina, in de sectie "Juridische content management", onderin het configuratiescherm. Het label linkt dan naar deze content.
* **Herroepingsrecht voor virtuele producten**. Voegt een verplichte checkbox toe als de winkelwagen een virtueel product bevat. Gebruik deze om ervoor te zorgen dat klanten zich bewust worden van het feit dat een virtueel product niet geretourneerd kan worden.
* **'Van' prijslabel (in geval van combinaties)**. Toont een 'Van'-label voor de prijs bij producten met combinaties. Omdat prijzen de prijzen tussen combinaties kunnen verschillen, geeft dit label aan dat de prijs hoger kan zijn.
* **Bovenste tekst van de winkelwagen**. Voeg een aangepaste tekst toe aan het winkelwagenoverzicht.
* **Lagere winkelwagentekst**. Voeg een aangepaste tekst toe aan de onderkant van het winkelwagenoverzicht.

### Functies <a href="#administratiemodules-functies" id="administratiemodules-functies"></a>

* **Activeer 'vertel een vriend'**. Als dit is ingeschakeld, dan is de module 'Informeer een vriend' toegestaan op uw productpagina.\
  Deze optie zorgt ervoor dat u aan lokale wetgeving kunt voldoen: de e-mails die door deze functie worden verzonden kunnen worden beschouwd als ongewenste commerciële e-mails.
* **Activeer 'Opnieuw bestellen'-functie**. Als dit is ingeschakeld, dan staat de optie 'Opnieuw bestellen' toe dat klanten hun bestelling met één klik opnieuw kunnen bestellen vanaf hun bestelgeschiedenisoverzicht.\
  Deze optie zorgt ervoor dat u aan lokale wetgeving kunt voldoen: de producten die opnieuw worden besteld kunnen worden beschouwd als ongewenste goederen (vanwege herhaling).
* **'Geavanceerde afrekenpagina' inschakelen**. Vervangt het standaard afrekenproces met een versie die zich aan EU-regelgeving houdt. Deze optie werkt alleen goed met het standaard bootstrap-template of een ander thema dat is aangepast aan deze functie. Ook moeten betaalmodules deze nieuwe afrekenpagina ondersteunen.\
  Zodra dit is ingeschakeld, dan toont de geavanceerde afrekenpagina de volgende secties: betaalmethoden, adresoverzicht, algemene voorwaarden, winkelwagenoverzicht een een knop "Bestellen met betaalplicht".
* **Gemiddelde btw voor verzending en verpakking**. In plaats van een belastingregel toepassen op vervoerders en cadeauverpakking, kan het gemiddelde belastingspercentage van de producten in de winkelwagen gebruikt worden om toe te passen om cadeauverpakking en verzendkosten. Dit is erg nuttig in Duitsland.\
  Zodra u dit hebt ingeschakeld, wordt belasting voor verzending en verpakkingskosten berekend aan de hand van de belasting op de producten in de winkelwagen.\
  Dit betekent dat de klant een prijs met btw te zien krijgt voorafgaand aan het afrekenen en de verzending- en verpakkingsbelastingen berekend worden tijdens het afrekenproces.

### Juridische content management <a href="#administratiemodules-juridischecontentmanagement" id="administratiemodules-juridischecontentmanagement"></a>

Verschillende opties in deze module moeten weten naar welke CMS-pagina's gelinkt kan worden. Als er geen pagina beschikbaar is, dan moet u deze nog aanmaken.

### Extra e-mailcontent  <a href="#administratiemodules-extrae-mailcontent" id="administratiemodules-extrae-mailcontent"></a>

Met deze interface kunt u kiezen welke documenten u aan de onderkant van de standaarde-mails wilt toevoegen die verzonden worden door de winkel – bijvoorbeeld de inhoud van de algemene voorwaarden kan aan de onderkant van alle facturen worden toegevoegd.

De content kan worden ingesteld in de sectie "Juridische content management". Als er een optie niet is ingesteld, dan kunt u hier geen content kiezen om te verzenden.

## Cron taakmanager <a href="#administratiemodules-crontaakmanager" id="administratiemodules-crontaakmanager"></a>

Deze module geeft u het gereedschap om met crontaken te werken: u kunt taken aanmaken die een gegeven URL, specifiek voor uw PrestaShop-winkel, aanroepen en hiermee dus updates en andere geautomatiseerde taken starten.

## CSV export voor nieuwsbrief <a href="#administratiemodules-csvexportvoornieuwsbrief" id="administratiemodules-csvexportvoornieuwsbrief"></a>

Deze module is gebouwd om een CSV-bestand te maken van de e-mailadressen van de klanten die geregistreerd zijn voor de nieuwsbrief.

Uw klanten kunnen hun e-mailadres opgeven in het nieuwsbriefblok op de homepage door hun e-mail in te voeren. U hebt deze e-mailadressen nodig voor marketing.\
Bij het registreren kunnen klanten twee opties instellen met betrekking tot marketing: de eerste optie is inschrijven voor de nieuwsbrief, de tweede is aanbiedingen ontvangen van uw partners (opt-in).

### Exporteer klanten <a href="#administratiemodules-exporteerklanten" id="administratiemodules-exporteerklanten"></a>

Deze sectie maakt het mogelijk om de adressen van uw klanten te filteren voor dat u een CSV-bestand exporteert. Filteren op land is bijvoorbeeld heel handig als u nieuwsbrieven wilt verzenden in de juiste taal.

U kunt meer informatie invoeren bij het exporteren van e-mailadressen. Gebruik de selector "Nieuwsbrief abonnees" om één van de drie volgende items te selecteren:

* **Alle abonnees**. Hiermee kunt u alle e-mailadressen exporteren van gebruikers die zich hebben geregistreerd voor de nieuwsbrief, ongeacht of ze klant zijn of niet.
* **Geregistreerde abonnees**. Hiermee kunt u e-mailadressen exporteren van gebruikers die klant zijn en zich hebben geregistreerd voor nieuwsbrief.
* **Niet geregistreerde abonnees**. Hiermee kunt u e-mailadressen exporteren van gebruikers die geen klant, maar zich wel hebben aangemeld voor de nieuwsbrief.
* **Geen abonnees**. Hiermee worden gebruikers en/of klanten geselecteerd die zich niet hebben geregistreerd voor de nieuwsbrief. Wees hier voorzichtig mee.

De volgende selector heet "Reclame abonnees", waar u contacten kunt filteren op hun interesse om aanbiedingen van partners te ontvangen. Er zijn vier keuzes beschikbaar:

* **Alle klanten**. Maakt het mogelijk om alle e-mailadressen van alle klanten te selecteren. Dit zijn zowel gebruikers met een opt-in als zonder.
* **Abonnees**. Maakt het mogelijk om alleen de klanten met een opt-in te selecteren.
* **Geen abonnees**. Maakt het mogelijk om alleen klanten te selecteren zonder opt-in.

Zodra u de e-mailadressen hebt gefilterd, klikt u op de knop "Exporteer .CSV bestand" om de adressen te downloaden. Het bestand bevat zes typen informatie: de klant, ID, achternaam, voornaam, e-mailadressen, IP-adressen en registratiedatum. U kunt deze informatie gebruiken voor uw marketingcampagnes.

## PrestaShop Opschoner <a href="#administratiemodules-prestashopopschoner" id="administratiemodules-prestashopopschoner"></a>

Deze module is erg nuttig als u PrestaShop voor de eerste keer gebruikt en u klaar bent om uw eigen gegevens toe te voegen: u moet eerst de demonstratiedata verwijderen dat bij de installatie van PrestaShop mee is geïnstalleerd: producten, categorieën, klanten, bestellingen, etc.

De configuratiepagina heeft drie secties:

* **Catalogus**. Dit zal de gegevens van de huidige catalogus verwijderen, zelfs de items die u zelf hebt toegevoegd. Vink de box aan en klik op de knop "Verwijder de catalogus" om het proces te starten.
* **Bestellingen en klanten**. Dit zal alle bestellingen en klanten verwijderen, zelfs degene die u zelf hebt aangemaakt. Vink de box aan klik op de knop "Verwijder bestellingen en klanten" om het proces te starten.
* **Functionele integriteitsbeperkingen**. Dit controleert uw database en zorgt ervoor dat alles goed is ingesteld, en zal proberen om reparaties uit te voeren.
* **Database schoonmaken**. Zorgt ervoor dat er minder schijfruimte wordt gebruikt.

**Wees erg voorzichtig**: alle acties op deze pagina zijn onomkeerbaar. Zorg ervoor dat u eerst een reservekopie aanmaakt van uw gegevens.

## E-mail notificaties <a href="#administratiemodules-e-mailnotificaties" id="administratiemodules-e-mailnotificaties"></a>

PrestaShop kan u en uw klanten notificaties sturen in sommige gevallen:

* Uw klanten: als een product niet meer op voorraad is.
* U : als er een nieuwe bestelling is geplaatst.
* U: als de voorraad onder een bepaald niveau is.
* U: als de voorraaddekking van een product te laag is.

### Klantnotificaties <a href="#administratiemodules-klantnotificaties" id="administratiemodules-klantnotificaties"></a>

Er is slechts één optie in deze sectie:

* **Product beschikbaarheid**. Als u deze instelling activeert verschijnt er een veld op de productpagina van uw winkel als het product niet meer op voorraad is. Het vraagt uw klanten om hun contactinformatie achter te laten, zodat ze een e-mail ontvangen als het product weer op voorraad is.

### Notificaties voor winkeliers <a href="#administratiemodules-notificatiesvoorwinkeliers" id="administratiemodules-notificatiesvoorwinkeliers"></a>

Er zijn een aantal instellingen voor winkeliers:

* **Nieuwe bestelling**. Schakel deze optie in als u meldingen wilt ontvangen over elke nieuwe bestelling.
* **Niet op voorraad**. Schakel deze optie en de drempel in met de waarde wanneer u een melding wilt ontvangen (3 is standaard).
* **Dekkingswaarsshuwing**. Schakel deze optie in en kies de dekkingswaarde wanneer u een melding wilt ontvangen (0 is standaard).

Notificaties voor winkeliers kunnen naar meerdere e-mailadressen tegelijkertijd worden verzonden. Om dit te doen voert u de e-mailadressen in (een e-mailadres per regel).

## Google Analytics API <a href="#administratiemodules-googleanalyticsapi" id="administratiemodules-googleanalyticsapi"></a>

Deze module maakt het mogelijk om uw PrestaShop-winkel te verbinden met uw Google Analytics-account.

U moet eerst de API-versie kiezen:

* Versie 1.3 vereist dat u uw e-mail, wachtwoord en profiel van Google Analytics invoert.
* Versie 3.0 vereist dat u uw Google Analytics Client ID, Client Secret en profiel invoert.

We raden versie 3.0 aan, omdat versie 1.3 achterhaald is. Om versie 3.0 aan de praat te krijgen, moet u eerst Oath-toegang inschakelen door deze instructies te volgen: [https://developers.google.com/analytics/devguides/config/mgmt/v3/mgmtAuthorization](https://developers.google.com/analytics/devguides/config/mgmt/v3/mgmtAuthorization)

## Watermerk <a href="#administratiemodules-watermerk" id="administratiemodules-watermerk"></a>

Deze module maakt het mogelijk om een watermerk aan alle productafbeeldingen in uw winkel toe te voegen. Dit limiteert de verspreiding op het internet – en voorkomt hopelijk dat mensen de afbeeldingen gaan stelen.

Als u uw producten wilt exporteren naar Google Shopping, dan moet u weten dat het gebruik van promotionele teksten, logo's en watermerken in de afbeeldingen niet is toegestaan. U mag alleen afbeeldingen uploaden die vrij zijn van watermerken / logo's.\
Hier vindt u meer over de Google Shopping policy: [https://support.google.com/merchants/answer/2700371?hl=nl\&ref\_topic=2701481](https://support.google.com/merchants/answer/2700371?hl=nl\&ref\_topic=2701481)

De configuratiepagina toont meteen enkele meldingen van de instellingen die momenteel ontbreken.

* **Watermerk bestand**. De gekozen afbeelding moet in GIF-formaat zijn.
* **Watermerk ondoorzichtigheid (0-100)**. 100 betekent een ondoorzichtige afbeeldingen, dit maakt uw afbeeldingen erg duidelijk, maar het verbergt ook delen van uw afbeeldingen. De standaardinstelling is 60. Dit is een goede balans.
* **Watermerk X-uitlijning**. Kies waar uw watermerk zou moeten verschijnen op elke afbeelding, hier op de horizontale as.
* **Watermerk Y-uitlijning**. Kies waar uw watermerk zou moeten verschijnen op elke afbeelding, hier op de verticale as.
* **Kies de afbeeldingstype's die u met een watermerk wilt beschermen**. De afbeeldingstypes waar de watermerk wordt toegevoegd. U hoeft waarschijnlijk alleen de grootste afbeeldingen te kiezen. Deze worden het meeste gestolen.

Zodra u de instellingen hebt opgeslagen, is de configuratie voltooid, maar zijn de watermerken nog niet toegevoegd aan de afbeeldingen. Ga naar de pagina "Afbeeldingen" onder het menu "Instellingen". Daar klikt u op de knop "Miniaturen hergenerern" aan de onderkant van de pagina. PrestaShop verwerkt al uw afbeeldingen (zoals geselecteerd in de configuratie) en uw watermerk zal, op alle afbeeldingen die u hebt geselecteerd, verschijnen.

## Verkoopervaring <a href="#administratiemodules-verkoopervaring" id="administratiemodules-verkoopervaring"></a>

Deze module is ontworpen voor PrestaShop-gebruikers om hun voortgang als e-winkelier bij te houden. Hiermee kunnen ze zien hoeveel voortgang ze hebben geboekt over de dagen, maanden en jaren. Het is standaard geïnstalleerd.

De module voegt een systeem toe met badges en punten, onderverdeeld in drie niveaus, allemaal belangrijk om succes te boeken.

* **Functies**. Dit houdt uw gebruik van functies binnen PrestaShop bij, zoals Prestaties, grootte van catalgous, medewerkers en SEO.
* **Prestaties**. Dit toont de voortgang bij op het gebied van aantal klanten, bestellingen en omzet.
* **Internationaal**. Houdt bij of u internationaal veel bestellingen krijg in markten zoals die van Amerika, Oceanië, Azië, Europa, Afrika en Maghhreb.

Des te meer voortgang u boek, hoe meer badges en punten u verdient.\
U hoeft geen informatie te verstrekken of alle formulieren in te vullen, we weten hoe druk u bent, alles is automatisch!

## NVD3 Charts <a href="#administratiemodules-nvd3charts" id="administratiemodules-nvd3charts"></a>

NVD3 ([http://nvd3.org/](http://nvd3.org/)) is een JavaScript-bibliotheek, bedoeld om prachtige grafieken te tonen door middel van D3.js, een JavaScript-bibliotheek om documenten aan te passen aan de hand van gegevens.

Deze module maakt NVD3 code beschikbaar voor eigen gebruik.

## Instappen <a href="#administratiemodules-instappen" id="administratiemodules-instappen"></a>

De module Instappen begroet gebruikers die voor de eerste keer de backoffice gebruiken: met een speelse interface wordt getoond hoe gebruikers hun winkel in enkele stappen kunnen lanceren.

## Eenvoudige HTML tabel weergave <a href="#administratiemodules-eenvoudigehtmltabelweergave" id="administratiemodules-eenvoudigehtmltabelweergave"></a>

Maakt het mogelijk voor het statistieksysteem om de gegevens in een tabel weer te geven.
