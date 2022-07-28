# Backups aanmaken en terugzetten

**Inhoudsopgave**

/\*\<!\[CDATA\[\*/\
div.rbtoc1597237783784 {padding: 0px;}\
div.rbtoc1597237783784 ul {list-style: disc;margin-left: 0px;}\
div.rbtoc1597237783784 li {margin-left: 0px;padding-left: 0px;}\
\
/\*]]>\*/

* [Backups aanmaken en terugzetten](backups-aanmaken-en-terugzetten.md#Backupsaanmakenenterugzetten-Backupsaanmakenenterugzetten)
  * [Uw eigen reservekopie maken](backups-aanmaken-en-terugzetten.md#Backupsaanmakenenterugzetten-Uweigenreservekopiemaken)
    * [Uw bestanden backuppen](backups-aanmaken-en-terugzetten.md#Backupsaanmakenenterugzetten-Uwbestandenbackuppen)
    * [Uw database backuppen](backups-aanmaken-en-terugzetten.md#Backupsaanmakenenterugzetten-Uwdatabasebackuppen)
      * [Gebruik maken van PrestaShop's gereedschap voor de database](backups-aanmaken-en-terugzetten.md#Backupsaanmakenenterugzetten-GebruikmakenvanPrestaShop%27sgereedschapvoordedatabase)
      * [phpMyAdmin gebruiken](backups-aanmaken-en-terugzetten.md#Backupsaanmakenenterugzetten-phpMyAdmingebruiken)
      * [Gebruik maken van de databasetool van uw provider](backups-aanmaken-en-terugzetten.md#Backupsaanmakenenterugzetten-Gebruikmakenvandedatabasetoolvanuwprovider)
  * [Uw reservekopie herstellen](backups-aanmaken-en-terugzetten.md#Backupsaanmakenenterugzetten-Uwreservekopieherstellen)
    * [Uw server opschonen](backups-aanmaken-en-terugzetten.md#Backupsaanmakenenterugzetten-Uwserveropschonen)
      * [Een onderhoudspagina maken](backups-aanmaken-en-terugzetten.md#Backupsaanmakenenterugzetten-Eenonderhoudspaginamaken)
      * [Bestanden verwijderen](backups-aanmaken-en-terugzetten.md#Backupsaanmakenenterugzetten-Bestandenverwijderen)
      * [Gegevens verwijderen](backups-aanmaken-en-terugzetten.md#Backupsaanmakenenterugzetten-Gegevensverwijderen)
    * [Uw bestanden en gegevens herstellen](backups-aanmaken-en-terugzetten.md#Backupsaanmakenenterugzetten-Uwbestandenengegevensherstellen)
      * [Uw bestanden herstellen](backups-aanmaken-en-terugzetten.md#Backupsaanmakenenterugzetten-Uwbestandenherstellen)
      * [Uw gegevens herstellen](backups-aanmaken-en-terugzetten.md#Backupsaanmakenenterugzetten-Uwgegevensherstellen)

## Backups aanmaken en terugzetten <a href="#backupsaanmakenenterugzetten-backupsaanmakenenterugzetten" id="backupsaanmakenenterugzetten-backupsaanmakenenterugzetten"></a>

Of u nu uw PrestaShop bijwerkt door middel van de automatische methode of de handmatige, u moet ervoor zorgen dat u uw eigen reservekopie maakt. Eén waarop u kunt vertrouwen en op uw eigen manier kunt herstellen.

Wanneer u de winkel gaat bijwerken, wordt er sterk aangeraden om de backup uit te voeren nádat u de winkel in onderhoudsmodus hebt geplaatst. Op deze manier weet u zeker dat er geen klantdata verloren gaat wanneer u de backup hebt moeten herstellen. Voer geen update uit als van zowel de bestanden als data geen goede reservekopie is gemaakt.

Voor de processen zoals beschreven in dit hoofdstuk moet u gebruik maken van een FTP-client, SQL-data downloaden vanaf een webserver en zelfs uw bestanden en data verwijderen. Als u niet goed weet hoe u gebruik maakt van deze programma's en tools, dan moet u hulp vragen bij een technische vriend/buurman/collega/etc. en de tijd nemen om elke stap te leren begrijpen. Als u deze technieken niet beheerst, is de kans groot dat u uw winkel voor altijd kwijtraakt.

### Uw eigen reservekopie maken <a href="#backupsaanmakenenterugzetten-uweigenreservekopiemaken" id="backupsaanmakenenterugzetten-uweigenreservekopiemaken"></a>

Maak eerst een map aan op uw computer waar u zowel de PrestaShop-bestanden en gegevens plaatst. Stop de huidige datum in de naam van de map, om precies te weten wanneer te reservekopie is gemaakt.

#### Uw bestanden backuppen <a href="#backupsaanmakenenterugzetten-uwbestandenbackuppen" id="backupsaanmakenenterugzetten-uwbestandenbackuppen"></a>

Dit is erg gemakkelijk:

1. Verbind met uw webserver door middel van een FTP-client zoals FileZilla.
2. Download alle bestanden van PrestaShop's online map naar uw eigen lokale reservekopiemap.

Dit proces neemt enige tijd in beslag, afhankelijk van uw internet en de snelheid van uw server. PrestaShop 1.6 heeft ongeveer 10.000 bestanden in 2.500 mappen en dan zijn uw eigen bestanden nog niet eens meegerekend (productafbeeldingen, thema's, modules, etc.), of de afbeeldingen van uw bezoekers. Raak uw FTP-client niet aan totdat de bestanden zijn overgebracht.

#### Uw database backuppen <a href="#backupsaanmakenenterugzetten-uwdatabasebackuppen" id="backupsaanmakenenterugzetten-uwdatabasebackuppen"></a>

Terwijl de bestanden worden gedownload, kunt u de tijd nemen om een reservekopie te maken van uw gegevens. Er zijn meerdere manieren om dit te doen...

**Gebruik maken van PrestaShop's gereedschap voor de database**

PrestaShop 1.6 heeft zijn eigen gereedschap voor de database, genaamd "DB-Backup". Deze is te vinden in het menu "Geavanceerde instellingen". Deze tool wordt in detail uitgelegd in [Database backup](../gebruikershandleiding/geavanceerde-instellingen/database-backup.md), maar hier is de basis:

1. Lees de disclaimer en klik op de knop "Ik heb de disclaimer gelezen. Creëer een nieuwe reservekopie." PrestaShop maakt een zip-archief van al uw databasetabellen.
2. Klik op het backup-bestand dat verschijnt in de nieuwe download-sectie. Dit zorgt ervoor dat u het backuparchief downloadt naar uw computer; deze heeft meestal een naam als "`1349964600-71d48cfe.sql.bz2`". Bewaar dat bestand in uw backupmap.

**phpMyAdmin gebruiken**

Als u liever phpMyAdmin gebruikt in plaats van PrestaShop's tool, dan kan dat natuurlijk ook! Dat gaat als volgt:

1. Login op phpMyAdmin.
2. Vanaf het hoofdscherm selecteert u "Databases".
3. Klik op de naam van PrestaShop's database om deze te openen.
4. In het databasescherm klikt u op de tab "Exporteren".
5. In het exportscherm:
   1. Zorg ervoor dat alle databasetabellen van PrestaShop zijn geselecteerd, en alleen deze. Ze zouden moeten beginnen met het voorvoegsel `ps_` (of elk ander voorvoegsel dat u gekozen hebt tijdens de installatie van PrestaShop).
   2. Zorg ervoor dat het rondje met de tekst "SQL" is geselecteerd.
   3. In de sectie "Object-aanmaakopties" kiest u de volgende checkboxen:
      * "`DROP TABLE / VIEW / PROCEDURE / FUNCTION / EVENT / TRIGGER` statement toevoegen"
      * "IF NOT EXISTS" onder "`CREATE TABLE` opties:"
      * &#x20;"AUTO\_INCREMENT" onder "CREATE TABLE opties:"
      * Voeg aanhalingstekens toe aan tabel- en kolomnamen (Beschermt tabel- en kolomnamen die speciale tekens en sleutelwoorden bevatten)
   4. In de sectie "Opmaakspecifieke opties" kiest u de volgende checkbox:
      * "Structuur"
   5. In de sectie "Uitvoer" kiest u de volgende opties:
      * Opslaan als bestand
      * Verander het veld "Bestands-naam template" niet!
      * Kies "gezipt" of "ge-gzipt" bij "Compressie".
   6. Klik op de knop "Starten".
6. De browser begint met het downloaden van het gegevensbestand. Bewaar dit bestand in de backupmap op uw computer.

Als uw server te zwak is om alle tabellen tegelijkertijd te exporteren, dan kunt u de reversekopie opbreken in enkele bestanden. Kies bijvoorbeeld de eerste 20 `ps_` datatabellen en exporteer die, daarmee duidelijk aangevend in de bestandsnaam dat dit het eerste bestand is van velen. Zodra er een reservekopie is gemaakt van deze tabellen, kunt u dit herhalen voor de volgende 20 tabellen, enzovoort. Vergeet niet de positie aan te geven in de bestandsnaam.

**Gebruik maken van de databasetool van uw provider**

Uw webhost stelt misschien geen phpMyAdmin beschikbaar en heeft in plaats daarvan zijn eigen tool, of een andere minder bekende, zoals de tool die in cPanel is geïntegreerd. Lees daarvoor de documentatie van uw hostingprovider. Het doel is om een export te verkrijgen van uw gegevens in SQL-formaat. Dit kan gecomprimeerd zijn, maar is niet noodzakelijk.

### Uw reservekopie herstellen <a href="#backupsaanmakenenterugzetten-uwreservekopieherstellen" id="backupsaanmakenenterugzetten-uwreservekopieherstellen"></a>

Nadat een automatische update is mislukt (wat de enige reden is om een update ongedaan te maken), en als u nog steeds bij het administratiepaneel van PrestaShop kunt, dan kunt u de sectie "terugzetten" van de "1-Click Upgrade"-module gebruiken om de vorige versie te herstellen. Lees hoofdstuk [Automatisch bijwerken](automatisch-bijwerken.md) voor meer informatie. Als u geen toegang hebt tot de module of als u de module niet hebt gebruikt om uw PrestaShop bij te werken, dan moet u de instructies in deze sectie volgen.

Eén probleem met de 1-Click Upgrade-module is dat uw altijd verbinding moet kunnen maken met de backoffice van PrestaShop als u de vorige versie wilt terugzestten – en in sommige gevallen kunnen vreemde configuraties voorkomen dat u nog kunt inloggen in uw backoffice en daardoor het gehele administratiepaneel onbruikbaar maakt (u kunt proberen om de browsercache te legen en het administratiepaneel enkele keren opnieuw te laden... Het zou slechts een tijdelijk CSS-probleem kunnen zijn).

Dit is waarom de 1-Click Upgrade-module aanraadt om uw eigen reservekopieën te maken: voordat u gaat upgraden, moet u een kopie hebben op uw harde schijf. In het kort:

* Een map (of zip-archief), met alle bestanden van PrestaShop, vooral die van uw eigen installatie: configuratiebestanden, thema's, modules, afbeeldingen, uploads van gebruikers, PDF en e-mailsjablonen, aangepaste klassen, etc.
* Een volledige kopie van uw database, in een ruw SQL-bestand of een zip-archief.

Deze lokale kopie van uw site moet extreem recent: in het beste geval is deze net gemaakt, nadat u uw winkel in onderhoudsmodus hebt geplaatst en vlak voordat u het upgrade-script hebt gedraaid (handmatig of automatisch). Op deze manier kunt u terug naar de meest recente versie van uw winkel, zonder gegevens kwijt te raken (gebruikers, verkopen, statistieken, etc.).

#### Uw server opschonen <a href="#backupsaanmakenenterugzetten-uwserveropschonen" id="backupsaanmakenenterugzetten-uwserveropschonen"></a>

Nu dat u een complete en recente lokale kopie hebt van uw winkel van de vorige versie, en de poging om de laatste versie van uw PrestaShop online te krijgen is niet gelukt, resulterende in een kapot administratiepaneel (de frontend zou ook onbereikbaar moeten zijn, omdat u uw winkel in onderhoudsmodus hebt geplaatst). Het terugzetten van de vorige versie betekent het herstellen van uw lokale kopie naar de server en dat betekent dat u vanaf een schone staat moet beginnen om te voorkomen dat nieuwe en oude data door elkaar raken, wat uw site verder stuk kan maken.

Maak u geen zorgen: omdat alle bestanden en gegevens zich op uw computer bevinden, kunt u ze snel herstellen. Omdat bezoekers nog steeds uw website proberen te bezoeken, moet u een aangepaste onderhoudspagina tonen terwijl u werk verricht aan uw winkel.

**Een onderhoudspagina maken**

Het herstellen van uw winkel naar de vorige versie kan veel tijd in beslag nemen, afhankelijk van hoe groot uw winkel is en dus afhankelijk van het aantal bestanden en data dat u moet verplaatsen. Het is daarom belangrijk om een onderhoudspagina te tonen die niet afhankelijk is van PrestaShop.

Inderdaad, de huidige onderhoudspagina leunt sterk op PrestaShop om informatie te tonen: winkelnaam, winkellogo, vertalingen, CSS-bestand, metadata, etc. Zelfs als uw winkel momenteel in onderhoudsmodus is en de onderhoudspagina toont aan bezoekers, kan de pagina straks niet meer werken als u uw data verwijderd... Zelfs dit bestand zal er straks niet meer zijn als uw bestanden verwijderd, want de pagina is onderdeel van uw huidige thema. Om precies te zijn, in het bestand `maintenance.tpl`.

Om die reden is een aangepaste onderhoudspagina nodig. Het hoeft er niet erg mooi uit te zien, omdat de rol is om even snel aan gebruikers te tonen dat er onderhoud is en ze de website later weer kunnen bezoeken.

Hier is een simpel voorbeeld voor een internationale site:**Voorbeeld van onderhoudspagina**

```
<!DOCTYPE html>
<html>
  <head>
    <title>Our shop is under maintenance</title>    
  </head>
  <body>
    <p>In order to perform site maintenance, our online shop has shut down temporarily.</p>
    <p>We apologize for the inconvenience and ask that you please try again later.</p>
  </body>
</html>
```

Kopieer deze code naar een `index.html` bestand en upload deze naar de map van PrestaShop door middel van uw FTP-client. Op de meeste servers heeft het `index.html` bestand een hogere prioriteit dan het `index.php` bestand, dus zodra u `index.html` upload naar de hoofdmap van PrestaShop, dan moet uw winkel de aangepaste ondershoudspagina tonen in plaats van die van PrestaShop. Controleer uw serverinstellingen om te zien of dit voor u ook geldt.

**Bestanden verwijderen**

Maak verbinding met uw webruimte met uw FTP-client. Ga naar de map van PrestaShop (als deze zich niet in de hoofdmap bevindt van de server), selecteer alle bestanden en mappen in de map van PrestaShop (behalve `index.html`, uw aangepaste onderhoudspagina) en verwijder ze allemaal. U moet dit alleen doen als u zeker weet dat u lokaal een exacte kopie hebt van uw webwinkel.

Dit kan een aantal minuten duren, omdat PrestaShop meer dan 7.000 bestanden heeft. Terwijl deze worden verwijderd, kunt u de datatabellen verwijderen (volgende sectie).

**Gegevens verwijderen**

Open uw database manager — meestal stelt u hostingprovider phpMyAdmin of een aangepaste tool beschikbaar. Bekijk de database van uw PrestaShop-installatie: selecteer de tabellen die beginnen met `ps_` (of het voorvoegsel dat u gekozen hebt bij de installatie van PrestaShop); als PrestaShop het enige softwarepakket is dat gebruikmaakt van deze database, dan kunt u op de link "Selecteer alles" aan de onderkant klikken en vervolgens "Verwijderen" selecteren. Op het volgende scherm vraag phpMyAdmin of u zeker bent: klik op de knop "Ja". Herhaal deze stap, totdat alle tabellen zijn verwijderd.

Wacht het proces rustig af. Uiteindelijk toont phpMyAdmin de database, die geen tabellen meer heeft.

Uw server heeft nu geen bestanden en gegevens meer van PrestaShop, behalve het bestand `index.html`. Het is nu tijd om uw winkel weer online te krijgen, deze keer met de reservekopie waarvan u weet dat het werkt!

#### Uw bestanden en gegevens herstellen <a href="#backupsaanmakenenterugzetten-uwbestandenengegevensherstellen" id="backupsaanmakenenterugzetten-uwbestandenengegevensherstellen"></a>

Zodra uw FTP-client klaar is met het verwijderen van bestanden, kunt u beginnen met het uploaden van bestanden die zijn opgeslagen op uw computer! Omdat dit proces enige tijd in beslag neemt is het belangrijk om geen kostbare minuten te verliezen (want dit kan leiden in gemiste verkopen), zodat uw website niet langer offline blijft dan nodig is.

**Uw bestanden herstellen**

Dit proces is net zo gemakkelijk als bovenstaand proces:

1. Maak verbinding met uw webserver met behulp van een FTP-client, zoals FileZilla.
2. Upload alle bestanden vanaf uw lokale reservekopiemap naar de map van PrestaShop.

De online-map van PrestaShop zou leeg moeten zijn om ruimte te maken voor de nieuwe bestanden en te voorkomen dat oude en nieuwe bestanden conflicteren. Als u niet alle online-bestanden hebt verwijderd (behalve `index.html`, uw onderhoudspagina), dan moet u uw FTP-client vertelen om bestaande bestanden te overschrijven. U moet geen enkel bestand overhouden dat ten tijde van de mislukte update op uw server stond.

**Uw gegevens herstellen**

Het stappenplan dat hier beschreven wordt gebruikt phpMyAdmin; dat is een standaard webtool. Als uw hostingprovider een andere tool gebruikt om uw databases te beheren, dan moet u het stappenplan aanpassen aan deze tool. Bekijk de documentatie van uw hostingprovider voor meer informatie.

Het herstellen van de gegevens net zo gemakkelijk als een kopie maken van de gegevens:

1. Login op phpMyAdmin.
2. Vanaf het hoofdscherm kiest u "Databases".
3. Klik op de naam van de database die PrestaShop gebruikt.
4. Op het databasescherm, klikt u op de tab "Importeren".
5. In het importeerscherm:
   1. In de sectie "Te importeren bestand", klikt u op "Bladeren..." en zoekt u naar het reservekopiebestand van uw gegevens. Het kan het ruwe SQL-bestand zijn (`.sql`) of een gecomprimeerde versie (`.sql.zip`, `.sql.gzip`, `.sql.tar.gz`, etc.).
   2. In de sectie "Opmaak", zorg ervoor dat het formaat "SQL" is geselecteerd.
   3. Klik op de knop "Starten".
6. De browser zou nu moeten beginnen met het uploaden van het reservekopiebestand.

Als u meer dan één reservekopiebestand hebt, dan moet u deze achter elkaar importeren.

Asl laatste verwijderd u uw onderhoudspagina weer (met de naam `index.html`). Nu is uw website gelukig weer online!
