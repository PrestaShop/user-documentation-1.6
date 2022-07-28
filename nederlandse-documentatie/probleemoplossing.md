# Probleemoplossing

**Inhoudsopgave**

/\*\<!\[CDATA\[\*/\
div.rbtoc1597237805672 {padding: 0px;}\
div.rbtoc1597237805672 ul {list-style: disc;margin-left: 0px;}\
div.rbtoc1597237805672 li {margin-left: 0px;padding-left: 0px;}\
\
/\*]]>\*/

* [Probleemoplossing](probleemoplossing.md#Probleemoplossing-Probleemoplossing)
  * [Schakel foutmeldingen in als u witte pagina's krijgt](probleemoplossing.md#Probleemoplossing-psmodedevtrueSchakelfoutmeldingeninalsuwittepagina%27skrijgt)
  * [Het is niet meer mogelijk om in te loggen](probleemoplossing.md#Probleemoplossing-Hetisnietmeermogelijkominteloggen)
  * [Een wachtwoord handmatig herstellen](probleemoplossing.md#Probleemoplossing-Eenwachtwoordhandmatigherstellen)
  * [PrestaShop verstuurt het nieuwe wachtwoord niet](probleemoplossing.md#Probleemoplossing-PrestaShopverstuurthetnieuwewachtwoordniet)
  * [Inloggen nadat per ongeluk het standaardtaalpakket is verwijderd](probleemoplossing.md#Probleemoplossing-Inloggennadatperongelukhetstandaardtaalpakketisverwijderd)

## Probleemoplossing <a href="#probleemoplossing-probleemoplossing" id="probleemoplossing-probleemoplossing"></a>

### Schakel foutmeldingen in als u witte pagina's krijgt <a href="#probleemoplossing-psmodedevtrueschakelfoutmeldingeninalsuwittepaginaskrijgt" id="probleemoplossing-psmodedevtrueschakelfoutmeldingeninalsuwittepaginaskrijgt"></a>

Module

Voor PrestaShop 1.6 en hoger kunt u gebruikmaken van een module: [https://www.prestashop.com/forums/topic/513401-free-module-enable-debug-mode-from-back-office/](https://www.prestashop.com/forums/topic/513401-free-module-enable-debug-mode-from-back-office/)

Als uw backoffice en/of frontoffice witte pagina's toont, zonder foutmeldingen, dan is het noodzakelijk om de PHP-fouten zichtbaar te maken om het probleem te vinden.

Dit kan gedaan worden met het bestand `/config/defines.inc.php` in uw PrestaShop-installatie. U moet de volgende regel aanpassen:

```
define('_PS_MODE_DEV_', false);
```

...en veranderen naar:

```
define('_PS_MODE_DEV_', true);
```

Ga nu naar dezelfde pagina in uw winkel. PrestaShop toont alle relevante foutmeldingen (als ze er zijn), die u moeten helpen bij het oplossen van het probleem.

Zodra het probleem is opgelost, moet u de instellingen weer terugzetten: bewerk `/config/defines.inc.php` en zet de waarde `false` weer terug bij `_PS_MODE_DEV_`.

### Het is niet meer mogelijk om in te loggen <a href="#probleemoplossing-hetisnietmeermogelijkominteloggen" id="probleemoplossing-hetisnietmeermogelijkominteloggen"></a>

Er zijn gevallen waarbij PrestaShop uw e-mail en wachtwoord niet meer herkent, waardoor het onmogelijk wordt om in te loggen op de front- of backoffice. De gebruiker wordt simpelweg teruggestuurd naar het loginscherm. Sommige gebruikers melden dat IE10 de enige browser is die hier last van heeft.

Dit is meestal een probleem dat veroorzaakt worden door de browser cookie van uw winkel: als de gebruiker herhaaldelijk in- en uitlogt, dan kan er iets fout gaan met de encryptiesleutels.

In elk geval is er een manier om dit op te lossen door de cache en cookies in een browser te verwijderen. Hier is een pagina met uitleg hoe u dit doet: [https://support.google.com/mail/answer/32050?hl=nl](https://support.google.com/mail/answer/32050?hl=nl)[.](https://support.google.com/mail/answer/32050?hl=en)

### Een wachtwoord handmatig herstellen <a href="#probleemoplossing-eenwachtwoordhandmatigherstellen" id="probleemoplossing-eenwachtwoordhandmatigherstellen"></a>

Het komt voor dat er niets gebeurt als u een nieuw wachtwoord opvraagt. Er kunnen een aantal redenen voor zijn, maar het belangrijkste is dat er weer ingelogd kan worden.

Hiervoor moet u toegang hebben tot uw database, door bijvoorbeeld gebruik te maken van phpMyAdmin.

U moet de volgende procedure volgen:

1. Open het bestand `/config/settings.inc.php`, in de hoofdmap van de winkel. Zoek de regel met "`_COOKIE_KEY`\_". Kopieer de inhoud ernaast (zonder aanhalingstekens): het is onderdeel van de MD5 van uw wachtwoord.
2. U moet nu een nieuwe MD5-hash genereren voor uw wachtwoord:
   1. Ga naar [http://www.miraclesalad.com/webtools/md5.php](http://www.miraclesalad.com/webtools/md5.php).
   2. Plak de waarde van "`_COOKIE_KEY`\_" in het tekstveld in het tekstveld en voeg hier uw wachtwoord aan toe, xykxB41JrEacRIoZxDioPNRmKeuO3ixCLygNxBAkeOkAHf2YUVESuT9jMIJNWACHTWOORD, waar de cookie\_key eindigt met T9j en uw wachtwoord MIJNWACHTWOORD is (het mag van alles zijn).
   3. Klik op de knop "md5": dit maakt een MD5-hash aan van de inhoud van het tekstveld. Kopieer deze.
3. U moet nu de hash in uw database stoppen:
   1. Open de database van uw winkel met phpMyAdmin. Als u niet weet hoe u phpMyAdmin gebruikt, kunt u uw webmaster of hostingprovider om hulp vragen.
   2. Open de tabel `pw_employee`, zoek de rij die bij uw account hoort (u moet uw voor- en achternaam zien, en e-mailadres) en klik op de knop "Bewerken".
   3. Zoek het veld `passwd` en voer hier de MD5 in die u zojuist hebt gegenereerd/
4. Log in op uw backoffice met het e-mailadres dat u in de tabel ziet en het wachtwoord dat u zojuist hebt gebruikt (MIJNWACHTWOORD).

Als dit nog steeds niet werkt, dan kunt u phpMyAdmin gebruiken om naar de tabel `ps_shop_url` te gaan en de waarde van de hoofdwinkel kunt controleren. De `id` is 1. Het moet het bestandspad van de winkel bevat:

* Als uw winkel zich in de hoofdmap van de server bevindt, dan moet deze variabele "/" zijn.
* Als u winkel zich in een submap bevindt, moet deze zijn ingevoerd. Bijvoorbeeld, als deze te vinden is op  "[http://www.mywebsite/shop/](http://www.mywebsite/shop/)", dan moet de variabele de waarde "/shop/" bevatten.

Als alles faalt, neemt u contact op met het PrestaShop supportteam op: [http://support.prestashop.com/en/](http://support.prestashop.com/en/).

### PrestaShop verstuurt het nieuwe wachtwoord niet <a href="#probleemoplossing-prestashopverstuurthetnieuwewachtwoordniet" id="probleemoplossing-prestashopverstuurthetnieuwewachtwoordniet"></a>

Om een nieuw wachtwoord aan te vragen moet uw winkel kunnen verbinden met de SMTP-server, zodat PrestaShop e-mails kan verzenden.

Er zijn twee oplossingen beschikbaar:

1. **Configureer de SMTP-server om e-mails te versturen**\
   ****
   1. Vraag uw hostingprovider om de informatie.
   2. Ga naar uw backoffice en dan de pagina "E-mail" onder het menu "Geavanceerde instellingen".
   3. Selecteer de optie "Stel mijn eigen SMTP-parameters in". Er verschijnt een formulier: vul de informatie van uw host in.
   4. Bewaar uw  veranderingen.
   5. Vraag opnieuw om een wachtwoord. U zou deze moeten ontvangen.
2. **Volg deze stappen**:
   1. Kies een nieuw wachtwoord. In ons voorbeeld: "\$$$rabbit$159\$$$".
   2. Met uw FTP-client opent u het bestand `login.php` in de administratiemap (de naam hangt af van uw installatie).
   3. Aan de onderkant van het bestand voegt u de volgende regel toe:\
      `echo md5( PSQL( _COOKIE_KEY_ . 'newpassword' ) );`\
      Dus met ons wachtwoord:\
      `echo md5( PSQL( _COOKIE_KEY_ . '$$$rabbit$159$$$' ) );`\
      Plaat hier uw eigen wachtwoord!
3. Ga naar het loginscherm van de backoffice, alsof u wilt inloggen, en kopieer de tekst dat aan de onderkant van de pagina verschijnt (bijv. a0ee884b507dd4624ce51968cfbb19a9).
4. Ga naar de database van PrestaShop, met bijvoorbeeld phpMyAdmin. In de tabel `ps_employee` vervangt u de huidige waarde in de kolom `passwd` met de nieuwe waarde voor het account waarvan u het wachtwoord wilt wijzigen. Sla uw instellingen op.
5. U kunt nu weer inloggen met het gebruikelijke account en nieuwe wachtwoord.

### Inloggen nadat per ongeluk het standaardtaalpakket is verwijderd <a href="#probleemoplossing-inloggennadatperongelukhetstandaardtaalpakketisverwijderd" id="probleemoplossing-inloggennadatperongelukhetstandaardtaalpakketisverwijderd"></a>

In het geval dat u het standaardtaalpakket hebt verwijderd van uw winkel, dan kunnen er problemen optreden als u wilt verbinden met uw backoffice.

Zo kunt u het probleem oplossen als de standaardtaal Nederlands was:

1. Ga naar phpMyAdmin
2. Kies de database van uw winkel en selecteerde tabel `ps_lang.`
3. Klik op de knop "Toevoegen" aan de bovenkant een maak een nieuw item aan met de volgende waarden:
   * `id_lang` -> 1
   * `name` -> Nederlands
   * `active` -> 1
   * `iso_code` -> nl
   * `language_code` -> nl
   * `date_format_lite` -> d-m-Y
   * `date_format_full` -> d-m-Y H:i:s
   * `is_rtl` -> 0
4. Voor de query uit.

U moet nu weer in kunnen loggen.
