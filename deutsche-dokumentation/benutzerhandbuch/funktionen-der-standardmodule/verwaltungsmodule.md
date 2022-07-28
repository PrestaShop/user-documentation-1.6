# Verwaltungsmodule

/\*\<!\[CDATA\[\*/\
div.rbtoc1597071535452 {padding: 0px;}\
div.rbtoc1597071535452 ul {list-style: disc;margin-left: 0px;}\
div.rbtoc1597071535452 li {margin-left: 0px;padding-left: 0px;}\
\
/\*]]>\*/

* [Verwaltung](verwaltungsmodule.md#Verwaltungsmodule-Verwaltung)
  * [1-Click Upgrade - AutoUpgrade](verwaltungsmodule.md#Verwaltungsmodule-1-ClickUpgrade-AutoUpgrade)
  * [Europäische Rechtssicherheit](verwaltungsmodule.md#Verwaltungsmodule-EuropäischeRechtssicherheit)
    * [Label-Optionen](verwaltungsmodule.md#Verwaltungsmodule-Label-Optionen)
    * [Funktionen](verwaltungsmodule.md#Verwaltungsmodule-Funktionen)
    * [Verwaltung rechtskonformer Inhalte](verwaltungsmodule.md#Verwaltungsmodule-VerwaltungrechtskonformerInhalte)
    * [Zusätzlich E-Mail-Inhalte](verwaltungsmodule.md#Verwaltungsmodule-ZusätzlichE-Mail-Inhalte)
  * [Cron Tasks Verwaltung](verwaltungsmodule.md#Verwaltungsmodule-CronTasksVerwaltung)
  * [CSV-Export für Newsletter (zu finden im Modul „Block Newsletter“)](verwaltungsmodule.md#Verwaltungsmodule-CSV-ExportfürNewsletter\(zufindenimModul„BlockNewsletter“\))
    * [Abonnenten Exportieren](verwaltungsmodule.md#Verwaltungsmodule-AbonnentenExportieren)
    * [Kunden exportieren](verwaltungsmodule.md#Verwaltungsmodule-Kundenexportieren)
  * [PrestaShop Cleaner](verwaltungsmodule.md#Verwaltungsmodule-PrestaShopCleaner)
  * [Mailalerts](verwaltungsmodule.md#Verwaltungsmodule-Mailalerts)
    * [Customer notifications](verwaltungsmodule.md#Verwaltungsmodule-Customernotifications)
    * [Merchant notifications](verwaltungsmodule.md#Verwaltungsmodule-Merchantnotifications)
  * [Google Analytics API](verwaltungsmodule.md#Verwaltungsmodule-GoogleAnalyticsAPI)
  * [Watermark](verwaltungsmodule.md#Verwaltungsmodule-Watermark)
  * [Handelserfolg](verwaltungsmodule.md#Verwaltungsmodule-Handelserfolg)
  * [NVD3 Charts](verwaltungsmodule.md#Verwaltungsmodule-NVD3Charts)
  * [Erste Schritte](verwaltungsmodule.md#Verwaltungsmodule-ErsteSchritte)
  * [Einfache HTML-Tabelle](verwaltungsmodule.md#Verwaltungsmodule-EinfacheHTML-Tabelle)

## 1-Click Upgrade - AutoUpgrade <a href="#verwaltungsmodule-1-clickupgrade-autoupgrade" id="verwaltungsmodule-1-clickupgrade-autoupgrade"></a>

Dieses Modul macht es wirklich einfach PrestaShop auf die neueste Version zu aktualisieren.

Siehe das Kapitel "Automatic Update" des Handbuchs "Updating PrestaShop" (noch nicht in Deutsch verfügbar) für mehr Informationen: [Automatic update](http://doc.prestashop.com/display/PS16/Automatic+update).

## Europäische Rechtssicherheit <a href="#verwaltungsmodule-europaeischerechtssicherheit" id="verwaltungsmodule-europaeischerechtssicherheit"></a>

Neu in PrestaShop 1.6.1.0.

Das Modul „Europäische Rechtssicherheit“ hilft Händlern, ihre Shops den neuesten EU-Vorschriften anzupassen.

Dies ist must-have-Modul für europäische Shops.

Die meisten Optionen dieses Moduls sollen mit den folgenden Optionen mehr Transparenz für die Kunden zur Verfügung stellen:

* Ausführlichere Preisanzeigen( "Ab"-Preis, Steuern, Versandkosten und Lieferverzögerungen, Produktgewicht, etc.)
* One-Page-Checkout (erweiterter Checkout durch zusätzliche Informationen)
* Rechtsinhalt im Anhang bei E-Mails

Nicht alle der Option sind in allen Ländern nützlich, aber sie alle helfen, Ihren Shop den EU-E-Commerce-Gesetzen besser anzupassen.\
Die Standardeinstellungen sind die empfohlenen Einstellungen; es liegt an Ihnen, die Funktionen Ihrer Ansicht nach zu aktivieren oder zu deaktivieren.

### Label-Optionen <a href="#verwaltungsmodule-label-optionen" id="verwaltungsmodule-label-optionen"></a>

Stellen Sie sicher, alle Textfelder in alle verfügbaren Sprachen zu übersetzen.

* **Lieferzeit (auf Lager)**. Gibt die geschätzte Lieferzeit für Ihre Artikel auf Lager an. Lassen Sie das Feld leer, um die Option zu deaktivieren. Standard-Text hierfür ist "Lieferzeit: 1-2 Werktage".
* **Lieferzeit (nicht vorrätig)**. Gibt die geschätzte Lieferzeit für Ihre nicht vorrätigen Artikel an. Lassen Sie das Feld leer, um die Option zu deaktivieren. Standard-Text ist "Lieferzeit: 7-10 Werktage".
* **Anzeige Streichpreis**. Wenn ein Artikel im Angebot ist, wird der vorherige Preis durchgestrichen angezeigt.
* **Anzeige MwSt.**. Zeigt neben dem Artikelpreis an, ob die Steuer enthalten ist (zzgl./inkl. MwSt.).
* **Anzeige Versandkosten**. Zeigt neben dem Artikelpreis an, ob die Versandkosten im Preis inbegriffen sind.\
  Stellen Sie sicher, dass die Option "Versand und Zahlung" mit einer CMS-Seite im Abschnitt "Verwaltung rechtskonformer Inhalte" weiter unten im Formular verbunden ist, wenn Sie diese Option aktivieren. Das Label wird dann auf diese Inhalte weiterleiten.
* **Anzeige Gewicht**. Zeigt das Gewicht eines Artikels(wenn die Information verfügbar ist und der Artikel mehr als 1 kg wiegt).
* **Dezimalstellen Gewicht**. Legt fest, wie präzise das Gewicht angezeigt wird(z.B.: 1 kg / 1,01 kg). Der Wert kann nicht negativ sein.
* **Widerrufsrecht in den AGB**. Bezieht das Widerrufsrecht in den Inhalt der CMS-Seite "Allgemeine Geschäftsbedingungen" (AGB) ein.\
  Stellen Sie sicher, dass die Option "Allgemeine Geschäftsbedingungen" mit einer CMS-Seite im Abschnitt "Verwaltung rechtskonformer Inhalte" weiter unten im Formular verbunden ist. Das Label wird dann auf diese Inhalte verknüpfen.
* **Widerrufsrecht für virtuelle Artikel**. Fügt eine unumgehbare Checkbox ein, wenn der Warenkorb einen virtuellen Artikel enthält. Verwenden Sie diese Option um sicherzustellen, damit Kunden bewusst ist, dass ein virtueller Artikel nicht zurückgegeben werden kann.
* **"Ab Preis"-Anzeige (falls Varianten vorhanden)**. Zeigt eine "Ab"-Anzeige vor dem Preis bei Artikeln mit Varianten. Da die Preise von einer Variante zur anderen unterschiedlich sein können, zeigt diese Anzeige, dass der Endpreis höher sein kann.
* **Freitext 1 (über Bestellübersicht)**. Fügt einen benutzerdefinierten Text über der Bestellübersicht ein.
* **Freitext 2 (unter Bestellübersicht)**. Fügt einen benutzerdefinierten Text am unteren Rand der Bestellübersicht ein.

### Funktionen <a href="#verwaltungsmodule-funktionen" id="verwaltungsmodule-funktionen"></a>

* **Aktiviere "An einen Freund senden"**. Wenn diese Option aktiviert ist, kann ein Kunde eine E-Mail an einen Freund mit dem Link zu einer Artikelseite senden.\
  Diese Option setzt voraus, dass sie auch Ihrer lokalen Gesetzgebung entspricht, bevor Sie sie aktivieren: die E-Mails von dieser Funktion gesendet werden, können als unerwünschte kommerzielle E-Mails interpretiert werden.
* **Aktiviere „Nachbestellen“**. Wenn diese Option aktiviert ist, kann ein Kunde einen Artikel mit einem einzigen Klick auf seiner Bestellhistorie neu bestellen.\
  Diese Option setzt voraus, dass sie auch Ihrer lokalen Gesetzgebung entspricht, bevor Sie sie aktivieren: Dies kann als unaufgefordert zugesandte Ware angesehen werden.
* **Aktiviere One-Page-Checkout**. Ersetzt den Standard Bestellprozess mit einem gesetzlich  konformeren (natürlich EU-bezogen). Diese Option funktioniert nur mit dem Standard-Bootstrap-Vorlage oder einer anderen kompatiblen Vorlage und mit kompatiblen Zahlungsmethoden (viele Module wurden bereits daran angepasst).\
  Sobald die Option aktiviert wird, zeigt die neue One-Page-Checkout-Seite die folgenden Abschnitte: Zahlungsmöglichkeiten, Adresse(n), Allgemeine Geschäftsbedingungen, eine Bestellübersicht und den Button „Zahlungspflichtig bestellen“.
* **Anteiliger Steuersatz auf Versand und Verpackung**. Anstatt Versanddiensten und Geschenkverpackung Steuerregeln zuzuordnen,  kann die durchschnittliche Steuer auf Artikel im Warenkorb berechnet und verwendet werden, um die Steuer von Geschenkverpackung und Versand zu berechnen. Dies ist sehr nützlich in Deutschland.\
  Wenn aktiviert, werden die Steuern für Versand und Verpackung im Verhältnis zu den Steuern auf die Artikel im Warenkorb berechnet.\
  Im Endeffekt bedeutet dies, dass der Kunde am Anfang der Bestellung einen "mit Steuer"-Preis am angezeigt bekommt, Steuern auf Versand und Verpackung werden beim Bestellprozess dazu addiert und auf Ihre Marge berechnet.

### Verwaltung rechtskonformer Inhalte <a href="#verwaltungsmodule-verwaltungrechtskonformerinhalte" id="verwaltungsmodule-verwaltungrechtskonformerinhalte"></a>

Einige Optionen dieses Moduls müssen vom System "wissen", wofür einige CMS-Seiten da sind. Wenn keine Seite für einige benötigte Punkte zur Verfügung steht, dann müssen Sie diese noch erstellen.

### Zusätzlich E-Mail-Inhalte <a href="#verwaltungsmodule-zusaetzliche-mail-inhalte" id="verwaltungsmodule-zusaetzliche-mail-inhalte"></a>

Mit dieser Schnittstelle können Sie festlegen, welche Dokumente am Footer jeder E-Mail des Shops mitgesendet werden sollen - zum Beispiel können die allgemeinen Geschäftsbedingungen am Footer aller Rechnungen angebracht werden.

Der Inhalt wird von den Einstellungen in "Verwaltung rechtskonformer Inhalte" dieses Modul festgelegt. Wenn keine Option gesetzt ist, können Sie keinen Inhalt zum senden auswählen.

## Cron Tasks Verwaltung <a href="#verwaltungsmodule-crontasksverwaltung" id="verwaltungsmodule-crontasksverwaltung"></a>

Dieses Modul funktioniert wie ein Cron-Tool: Sie können hier wiederkehrende Aufgaben mit sicheren URLs als Cronjobs anlegen (z.B. regelmäßige Updates oder andere häufig anfallende Aufgaben).

## CSV-Export für Newsletter (zu finden im Modul „Block Newsletter“) <a href="#verwaltungsmodule-csv-exportfuernewsletter-zufindenimmodul-blocknewsletter" id="verwaltungsmodule-csv-exportfuernewsletter-zufindenimmodul-blocknewsletter"></a>

Diese Funktion wurde geschrieben, um eine CSV-Datei der E-Mail-Adressen zu exportieren, unter denen Ihre Kunden in Ihrem System registriert sind.

Ihre Kunden können Ihnen ihre E-Mail-Adresse geben, indem Sie sie entweder im Newsletter-Block eintragen, oder bei der Registrierung ankreuzen, dass sie einen Newsletter erhalten möchten. Sie brauchen diese E-Mail-Adressen, um Marketing zu betreiben.\
Bei der Registrierung haben Ihre Kunden zwei Möglichkeiten, welche Newsletter Sie erhalten: Die erste Option, das normale Abonnieren eines Newsletters, die zweite zum Erhalten Angeboten Ihrer Partner (Opt-In).

### Abonnenten Exportieren <a href="#verwaltungsmodule-abonnentenexportieren" id="verwaltungsmodule-abonnentenexportieren"></a>

Im ersten Abschnitt können Sie alle E-Mail-Adressen exportieren, die Ihrem Shop zur Verfügung stehen. Nach einem Klick auf den Button ".CSV-Datei exportieren", wird eine Meldung mit einem Link angezeigt, auf den Sie klicken können, um die Datei herunterzuladen, die die Adressen enthält.

Vier Informationen werden in dieser Datei vorhanden sein: Die Kundennummer, E-Mail-Adresse, der Tag der Registrierung und die IP-Adresse. Wenn Sie diese Daten mit einer Software wie Microsoft Excel verwenden, können Sie die Informationen sortieren, wie Sie möchten.

### Kunden exportieren <a href="#verwaltungsmodule-kundenexportieren" id="verwaltungsmodule-kundenexportieren"></a>

In diesem Abschnitt können Sie die Adressen Ihrer Kunden filtern, bevor Sie eine CVS-Datei ihrer Daten exportieren. Zum ist das Filtern nach Land besonders nützlich, wenn Sie Newsletter immer in der richtigen Sprache und zur Anpassung Ihrer Angebote senden möchten.

Sie berücksichtigen daher mehr Informationen, wenn Sie E-Mail-Adressen exportieren. Benutzen Sie das Dropdown-Menü "Newsletter-Abonnenten", um eine der folgenden drei Optionen auszuwählen:

* **Alle Abonnenten**. Ermöglicht es Ihnen, alle E-Mail-Adressen Ihrer Kunden zu wählen, die ein Konto auf Ihren Shop öffnen. Das heißt, diejenigen, die Informationen von Ihrer Seite erhalten möchten, als auch diejenigen, die dies nicht tun. Seien Sie vorsichtig, was Sie mit ihm getan hat, dann.
* **Abonnenten**. Ermöglicht es Ihnen, nur die Kunden zu wählen, die einen Newsletter von Ihnen erhalten wollen.
* **Nicht-Abonnenten**. Ermöglicht es Ihnen, nur die Kunden zu wählen, die keinen Newsletter von Ihnen erhalten wollen.

Das nächste Dropdown-Menü "Partnerangebote akzeptiert" ist dafür zuständig, Adressen der Kunden zu filtern, die Angebote von Ihren Partnern erhalten möchten. Hier gibt es wieder drei ähnliche Optionen:

* **Alle Kunden**. Ermöglicht es Ihnen, alle E-Mail-Adressen Ihrer Kunden zu wählen, die ein Konto in Ihrem Shop haben. Das heißt, sowohl diejenigen, die Newsletter wollen, und diejenigen, die keine wollen.
* **Partnerangebote akzeptiert**. Ermöglicht es Ihnen, nur die Kunden zu wählen, die einen Newsletter von Ihren Partnern erhalten wollen.
* **Partnerangebote nicht akzeptiert**. Ermöglicht es Ihnen, nur die Kunden zu wählen, die keinen Newsletter von Ihren Partnern erhalten wollen.

Sobald Sie die E-Mail-Adressen gefiltert wurden, können Sie diese exportieren, indem sie auf den Button ".CSV-Datei exportieren" klicken, um die gewählten Adressen dann herunterzuladen. Eine Meldung erscheint, in der Sie auf die Datei klicken und diese somit herunterladen können. Diese Datei enthält sechs Arten von Informationen: die Kunden-ID, Nachname, Vorname, E-Mail-Adresse, IP-Adresse und das Datum der Anmeldung. Sie können dann diese Informationen benutzen, um Ihre Marketing-Kampagnen zu senden.

## PrestaShop Cleaner <a href="#verwaltungsmodule-prestashopcleaner" id="verwaltungsmodule-prestashopcleaner"></a>

Dieses Modul ist sehr nützlich, wenn Sie mit der Erkundung und dem Lernen von PrestaShop fertig sind und nun bereit sind, Ihre eigenen Inhalte hochzuladen und Ihren Shop zu starten: Sie müssen zuerst alle Demo-Daten entfernen, die zusammen mit PrestaShop installiert wurden: Artikel, Kategorien, Kunden, Bestellungen, etc.

Die Konfigurationsseite besteht aus drei Abschnitten:

* **Katalog**. Dadurch werden alle Daten aus dem aktuellen Katalog gelöscht, auch die Elemente, die Sie selbst hinzugefügt haben. Aktivieren Sie das Feld und klicken Sie auf "Delete catalog", um den Vorgang zu starten.
* **Orders and Customers**. Diese Option löscht alle aktuell registrierten Bestellungen und Kunden, auch diejenigen, die Sie selbst erstellt haben. Aktivieren Sie das Feld und klicken Sie auf "Delete orders & customers", um den Vorgang zu starten.
* **Functional integrity constraints**. Dies wird Ihre Datenbank überprüfen und sicherstellen, dass alles richtig eingestellt ist und versucht, Dinge zu reparieren, die nicht richtig eingestellt sind.
* **Database Cleaning**. Dies hilft, Speicherplatz zu reduzieren und Plattenzugriffseffizienz zu verbessern.

**Seien Sie sehr vorsichtig**: jede Aktion, die durch diese Buttons verursacht wird, kann nicht rückgängig gemacht werden. Achten Sie darauf, eine aktuelle Sicherungskopie Ihrer Datenbank zur Verfügung zu haben.

## Mailalerts <a href="#verwaltungsmodule-mailalerts" id="verwaltungsmodule-mailalerts"></a>

PrestaShop ermöglicht es Ihnen, Sie und Ihre Kunden per E-Mail in bestimmten Fällen zu benachrichtigen:

* Ihre Kunden: wenn ein Artikel ausverkauft ist.
* Sie: wenn eine neue Bestellung aufgegeben wurde.
* Sie: Wenn der Lagerbestand eines Artikels unter einem bestimmten Schwellenwert liegt.
* Sie: Wenn die Abdeckung des Lagerbestands des Artikels unter einer bestimmten Anzahl von Tagen liegt.

### Customer notifications <a href="#verwaltungsmodule-customernotifications" id="verwaltungsmodule-customernotifications"></a>

Es gibt nur eine Einstellung in diesem Abschnitt:

* **Product availability**. Wenn Sie diese Einstellung aktivieren, erscheint ein Feld auf der Produktseite Ihres Shops, wenn das Produkt ausverkauft ist. Es fragt Ihren Kunden nach seinen Kontaktinformationen, um ihn zu kontaktieren, wenn der Artikel wieder auf Lager verfügbar ist.

### Merchant notifications <a href="#verwaltungsmodule-merchantnotifications" id="verwaltungsmodule-merchantnotifications"></a>

Es gibt verschiedene Einstellungen für Händler:

* **New order**. Aktivieren Sie diese Einstellung, wenn Sie bei jeder neuen Bestellung benachrichtigt werden möchten.
* **Ausverkauft**. Aktivieren Sie diese Einstellung und stellen Sie das "Threshold"-Feld auf den Wert, bei dem Sie benachrichtigt werden möchten(Standard ist 3).
* **Coverage warning**. Aktivieren Sie diese Einstellung und tragen Sie im Feld "Coverage“ den Wert ein, bei dem Sie benachrichtigt werden möchten(Standard: 0).

Händler-Mail-Benachrichtigungen können gleichzeitig an mehrere Adressen gesendet werden. Tragen Sie jede Adresse einfach in das Textfeld ein(eine Adresse pro Zeile).

## Google Analytics API <a href="#verwaltungsmodule-googleanalyticsapi" id="verwaltungsmodule-googleanalyticsapi"></a>

Dieses Modul ermöglicht es Ihnen, Ihren PrestaShop mit Ihrem Google Analytics-Konto zu verknüpfen.

Zunächst müssen Sie die API-Version, die Sie verwenden möchten, wählen:

* Bei Version 1.3 benötigen Sie Ihre Google Analytics E-Mail-Adresse, Passwort und Profil.
* In der Version 3.0 benötigen Sie Ihre Google Analytics-Client-ID, Client-Schlüssel und Profil.

Wir empfehlen 3.0 ein, da 1.3 veraltet ist. Um die Version 3.0 nutzen zu können, müssen Sie OAuth-Zugriff aktivieren, indem Sie folgende Anweisungen ausführen: [https://developers.google.com/analytics/devguides/config/mgmt/v3/mgmtAuthorization](https://developers.google.com/analytics/devguides/config/mgmt/v3/mgmtAuthorization)

## Watermark <a href="#verwaltungsmodule-watermark" id="verwaltungsmodule-watermark"></a>

Dieses Modul ermöglicht es Ihnen, ein Wasserzeichen über alle Artikelbilder Ihres Shops zu legen. Dies schränkt ihre Nutzung im Internet ein – und hält hoffentlich auch Menschen davon ab, sie zu stehlen.

Wenn Sie Ihre Artikel in Google Shopping exportieren möchten, sollten Sie wissen, dass die Verwendung von Werbetext / Logos und Wasserzeichen in den Bildern nicht erlaubt ist. Sie können nur Bilder hochladen, die frei von zusätzlichen Wasserzeichen / Logos sind.\
Erfahren Sie mehr über die Google-Shopping-Richtlinien hier: [https://support.google.com/merchants/answer/2700371?hl=en\&ref\_topic=2701481](https://support.google.com/merchants/answer/2700371?hl=en\&ref\_topic=2701481)

Die Konfigurationsseite informiert Sie sofort, welche Einstellungen noch fehlen.

* Watermark file. Das gewählte Bild muss im GIF-Format sein.
* Watermark opacity(1-100). 100 beläuft sich auf ein nicht-transparentes Bild, was bedeutet, dass das Logo gut sichtbar sein wird, aber auch vollständig Teile des ganzen Bildes verdeckt. Die Standardeinstellung, 60, ist in der Regel ein guter Kompromiss.
* &#x20;Watermark X align. Wählen Sie, wo das Wasserzeichen in jedem Ihrer Bilder, hier auf der horizontalen Achse, angezeigt werden soll.
* Watermark Y align. Wählen Sie, wo das Wasserzeichen in jedem Ihrer Bilder, hier auf der vertikalen Achse, angezeigt werden soll.
* Choose image types for watermark protection. Die Bildtypen, auf die das Wasserzeichen aufgebracht werden soll. Sie müssen wirklich nur die größten Größen zu wählen, da diese am ehesten gestohlen werden.

Nachdem Sie Ihre Einstellungen gespeichert haben ist die Konfiguration abgeschlossen, aber die Wasserzeichen sind noch nicht hinzugefügt. Navigieren Sie zum Menü "Voreinstellungen" und öffnen Sie die Seite "Bilder". Dort klicken Sie auf "Wiederherstellen der Vorschaubilder" am unteren Rand der Seite. PrestaShop bearbeitet nun alle Ihre Bilder (wie in der Konfiguration ausgewählt), und die Wasserzeichen werden auf die ausgewählten Bildergrößen angewendet.

## Handelserfolg <a href="#verwaltungsmodule-handelserfolg" id="verwaltungsmodule-handelserfolg"></a>

Dieses Modul wurde speziell für PrestaShop Benutzer entworfen, damit diese ihre Fortschritte als Online-Händler einsehen, wie stark sie gewachsen sind, sowie Fortschritte im Laufe der Tage, Monate und Jahre. Das Modul wird standardmäßig installiert.

Dieses Modul fügt ein System von Abzeichen und Punkte ein, die sich auf drei Ebenen aufteilen, von denen alle in der E-Commerce-Welt für Ihren Erfolg wichtig sind:

* **Maßnahmen**. Dokumentiert Ihre Verwendung von wichtigen E-Commerce-Funktionen wie Site-Performance, Katalog-Größe, Mitarbeiter und SEO.
* **Erreichte Ziele**. Verfolgt Ihren Abschluss von bestimmten Schlüssel-E-Commerce-Zielen, wie die Anzahl der Kunden, Bestellungen und den Umsatz.
* **International**. Verfolgt Ihre Präsenz in wichtigen internationalen Märkten wie Nord- und Südamerika, Ozeanien, Asien, Europa, Afrika und Maghreb.

Je mehr Fortschritte Ihr Geschäft macht, desto mehr Abzeichen und Punkte verdienen Sie.\
Es besteht keine Notwendigkeit, alle Informationen vorzulegen oder irgendwelche Formulare auszufüllen. Wir wissen, wie beschäftigt Sie sind; alles geschieht automatisch. Mit diesem Tool können Sie die wichtigsten Aspekte Ihres Shops einsehen, Ihre Fortschritte betrachten und sich noch einmal an große Erfolge erinnern.

## NVD3 Charts <a href="#verwaltungsmodule-nvd3charts" id="verwaltungsmodule-nvd3charts"></a>

NVD3 ([http://nvd3.org/](http://nvd3.org/)) ist eine JavaScript-Bibliothek, die speziell zum Darstellen von schönen Diagrammen mit D3.js ([http://d3js.org/](http://d3js.org/)) entworfen wurde, es ist eine Bibliothek zur Datenmanipulation.

Dieses Modul macht es Ihnen möglich, NVD3 Charting-Code für eigene Anwendungen und Diagramme zu nutzen.

## Erste Schritte <a href="#verwaltungsmodule-ersteschritte" id="verwaltungsmodule-ersteschritte"></a>

Das Erste-Schritte-Modul empfängt Erstanwender in ihrem Backoffice in PrestaShop: durch eine kleine spielerische Schnittstelle zeigt es dem Benutzer, wie er / sie sein / ihr Geschäft in mehreren Schritten an den Start bringt.

## Einfache HTML-Tabelle <a href="#verwaltungsmodule-einfachehtml-tabelle" id="verwaltungsmodule-einfachehtml-tabelle"></a>

Ermöglicht, die Statistiken in einer HTML-Tabelle anzuzeigen.
