# Was für die Installation benötigt wird

**Inhaltsverzeichnis**

* [Was für die Installation benötigt wird](was-fuer-die-installation-benoetigt-wird.md#WasfürdieInstallationbenötigtwird-WasfürdieInstallationbenötigtwird)
  * [Systemvoraussetzungsanleitung](was-fuer-die-installation-benoetigt-wird.md#WasfürdieInstallationbenötigtwird-Systemvoraussetzungsanleitung)
  * [Detaillierte Installationsanweisung](was-fuer-die-installation-benoetigt-wird.md#WasfürdieInstallationbenötigtwird-DetaillierteInstallationsanweisung)
    * [Eine Domain registrieren](was-fuer-die-installation-benoetigt-wird.md#WasfürdieInstallationbenötigtwird-EineDomainregistrieren)
    * [Einen Host finden](was-fuer-die-installation-benoetigt-wird.md#WasfürdieInstallationbenötigtwird-EinenHostfinden)
    * [Technische Vorraussetzungen](was-fuer-die-installation-benoetigt-wird.md#WasfürdieInstallationbenötigtwird-TechnischeVorraussetzungen)
    * [Werkzeuge](was-fuer-die-installation-benoetigt-wird.md#WasfürdieInstallationbenötigtwird-Werkzeuge)
    * [Planung](was-fuer-die-installation-benoetigt-wird.md#WasfürdieInstallationbenötigtwird-Planung)
    * [PrestaShop installieren](was-fuer-die-installation-benoetigt-wird.md#WasfürdieInstallationbenötigtwird-PrestaShopinstallieren)

## Was für die Installation benötigt wird <a href="#wasfuerdieinstallationbenoetigtwird-wasfuerdieinstallationbenoetigtwird" id="wasfuerdieinstallationbenoetigtwird-wasfuerdieinstallationbenoetigtwird"></a>

### Systemvoraussetzungsanleitung <a href="#wasfuerdieinstallationbenoetigtwird-systemvoraussetzungsanleitung" id="wasfuerdieinstallationbenoetigtwird-systemvoraussetzungsanleitung"></a>

Hier ist eine kurze Liste von Voraussetzungen für die Installation von PrestaShop 1.6. Ausführliche Informationen zu den Systemvoraussetzungen finden Sie im nächsten Kapitel.

* Systemvoraussetzungen:
  * PHP 5.2 oder Neuer.
    * Nützliche Einstellungen - Setzen Sie: `allow_url_fopen` auf On, `register_globals auf` Off, `magic_quotes_*` auf Off, `safe_mode auf` Off (all in the `php.ini` file), `file_max_upload_size` auf "16M".
    * Nützliche PHP Erweiterungen: PDO\_MySQL, cURL, SimpleXML, mcrypt, GD, OpenSSL, DOM, SOAP (alle in der der `php.ini`).
    * Nützliche Server Werkzeuge: cron/crontab, Memcached.
  * MySQL 5.0 oder Neuer.
  * empfohlen: \

    * Unix/Linux hosting.
    * Apache Web Server 1.3 oder Neuer oder nginx Web Server.
      * Apache Modul Einstellungen: `mod_rewrite` enabled, `mod_security` disabled, `mod_auth_basic` disabled.
    * Mindestens 64 MB RAM zugeordnet zu PHP.
* Zugangsdaten zu Ihrem FTP Server und zu Ihrer MySQL Datenbank\

  * Diese erhalten Sie von Ihrem Hoster, wenn Sie keine lokale Installation erstellen.&#x20;
* Ein beliebiger Text-Editor
* Ein beliebiger FTP-Client
* Ein beliebiger Web-Browser (Internet Explorer: mindestens IE8).

Außerdem müssen Sie wissen unter welcher URL/Ihrer Domain Sie Ihr(e) Shop(s) erreichen wollen.

Schauen Sie auch auf die offizielle Seite mit den Systemvoraussetzungen: [http://www.prestashop.com/de/system-requirements](http://www.prestashop.com/de/system-requirements).

Die Systemvoraussetzungen werden erfüllt? Folgen Sie der Installationsanleitung: [http://doc.prestashop.com/display/PS16/Installation+PrestaShop](http://doc.prestashop.com/display/PS16/Installation+PrestaShop).

### Detaillierte Installationsanweisung <a href="#wasfuerdieinstallationbenoetigtwird-detaillierteinstallationsanweisung" id="wasfuerdieinstallationbenoetigtwird-detaillierteinstallationsanweisung"></a>

Prestashop ist eine Web-Applikation: sie bedarf eines Webservers, um ausgeführt zu werden und sie benötigt eine Domain, damit Ihre Besucher ihren Shop aufrufen können

#### Eine Domain registrieren <a href="#wasfuerdieinstallationbenoetigtwird-einedomainregistrieren" id="wasfuerdieinstallationbenoetigtwird-einedomainregistrieren"></a>

Bevor sie etwas downloaded oder installieren müssen Sie Ihrem Prestashop ein Zuhause einrichten.Dieses besteht aus zwei Komponenten: einer Domain und einem Webserver. Eine Domain dient der Identifikation für Ihre Website z.B. example.com oder meinonlineshop.net. Die domain verweist auf Ihren Webserver und repräsentiert ihren Shop im Internet.

Sie müssen eine Domain für Ihren Shop kaufen. In der Regel erhalten Sie eine Domain zusammen mit einem Online-Hostingpaket: einige Webhoster bieten auch kostenlose Domains für neue Accounts. Teilweise ist auch das erste Jahr gratis. Dies macht es einfacher direkt die Kombination von Hosting und Domain in einem Rutsch zu holen.

Es kann manchmal Probleme mit Hostern geben. Wenn Sie unzufrieden sind mit Ihrem Hostingangebot, und sich entschließen zu einem besseren Hoster zu wechseln müssen Sie Ihre Dateien, Daten(banken) und die Domain(s) zu diesem transferieren.

Die Dateien und Daten sind einfach zu transferieren, aber für den Umzug der Domain sind die Hoster als Registrare zuständig. Diese können unter Umständen den Domainumzug blockieren oder Gebühren für den Umzug verlangen. Und weil Ihre Domain ihre webadresse und oftmals auch die Marke Ihres Geschäfts darstellt sollten Sie sich streng an die Webhosting Regeln halten.

Deswegen wird oft empfohlen seine Domain bei einem unabhängigen Registrar zu registrieren (siehe auch: [http://de.wikipedia.org/wiki/Domain\_Name\_Registrar](http://de.wikipedia.org/wiki/Domain\_Name\_Registrar)). Rein rechtlich können Sie eine Domain nicht kaufen. Sie können diese nur mieten, in der Regel für eine Jahresgebühr. Sie haben dann das Recht die Domain zu nutzen, solange Sie die Gebühr zahlen. Zahlen Sie die Gebühr nicht mehr verlieren Sie die Domain und eine beliebige andere Person kann sich das Recht der Nutzung erkaufen. Also auch wenn sie für die Registrierung der Domain bei einem Registrar extra bezahlen kann sich dies z.B. bei einem Hosterwechsel bezahlbar machen. Sie ändern einfach den DNS Eintrag und innerhalb von 24 Stunden ist Ihr Geschäft auf einem anderen Server für die Welt erreichbar.

Wenn Sie Lieber eine Domain von einem unabhängigen Registrar erhalten wollten, finden Sie im Folgenden einige Beispiele:

* Gandi: [http://en.gandi.net/](http://en.gandi.net/)
* Namecheap: [http://www.namecheap.com/](http://www.namecheap.com/)
* PairNIC: [https://www.pairnic.com/](https://www.pairnic.com/)

Dies sind nur ausgewählte Beispiele von einem viel größereren Angebot an Anbietern.

#### Einen Host finden <a href="#wasfuerdieinstallationbenoetigtwird-einenhostfinden" id="wasfuerdieinstallationbenoetigtwird-einenhostfinden"></a>

Nun, da Sie eine Domain haben, müssen Sie diese zu Prestashop leiten. Das heißt: Die Prestashop-Dateien müssen auf einem Webserver liegen. Möglicherweise haben Sie einen eigenen lokalen Webserver, meistens werden Webserver jedoch von Anbietern gehostet, (siehe: [http://en.wikipedia.org/wiki/Internet\_hosting\_service](http://en.wikipedia.org/wiki/Internet\_hosting\_service)), welche einen Webserver für einen monatlichen Preis vermieten.

Bevor Sie einen Onlineshop starten, müssen Sie sich für einen Provider entscheiden. Fast jeder Hoster unterstützt Prestashop,manche bieten jedoch optimierte Lösungen dafür an:

* 1&1 in Spanien: [1&1](http://www.prestashop.com/es/ecommerce-hosting/1and1)
* OVH in Frankreich: [OVH](http://www.ovh.com/fr/solutions/prestashop/?pk\_campaign=partenariatprestashop\&pk\_kwd=pagefr)
* InMotion in allen Ländern, außer Frankreich und Spanien: [InMotion](http://www.inmotionhosting.com/prestashop-hosting)

Werfen Sie einen Blick auf [unsere Hosting-Partner](http://www.prestashop.com/en/ecommerce-hosting)!

Wenn Sie einen Host wählen, achten Sie auf eine wichtige Vorraussetzung: PHP 5.2 (oder höher) ist eine Pflichtvorraussetzung, die Programmiersprache, in der Prestashop geschrieben ist, und MySQL 5 (oder höher), das Datenbanksystem, in dem Prestashop Daten speichert.Es gibt noch ein paar mehr Vorraussetzungen, lesen Sie dafür den Abschnitt "Technische Vorraussetzungen" weiter unten. PrestaShop kann ihren Onlineshop auch auf haus-eigenen Servern hosten.Unser PrestaBox service wurde konzipiert, um Kunden von jedem technischen Aufwand zu befreien, wie z.B. Installation und Updaten von Prestashop.

Bitte besuchen Sie unserere PrestaBox Website für weitere Informationen über unseren günstigen und sicheren Hosting Service. Diese Methode wird für Unternehmen mit geringer / ohne Erfahrung oder mit dem Internet und Computern empfohlen.

Sie können Prestabox über diese Adresse aufrufen: [http://www.prestabox.com/](http://www.prestabox.com/)

#### Technische Vorraussetzungen  <a href="#wasfuerdieinstallationbenoetigtwird-technischevorraussetzungen" id="wasfuerdieinstallationbenoetigtwird-technischevorraussetzungen"></a>

Prestashop ist ein, auf einem Webserver laufendes Programm und wurde in der Programmiersprache PHP geschrieben. Daten werden auf einem MySQL-Server gespeichert.

PHP is eine open-source Programmiersprache, die Hauptsächlich für Web-Applikationen benutzt wird. Seit der Entstehung 1995 ist PHP die von Web-Entwicklern meistbenutzte Programmiersprache geworden. Der Syntax ist an die Sprache C angelehnt, was Entwickerln das lernen leicht macht.

MySQL ist ein open-source Datenbankmanagementsystem. Auch 1995 enstanden, wurde MySQL das quasi-standard Datenbanksystem für Webentwickler. Es basiert auf der SQL Sprache, der gängigsten Datenbanksprache.

Egal welchen Hoster Sie wählen, folgende Komponenten müssen auf Ihrem Webserver installiert sein:

* **System**: Unix, Linux oder Windows. Unix wird empfohlen.
* **Web server**: Apache Web server 1.3 oder höher.
* **PHP 5.2 oder höher**. You may have to activate PHP 5. Möglicherweise müssen Sie PHP erst aktivieren (fragen Sie ihren Hosting Provider).
* **MySQL 5.0** **oder höher**.
* Mindestens 64 Mb RAM auf Ihrem Server(je mehr, desto besser).\
  \


PrestaShop funktioniert auch mit Microsoft's IIS Web server 6.0 oder höher und nginx 1.0 oder höher.

Mehr Informationen für Systemadministratoren finden Sie im [System Administrators Guide](http://doc.prestashop.com/display/PS15/System+Administrator+Guide).

#### Werkzeuge <a href="#wasfuerdieinstallationbenoetigtwird-werkzeuge" id="wasfuerdieinstallationbenoetigtwird-werkzeuge"></a>

Sie benötigen zwei Werkzeuge: Einen Texteditor, um Textdateien zu bearbeiten, und einen FTP Client, um Dateien von ihrem PC an einen Webserver zu senden und umgekehrt.

**Texteditor**

Hier eine Auflistung von bekannten Texteditoren:

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

Benutzen Sie kein Textverarbeitungsprogramm, wie Microsoft Word oder OpenOffice.

**FTP Client**

FTP steht für "File Transfer Protocol", die Standardmethode, um Dateien an einen Web-Host zu senden.

In dieser Anleitung wird Filezilla benutzt, ein kostenloser FTP Client für Windows, Mac OS X und Linux. Laden Sie ihn von [http://filezilla-project.org/](http://filezilla-project.org/)  herunter und Starten den Installer. Achtung: Downloaden Sie nur den Client, nicht den Server!

Nach der Installation müssen Sie den Client mit den Verbindungsparametern versehen, die Sie von Ihrem Host erhalten haben sollten, wenn nicht, fragen Sie nach oder durchsuchen Sie ihren Spam-Ordner.

Folgende Parameter werden gebraucht:

* **ein hostname** oder **eine IP Adress**e: Der Standort des FTP-Servers ihres Hosters
* **ein Benutzername**: zur Identifizierung ihres Hosting-Accounts
* **ein Passwort**: zur Sicherung vor unbefugten Zugriffen.

Öffnen Sie FileZilla und navigieren zum Site Manager Tool. Das funktioniert auf drei verschiedene Arten:

* Drücken Sie Ctrl-S,
* Klicken Sie den "Open the Site Manager" icon, oben links,
* Öffnen Sie das  "File"-Menü und wählen die "Site Manager..."-Option.

Ein neues Fenster wird sich öffnen.

Um ihren Web-Speicher hinzuzufügen:

1. Klicken Sie auf den "New Site" Button. Es wird ein neuer Eintrag in der Site List angelegt. Geben Sie ihm einen eindeutigen Namen. Auf der rechten Seite, im "General" Tab, tragen Sie die Parameter ein: host, user, password. Lassen Sie die anderen Parameter bei ihren Standardwerten, außer ihr Hoster gibt explizite Angaben dazu.
2. Wenn alle Felder richtig ausgefüllt wurden, klicken Sie auf den "Connect" Button. Dieser Schritt Speichert Ihren Eintrag in der Liste und loggt Ihren Account ein, um zu prüfen, ob alles funktioniert.

Wenn Ihnen FileZilla nicht gefällt, gibt es einige Alternativen:

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

#### Planung <a href="#wasfuerdieinstallationbenoetigtwird-planung" id="wasfuerdieinstallationbenoetigtwird-planung"></a>

Sie sollten vorher entscheiden, wo Sie PrestaShop hosten wollen. Bezogen auf den Domain-Namen gibt es vier Möglichkeiten:

* An der Wurzel der Domain: [http://www.example.com/](http://www.example.com/)
* In einem Ordner: [http://www.example.com/shop/](http://www.example.com/shop/)
* In einer Sub-domain: [http://store.example.com/](http://store.example.com/)
* In einem Ordner einer Sub-domain: [http://clothes.example.com/boutique/](http://clothes.example.com/boutique/)

Dank dem Multistore-Feature können Sie so Viele Shops mit einer einzigen installation von PrestaShop 1.6 haben, wie Sie benötigen, auch jeden mit eigenem Domain-Namen, wenn nötig. Sie sollten diese Möglichkeit bei der Strukturierung berücksichtigen.

Egal was Sie planen, der Standard Shop wird immer da sein, wo das PrestaShop-Verzeichnis ist.

#### PrestaShop installieren <a href="#wasfuerdieinstallationbenoetigtwird-prestashopinstallieren" id="wasfuerdieinstallationbenoetigtwird-prestashopinstallieren"></a>

Nun, da alle Vorbereitungen getroffen wurden, können sie zur Installations-Anleitung fortfahren: [Installing PrestaShop](http://doc.prestashop.com/display/PS16/Installing+PrestaShop).
