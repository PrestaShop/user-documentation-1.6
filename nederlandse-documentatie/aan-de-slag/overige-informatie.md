# Overige informatie

**Inhoudsopgave**

/\*\<!\[CDATA\[\*/\
div.rbtoc1597237783222 {padding: 0px;}\
div.rbtoc1597237783222 ul {list-style: disc;margin-left: 0px;}\
div.rbtoc1597237783222 li {margin-left: 0px;padding-left: 0px;}\
\
/\*]]>\*/

* [Overige informatie](overige-informatie.md#Overigeinformatie-Overigeinformatie)
  * [Houd altijd een testversie bij de hand!](overige-informatie.md#Overigeinformatie-Houdaltijdeentestversiebijdehand!)
  * [Controleren of de GD library aanwezig is](overige-informatie.md#Overigeinformatie-ControlerenofdeGDlibraryaanwezigis)

## Overige informatie <a href="#overigeinformatie-overigeinformatie" id="overigeinformatie-overigeinformatie"></a>

### Houd altijd een testversie bij de hand! <a href="#overigeinformatie-houdaltijdeentestversiebijdehand" id="overigeinformatie-houdaltijdeentestversiebijdehand"></a>

Nadat u klaar bent met het volledig instellen van uw winkel, maar voordat u het publiek bereikbaar maakt, raden wij **sterk** aan om eerst een lokale testversie aan te maken (met [WAMP](http://en.wikipedia.org/wiki/Comparison\_of\_WAMPs) voor Windows, [MAMP](http://en.wikipedia.org/wiki/MAMP) voor Mac, of [LAMP](http://en.wikipedia.org/wiki/LAMP\_\(software\_bundle) voor Linux, of [XAMPP](http://www.apachefriends.org/en/xampp.html) elk van de platforms), of op een andere locatie op uw webserver.

Deze tweede instantie kan nuttig zijn als acceptatieomgeving waarin u alle toekomstige veranderingen toepast voor uw online PrestaShop-winkel, zonder dat de productieomgeving wordt aangetast. Op deze manier, als er een fout wordt ontdekt, blijft uw productieversie intact.

Nadat u hebt vastgesteld dat uw testversie naar behoren werkt, kopieert u de testversie naar de live-versie. Het is het beste om dit buiten de spitsuren te doen, en om uw webwinkel tijdelijk in onderhoudsmodus te zetten vanuit uw back office.&#x20;

### Controleren of de GD library aanwezig is <a href="#overigeinformatie-controlerenofdegdlibraryaanwezigis" id="overigeinformatie-controlerenofdegdlibraryaanwezigis"></a>

De [GD library](http://www.boutell.com/gd/) zorgt ervoor dat PrestaShop afbeeldingen kan bewerken, nadat u ze hebt geüpload. Het gaat hier vooral om het vergroten/verkleinen van afbeeldingen.

Standaard is de GD library ingeschakeld, maar als dat niet het geval is zijn dit de standaardinstructies voor Windows:

1. Open php.ini in de hoofdmap van uw PHP-map.
2. Verwijder de comment bij extension=`php_gd2.dll` (ergens halverwege het bestand, in het midden van een lange lijst met extensies) door de ";" aan het begin van de regel te verwijderen.
3. Start PHP opnieuw op.

Als u geen toegang hebt tot het php.ini bestand (wat vaak het geval is bij gedeelde hosting), neem dan contact op met uw hostingprovider.
