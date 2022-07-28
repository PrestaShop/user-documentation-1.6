# Benodigdheden

**Inhoudsopgave**

/\*\<!\[CDATA\[\*/\
div.rbtoc1597237782240 {padding: 0px;}\
div.rbtoc1597237782240 ul {list-style: disc;margin-left: 0px;}\
div.rbtoc1597237782240 li {margin-left: 0px;padding-left: 0px;}\
\
/\*]]>\*/

* [Benodigdheden](benodigdheden.md#Benodigdheden-Benodigdheden)
  * [Snel aan de slag](benodigdheden.md#Benodigdheden-Snelaandeslag)
  * [Gedetailleerde setup-instructies](benodigdheden.md#Benodigdheden-Gedetailleerdesetup-instructies)
    * [Domeinnaam registreren](benodigdheden.md#Benodigdheden-Domeinnaamregistreren)
    * [Een hostingprovider zoeken](benodigdheden.md#Benodigdheden-Eenhostingproviderzoeken)
    * [Technische vereisten](benodigdheden.md#Benodigdheden-Technischevereisten)
    * [Gereedschap](benodigdheden.md#Benodigdheden-Gereedschap)
    * [Een plan opstellen](benodigdheden.md#Benodigdheden-Eenplanopstellen)
    * [PrestaShop installeren](benodigdheden.md#Benodigdheden-PrestaShopinstalleren)

## Benodigdheden <a href="#benodigdheden-benodigdheden" id="benodigdheden-benodigdheden"></a>

### Snel aan de slag <a href="#benodigdheden-snelaandeslag" id="benodigdheden-snelaandeslag"></a>

Hier is een korte lijst met benodigdheden om aan de slag te kunnen gaan met de installatie van PrestaShop 1.6. Mocht u niet genoeg hebben aan deze beknoptie instructies, dan kunt u in de volgende hoofdstukken uitgebreidere informatie vinden.

* Systeemvereisten:
  * PHP 5.4 of nieuwer.
    * Nuttige instellingen: `allow_url_fopen` instellen op On, `register_globals` instellen op Off, `magic_quotes_*` instellen op Off, `safe_mode` instellen op Off (allemaal te vinden in het bestand: `php.ini`), `file_max_upload_size` instellen op "16M".
    * Nuttige PHP-extensies: PDO\_MySQL, cURL, SimpleXML, mcrypt, GD, OpenSSL, DOM, SOAP.
    * Nuttige server-tools: cron/crontab, Memcached.
  * MySQL 5.0 of nieuwer.
  * Aangeraden: \

    * Unix/Linux hosting.
    * Apache Web Server 1.3 of nieuwer, of nginx Web Server.
      * Apache modul-instellingen: `mod_rewrite op` enabled, `mod_security` op disabled, `mod_auth_basic` op disabled.
    * Minstens 64 Mb aan RAM beschikbaar voor PHP.
* Toegangscodes voor FTP en uw MySQL database\

  * Deze worden door uw hostingprovider beschikbaar gesteld, mits u geen lokale installatie gebruikt.
* Een tekstverwerker.
* Een FTP client.
* Een moderne Web browser (in het geval van Internet Explorer: op zijn minst IE9).

U dient ook op de hoogte zijn van de URL waar de webwinkel te bereiken is.

Hier kunt u de officiële systeemvereisten bekijken: [https://www.prestashop.com/nl/systeem-vereisten](https://www.prestashop.com/nl/systeem-vereisten).

Zodra uw setup gereed is kunt u de intallatiehandleiding gebruiken: [http://doc.prestashop.com/display/PS16/PrestaShop+installeren](prestashop-installeren.md).

### Gedetailleerde setup-instructies <a href="#benodigdheden-gedetailleerdesetup-instructies" id="benodigdheden-gedetailleerdesetup-instructies"></a>

PrestaShop is een webapplicatie: het moet geïnstalleerd worden op een webserver, om te kunnen draaien, en heeft een domein nodig die uw klanten kunnen gebruiken om uw winkel te bzoeken.

#### Domeinnaam registreren <a href="#benodigdheden-domeinnaamregistreren" id="benodigdheden-domeinnaamregistreren"></a>

Voordat u PrestaShop downloadt of installeert, moet u zorgen voor een nieuw thuis voor PrestaShop. Dat bestaat uit twee componenten: een domeinnaam en een webserver. Een voorbeeld van een domeinnaam is [example.com](http://www.example.com) of [mijnonlinewinkel.nl](http://mijnonlinewinkel.nl). Dit is het 'gezicht' van uw webserver en daarom ook van uw winkel.

U moet een domeinnaam kopen voor uw winkel. Deze kunt u mogelijk tegelijk met uw hosting krijgen: veel hosting providers bieden een gratis domein aan bij elk account. Sommige zijn gratis voor een jaar, zolang u klant blijft van de betreffende hoster. Dit maakt het gemakkelijk om het gehele pakket (hosting+domeinnaam) ineen te bemachtigen.

Er kunnen problemen optreden met domeinnamen die aangeboden worden door hostingproviders. Als u niet tevreden bent met de service van een provider, dan kunt u ervoor kiezen om te verhuizen naar een betere host. Dit betekent dat u bestanden, data en domeinnaam moet verhuizen naar die andere provider.

De bestanden en andere data zijn gemakkelijk te verhuizen, maar afhankelijk van de hosting provider, kan het u erg lastig gemaakt worden om uw domeinnaam terug te krijgen. Omdat de domeinnaam door hen voor u is gekocht, behoort de domeinnaam, technisch gezien, tot hen. Zij kunnen u verbieden de domeinnaam te verhuizen naar een andere host of ze kunnen om een extra toeslag vragen. Zolang uw domeinnaam en merk online te vinden is via deze host, moet u de voorwaarden van de provider respecteren.

Dat is waarom in het algemeen wordt aangeraden om uw domeinnaam te kopen bij een onafhankelijke registrar (bekijk: [https://nl.wikipedia.org/wiki/Registrar](https://nl.wikipedia.org/wiki/Registrar)). Technisch gezien kunt u geen domeinnaam kopen; deze kunt u slechts huren, meestal voor de duur van een jaar. Dit geeft u het recht om de domeinnaam te gebruiken, maar zodra u stopt met betalen, is het niet meer uw eigendom en kan ieder ander deze domeinnaam overnemen. Dus, zolang u betaalt voor de registratie van de domeinnaam bij de onafhankelijke registrar en de kosten voor web hosting, bent u vrij om te verhuizen naar een betere host op elk moment, zonder dat het u extra kost: verander slechts het ip-adres dat bij de domeinnaam hoort en binnen 24 uur is de wijziging wereldwijd doorgevoerd.

Als u uw domeinnaam liever bij een onafhankelijke registrar koopt, dan zijn hier enkele betrouwbare registrars:

* Gandi: [http://en.gandi.net/](http://en.gandi.net/)
* Namecheap: [http://www.namecheap.com/](http://www.namecheap.com/)
* PairNIC: [https://www.pairnic.com/](https://www.pairnic.com/)

En er zijn er nog veel meer. Vraag bekenden om meer info!

#### Een hostingprovider zoeken <a href="#benodigdheden-eenhostingproviderzoeken" id="benodigdheden-eenhostingproviderzoeken"></a>

Nu dat u een domeinnaam heeft, moet u ervoor zorgen dat deze naar uw PrestaShop-installatie wijst. Dit betekent dat de bestanden op een webserver gezet moeten worden. U heeft wellicht een eigen webserver, maar de kans is groter dat u uw winkel laat hosten of gaat laten hosten bij een hostingprovider (zie: [https://nl.wikipedia.org/wiki/Hostingprovider](https://nl.wikipedia.org/wiki/Hostingprovider)). Deze biedt u een online thuis aan tegen een maandelijkse of jaarlijkse toeslag.

Voordat u met een webwinkel begint, moet u eerst een hostingprovider kiezen. Bij bijna elke webhost kan PrestaShop goed draaien. Echter, er zijn enkele hostingproviders met geoptimaliseerde servers voor PrestaShop:

* Combell in Nederland en België: [Combell](http://www.combell.com/nl/hosting/prestashop-webhosting)
* DataCT in Nederland: [DataCT](http://www.datact.nl/Software/Alle-software/Webshop/PrestaShop-Hosting.html)
* OVH in Frankrijk: [OVH](http://www.ovh.com/fr/solutions/prestashop/?pk\_campaign=partenariatprestashop\&pk\_kwd=pagefr)
* 1&1 in Spanje: [1&1](http://www.prestashop.com/es/ecommerce-hosting/1and1)
* InMotion Hosting in alle landen, behalve Frankrijk en Spanje: [InMotion](http://www.inmotionhosting.com/prestashop-hosting)

Bekijk onze [hosting partners](http://www.prestashop.com/en/ecommerce-hosting)!

Wanneer u een host uitkiest, vergeet dan niet deze cruciale eis: het moet ondersteuning bieden voor minstens PHP 5.4 (of nieuwer), de programmeertaal waarin PrestaShop is geschreven. MySQL 5.0 (of nieuwer), het databasesysteem waarin PrestaShop zijn data bewaart. Hiernaast zijn er nog enkele eisen: bekijk de sectie [Technische vereisten](benodigdheden.md#Benodigdheden-Technischevereisten) hieronder.

PrestaShop Cloud

PrestaShop kan uw winkel gratis hosten op zijn eigen servers. PrestaShop Cloud is opgericht om verkopers te bevrijden van technische complicaties, zoals het installeren en bijwerken van PrestaShop.

Bekijk onze PrestaShop Cloud website of meer te weten te komen over onze gratis en veilige hosting service. Deze service wordt sterk aangeraden voor bedrijven met weinig tot geen ervaring met internet en/of computers.

Meer informatie over PrestaShop Cloud is beschikbaar op dit adres: [https://www.prestashop.com/nl/aan-de-slag](https://www.prestashop.com/nl/aan-de-slag).

#### Technische vereisten <a href="#benodigdheden-technischevereisten" id="benodigdheden-technischevereisten"></a>

PrestaShop is een applicatie die op een webserver draait en is geschreven in de programmeertaal PHP. Het bewaart zijn data op een MySQL-server.

PHP is een open source programmeertaal, vooral gebruikt voor webapplicaties. Sinds de eerste versie, uit 1995, is het uitgegroeid tot één van de meest gebruikte programmeertalen door webontwikkelaars. Het gebruikt een C-achtige syntaxis, die het gemakkelijk maakt voor de meeste programmeurs om te leren.

MySQL is een open source database management systeem. De eerste versie hiervan stamt ook uit 1995, en is sindsdien het meest gebruikte databasesysteem door webdevelopers. Het is gebaseerd op de SQL-taal, de meeste gebruikte databasetaal.

Welke hosting service u ook kiest, het op zijn minst de volgende componenten bevatten:

* **Systeem**: Unix, Linux of Windows. Unix wordt sterk aangeraden.
* **Webserver**: Apache Web server 1.3 of nieuwer.
* **PHP 5.4 of nieuwer**. U moet mogelijk nog PHP 5 activeren (vraag uw hostingprovider om meer informatie).
* **MySQL 5.0 of nieuwer**.
* Minstens 64MB aan RAM op uw server (128MB wordt aangeraden, hoe meer hoe beter).

PrestaShop werkt ook met IIS Web server 6.0 of nieuwer, van Microsoft. Ook nginx versie 1.0 of nieuwer wordt ondersteund.

Meer informatie is beschikbaar voor systeembeheerder in de [System Administrators Guide](http://doc.prestashop.com/display/PS15/System+Administrator+Guide). Zorg ervoor dat u dit gelezen hebt!

#### Gereedschap <a href="#benodigdheden-gereedschap" id="benodigdheden-gereedschap"></a>

U heeft twee tools nodig: een tekstverwerker, om tekst- en/of configuratiebestanden te bewerken en een FTP-client, om bestanden up te loaden vanaf uw machine naar uw server en andersom.

**Tekstverwerker**

Hier zijn een aantal bekende tekstverwerkers:

* Windows:
  * Notepad++: [http://notepad-plus-plus.org/](http://notepad-plus-plus.org/)
  * UltraEdit: [http://www.ultraedit.com/](http://www.ultraedit.com/)
  * Crimson Editor: [http://www.crimsoneditor.com/](http://www.crimsoneditor.com/)
* OS X:
  * Textmate: [http://macromates.com/](http://macromates.com/)
  * Coda: [http://www.panic.com/coda/](http://www.panic.com/coda/)
  * Smultron: [http://www.peterborgapps.com/smultron/](http://www.peterborgapps.com/smultron/)
* Unix/Linux:
  * Vim: [http://www.vim.org/](http://www.vim.org/)
  * Emacs: [http://www.gnu.org/software/emacs/](http://www.gnu.org/software/emacs/)

Gebruik GEEN word processor wanneer u tekstbestanden aanpast zoals Microsoft Word of [OpenOffice](http://www.openoffice.org/)/[LibreOffice](https://www.libreoffice.org/) Write.

**FTP-client**

FTP is een afkorting voor "File Transfer Protocol". Dit komt neer op dé standaardmanier om bestanden te verplaatsen vanaf een computer naar een webhost.

In deze handleiding maken we gebruik van FileZilla, welke een goede en gratis FTP-client is voor zowel Windows, Mac OS X en Linux. Download het vanaf [http://filezilla-project.org/](http://filezilla-project.org/) en installeer deze. Let op: vermijdt FileZilla Server, installeer slechts FileZilla Client!

Zodra FileZilla is geïnstalleerd, moet u het configureren met de verbindingsinstellingen voor uw webserver, welke door uw hostingprovider geleverd moeten zijn. Als dat niet het geval is, vraag hen om deze gegeven - of bekijk uw spam folder.

In het algemeen zijn de volgende instellingen nodig:

* **een hostname** of **een IP-adres**: de locatie van uw FTP-server.
* **een gebruikersnaam**: uw accountnaam.
* **een wachtwoord**

Open FileZilla, en open de Site Manager tool. Deze kunt u op drie verschillende manieren openen:

* Druk op Ctrl-S,
* Klik op het "Open the Site Manager" icoon, linksboven,
* Klik op "File" en selecteer de "Site Manager..." optie.

Een nieuw venster opent.

Om uw hostingplek toe te voegen aan de Site Manager:

1. Klik op de "New Site" knop. Een nieuw item wordt aangemaakt in de websitelijst. Geef het een gemakkelijk te herkennen naam.&#x20;
2. Aan de rechterzijde, in het "General" tabblad, voer de instellingen in, zoals geleverd door uw hostingprovider. Dit zijn: host, user en pasword. U hoeft de andere instellingen niet te wijzigen, tenzij dit expliciet vermeld is door uw host.
3. Zodra de velden zijn ingevuld, klikt u op de "Connect" knop. Dit bewaart zowel uw site in de lijst en logt u automatisch in op uw account, zodat u gelijk zekerheid heeft of uw instellingen juist zijn.

Mocht FileZilla niet geschikt zijn voor u, dan zijn hier enkele alternatieven:

* Windows:
  * CoreFTP: [http://www.coreftp.com/](http://www.coreftp.com/)
  * WinSCP: [http://winscp.net/](http://winscp.net/)
  * SmartFTP: [http://www.smartftp.com/](http://www.smartftp.com/)
* Mac OS X:
  * Cyberduck: [http://cyberduck.ch/](http://cyberduck.ch/)
  * Transmit: [http://www.panic.com/transmit/](http://www.panic.com/transmit/)
  * Fetch: [http://fetchsoftworks.com/fetch/](http://fetchsoftworks.com/fetch/)
* Unix/Linux:
  * gFTP: [http://gftp.seul.org/](http://gftp.seul.org/)
  * kasablanca: [http://kasablanca.berlios.de/](http://kasablanca.berlios.de/)
  * NcFTP: [http://www.ncftp.com/ncftp/](http://www.ncftp.com/ncftp/)

#### Een plan opstellen <a href="#benodigdheden-eenplanopstellen" id="benodigdheden-eenplanopstellen"></a>

Voor nu is de eerste keuze die u moet maken, is hoe uw URL eruit gaat zien. Er zijn vier mogelijkheden met betrekking tot uw domeinnaam:

* In de 'root' van de domeinnaam: [http://www.example.com/](http://www.example.com/)
* In een map: [http://www.example.com/shop/](http://www.example.com/shop/)
* In een subdomein: [http://store.example.com/](http://store.example.com/)
* In en map van een subdomain: [http://clothes.example.com/boutique/](http://clothes.example.com/boutique/)

Let op: dankzij de multistore-mogelijkheid, kunt u zoveel winkels aanmaken als u nodig heeft, met slechts een enkele PrestaShop-installatie, elk met zijn eigen domeinnaam als dat nodig is. Houd daar rekening mee wanneer u gaat bepalen waar elke winkel komt.\
Wat uw plan ook mag zijn, de standaardwinkel zal zich altijd bevinden op de locatie waar PrestaShop zichzelf bevindt.&#x20;

#### PrestaShop installeren <a href="#benodigdheden-prestashopinstalleren" id="benodigdheden-prestashopinstalleren"></a>

Nu dat aan alle vereisten is voldaan, kunt u verder gaan met de installatiehandleiding: [http://doc.prestashop.com/display/PS16/PrestaShop+installeren](prestashop-installeren.md).
