# Module zu Versand & Logistik

## Carriercompare <a href="#modulezuversand-and-logistik-carriercompare" id="modulezuversand-and-logistik-carriercompare"></a>

Dieses Modul ermöglicht es dem Kunden, Lieferanten zu vergleichen, bevor der Bestellprozess fortgesetzt wird.

Dieses Modul ist sehr einfach aufgebaut: Installieren Sie es einfach, damit es Die Option im Front-Office angezeigt wird.

Für alle verfügbaren Lieferanten müssen die Gebühren korrekt eingestellt sein. Dies wird für jeden Versanddienste auf der Seite „Versand>Versanddienste“ individuell festgelegt, aufgeteilt auf Mehrwertsteuern, Spannen, Länder, und weitere Optionen.

Die Modulkonfigurationsseite hat nur eine Option, "How to refresh the carrier list?". Dies ermöglicht es Ihnen, Lieferanten nur anzuzeigen, wenn alle Informationen eingestellt sind, oder jederzeit.

## Dateofdelivery <a href="#modulezuversand-and-logistik-dateofdelivery" id="modulezuversand-and-logistik-dateofdelivery"></a>

Dieses Modul zeigt das ungefähre Datum der Lieferung am Ende der Bestellung.

Die Konfigurationsseite enthält zwei Abschnitte:

* **Link List**. Das Modul stützt sich auf Angaben Ihrer Versanddienste. Sie müssen daher Regeln für jeden Ihrer Versanddienste hinzufügen, indem Sie auf den Link "add a new carrier rule" klicken.
* **Settings**:
  * **Extra time when a product is out of stock**. Schätzen Sie die Zeit, die die es dauern könnte, bis Artikel wieder ab Lager verfügbar sind. Dies ist nur dann sinnvoll, wenn Kunden Artikel ohne Lagerbestand bestellen können(die Option hierfür ist auf der "Artikel"-Voreinstellungsseite im Abschnitt „Artikel Lager“).
  * **Extra time for preparation of the order**. Schätzen Sie die Zeit, die es voraussichtlich dauern wird, bis eine Bestellung vorbereitet wurde.
  * **Preparation option**. Wenn Ihr Versandteam am Wochenende arbeitet, kann dies hierdurch berücksichtigt werden.
  * **Date format**. Das Format, in dem der voraussichtliche Liefertermin angezeigt wird. Hier wird das PHP date () Format verwendet: jeder Buchstabe hat eine Bedeutung, dies wird unter dem darunter stehenden Link erklärt. Die Standardeinstellung "l j F Y" bedeutet, dass das Datum z.B. im Format "Samstag 21 Januar 2012" angezeigt wird. Es gibt viele weitere Einstellungen für das Datumsformat, die Sie auf Ihre Wünsche abstimmen können: siehe [http://www.php.net/manual/en/function.date.php](http://www.php.net/manual/en/function.date.php).

Eine neue Versanddienst-Regel zu erstellen ist sehr simpel:

* **Carrier**. Wählen Sie Versanddienst, für den Sie die Regel hinzufügen möchten. Wenn der gewünschte Versanddienst nicht vorhanden ist, müssen Sie ihn auf der Seite Versand>Versanddienste erstellen.
* **Delivery between**. Stellen Sie den Zeitraum ein, in dem der gewählte Versanddienst verspricht, Ihre Artikel zu liefern. Fragen Sie hier Ihren Versanddienst selbst nach diesen Informationen.
* **Delivery option**. Einige Versanddienste bereiten ihre Pakete am Wochenende vor, um sie gleich am Montagmorgen zu versenden. Stellen Sie sicher, dies zu kennzeichnen, wenn dieser Fall gegeben ist.

Sie sollten so viele Versanddienst-Regeln wie nötig erstellen.

## Fedex (fedexcarrier) <a href="#modulezuversand-and-logistik-fedex-fedexcarrier" id="modulezuversand-and-logistik-fedex-fedexcarrier"></a>

Bietet Ihren Kunden unterschiedliche Versandmethoden mit Fedex.

## Globkurier <a href="#modulezuversand-and-logistik-globkurier" id="modulezuversand-and-logistik-globkurier"></a>

Nur in Polen.

![](<../../../.gitbook/assets/23036725 (2).png>)

[GlobKurier.pl](http://globkurier.pl) ist einer der größten nationalen Versanddienste. Wir bieten nationale und internationale Dienstleistungen in mehr als 200 Ländern. Unsere Hauptziele sind konkurrenzfähige Preise, Geschwindigkeit und Sicherheit. Mit [GlobKurier.pl](http://globkurier.pl) können Sie sicher sein, dass Ihre Sendungen immer pünktlich ankommen. Darüber hinaus bieten wir Überzeugung in unsere Dienstleistungen.

## GoInterpay <a href="#modulezuversand-and-logistik-gointerpay" id="modulezuversand-and-logistik-gointerpay"></a>

![](<../../../.gitbook/assets/23038228 (2).png>)

Importieren Sie mehr als 200 Zahlungsmethoden mit einem einzigen Modul.

## Kiala Advanced (Nur für Vertragspartner von Kiala) <a href="#modulezuversand-and-logistik-kialaadvanced-nurfuervertragspartnervonkiala" id="modulezuversand-and-logistik-kialaadvanced-nurfuervertragspartnervonkiala"></a>

Dieses Modul ermöglicht es Ihren Kunden, ihre Artikel an eine Kiala Sammelstelle liefern zu lassen. Kiala-Sammelstellen sind in Frankreich und anderen ausgewählten europäischen Ländern weit verbreitet.

Sie müssen ein Kiala Konto haben, um dieses Modul verwenden zu können. Sie können hier zum Anmeldeformular navigieren: [http://www.kiala.com/](http://www.kiala.com/).\
Anschließend konfigurieren Sie das Modul mit allen Informationen über Sie und Ihren Shop im Abschnitt "Kiala-Modulstatus".\
Die "Ländereinstellungen" weiter unten hilft Ihnen bei der Anzeige, in welchen Ländern Sie Kiala Lieferung für Ihre Kunden erlauben möchten.\
Schließlich ergänzt "erweiterte Kiala-Einstellungen" den Abschnitt um ein paar weitere Optionen:

* **Export-Ordner**. Der lokale Ordner, in dem das Modul seine Exporte speichert, enthält viele nützliche Informationen.
* **Präfix für Bestell- und Paketnummer**. Sie können für Ihren Shop einen Shop-spezifischen Präfix haben, was für Ihre Kunden personalisierter wirkt.
* **Export bei jeder Bestellung ?**. Sie können entscheiden, ob Sie mehrere bestellungsspezifische Exportdateien haben möchten, anstatt eine große.
* **Parcel tracking criterion?**. Sollte das Paket auf einer Pro-Kunden oder Pro-Bestellung-Basis verfolgt werden? Wenn Sie unsicher sind, sollten Sie Pro-Bestellung auswählen.

Sobald die Einstellungen abgeschlossen sind, werden Kunden die "Kiala" Option im Front-Office sehen können.

## Tracking - Front office <a href="#modulezuversand-and-logistik-tracking-frontoffice" id="modulezuversand-and-logistik-tracking-frontoffice"></a>

Dieses Modul ergänzt PrestaShop um eine Affiliate-Programm-Funktion, die Ihren Partnern ermöglicht, auf eigene Statistiken zuzugreifen.

Das Affiliate-Programm-Tool auf der "Referrer" Seite befindet sich im Menü "Statistik". Sobald Sie "Tracking - Front-Office" installiert haben, können diese Partner auf ihre Statistiken zugreifen, indem Sie auf [http://www.ihreshopdomain.com/modules/trackingfront/stats.php](http://www.ihreshopdomain.com/modules/trackingfront/stats.php) navigieren.

Klicken Sie auf den „NEU“-Button, um einen neuen Partner zu erstellen und fügen Sie ihm Formular die Daten für Ihren Partner ein, tragen Sie die Gebühren ein, die sie pro Klick und pro Bestellung erhalten, sowie einen Prozentsatz des Umsatzes.

Klicken Sie auf den Button "Hilfe", um Anweisungen zu bekommen, wie Sie Referrer-URLs einrichten.

Der Abschnitt "Technische Informationen – Einfacher Modus" ermöglicht es Ihnen, reguläre Ausdrücke anstelle von Klartext-URLs zu verwenden.

## UPS <a href="#modulezuversand-and-logistik-ups" id="modulezuversand-and-logistik-ups"></a>

Bietet Ihren Kunden unterschiedliche Versandmethoden mit UPS

## USPS <a href="#modulezuversand-and-logistik-usps" id="modulezuversand-and-logistik-usps"></a>

Berechnet Versandkosten für die U.S.A. und den dortigen nationalen Versand.
