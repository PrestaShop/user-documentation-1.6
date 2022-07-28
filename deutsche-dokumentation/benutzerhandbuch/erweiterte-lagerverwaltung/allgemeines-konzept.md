# Allgemeines Konzept

## Allgemeines Konzept <a href="#allgemeineskonzept-allgemeineskonzept" id="allgemeineskonzept-allgemeineskonzept"></a>

Um Verwechslungen mit der klassischen Lagerverwaltungsfunktion der Version 1.4 von PrestaShop zu vermeiden und die Möglichkeiten der erweiterten Lagerverwaltung seit Version 1.5 zu sehen, sollten Sie zwei Konzepte unterschieden: Bestandsverwaltung und erweiterte Lagerverwaltung.

### Bestandsverwaltung <a href="#allgemeineskonzept-bestandsverwaltung" id="allgemeineskonzept-bestandsverwaltung"></a>

Dies ist wie die Lager-Management-Funktion von PrestaShop 1.4x Es ist die Produktmenge, die im Shop für jeden Artikel und jede Artikelvariante angezeigt wird. Das ist die Menge, die festlegt, ob ein Artikel bestellt werden kann oder nicht (es sei denn, die Option "Bestellung von Artikeln ohne Bestand" ist aktiviert). Diese Menge kann manuell für jeden Artikel und jede Artikelvariante geändert werden.

Seit PrestaShop 1.5.x, kann diese Menge automatisch entsprechend dem physischen Bestand des betroffenen Artikels eingestellt werden. Bei mehreren Shops ist die Menge für jeden Shop festzulegen.

Was folglich früher in PrestaShop 1.4.x "Lager" genannt wurde, wird seit PrestaShop 1.5.x  als "Bestandsverwaltung" deklariert.

### Erweiterte Lagerverwaltung <a href="#allgemeineskonzept-erweitertelagerverwaltung" id="allgemeineskonzept-erweitertelagerverwaltung"></a>

Dies ist die physikalische Verwaltung von gelagerten Artikeln aus einem Lager (oder mehreren). Dies ist das neue Konzept "Erweiterte Lagerverwaltung", das in PrestaShop 1.5x eingeführt wurde.

Diese neue Lager-Management-Funktion beinhaltet Lagerbewegung, Lagerbestand, Umlagerung zwischen Lagerhallen, Integration in die Multishop-Funktion und Bestellauftragsmanagement.

Dies macht es auch möglich, den aktuellen Lagerbestand einzubeziehen. Manchmal kann ein Artikel physisch im Lager verfügbar sein, aber nicht zum Verkauf zur Verfügung stehen, weil einige Kundenbestellungen noch auf den Versand warten. Der gleiche Artikel kann auch wieder von einem Lieferanten bestellt worden sein, und wurde im physischen Bestand noch nicht berücksichtigt.

Physischer Bestand besteht deshalb aus Artikeln, die auch wirklich physisch im Lager existieren, zu dem wir die gegenwärtig bestellte Menge von Lieferanten hinzufügen, und von dem wir die Menge abziehen, die derzeit von Kunden bestellt, aber noch nicht verschickt worden.

## Die Lagerverwaltung nutzen <a href="#allgemeineskonzept-dielagerverwaltungnutzen" id="allgemeineskonzept-dielagerverwaltungnutzen"></a>

### Muss ich die neue Lagerverwaltung nutzen? <a href="#allgemeineskonzept-mussichdieneuelagerverwaltungnutzen" id="allgemeineskonzept-mussichdieneuelagerverwaltungnutzen"></a>

Sie müssen die neue Lagerverwaltung nicht verwenden, das gleiche gilt für "Lagerbestand".

Sie können beide Einstellungen aktivieren/deaktivieren, indem Sie zur Seite Voreinstellungen>Artikel navigieren und nach unten scrollen. Sie müssen zunächst Bestandsverwaltung aktivieren, um die erweiterte Lagerverwaltung aktivieren zu können.

Die Funktion „Erweiterte Lagerverwaltung“, oder auch die Bestandsverwaltung und Ihre Warenlager sind unabhängig von der Multishop-Funktion. Folglich ist es egal, welchen Shop Sie gerade verwalten,  wenn Sie Ihr Lager betrachten, das Lager wird immer global verwaltet.

### Ich will nicht meine ganzen Einstellungen von PrestaShop 1.4.x / 15.x ändern. Was kann ich tun? <a href="#allgemeineskonzept-ichwillnichtmeineganzeneinstellungenvonprestashop1.4.x-15.xaendern.waskannichtun" id="allgemeineskonzept-ichwillnichtmeineganzeneinstellungenvonprestashop1.4.x-15.xaendern.waskannichtun"></a>

Wenn Sie die neue fortschrittliche erweiterte Lagerverwaltung von PrestaShop 1.5 nicht verwenden möchten und mit der klassischen Methode einfach zufrieden sind, müssen Sie nur die alte Lagerverwaltung aktivieren, und nicht die erweiterte. gehen Sie auf die Voreinstellungsseite "Artikel", scrollen Sie zum Abschnitt "Artikel Lager", und wählen Sie "Ja" bei "Bestandsverwaltung aktivieren", und stellen Sie sicher, dass „Erweiterte Lagerverwaltung aktivieren“ auf „Nein“ steht.

Die "Lagerbestand"-Funktion ist nun in der "Mengen" Registerkarte jedes Artikels zentralisiert: Wenn Sie einen neuen Artikel erstellen oder einen vorhandenen bearbeiten steht der Tab "Mengen" auf der linken Seite zur Verfügung, neben anderen Tabs.

### Entspricht die neue erweiterte Lagerverwaltung meinen Bedürfnissen? <a href="#allgemeineskonzept-entsprichtdieneueerweitertelagerverwaltungmeinenbeduerfnissen" id="allgemeineskonzept-entsprichtdieneueerweitertelagerverwaltungmeinenbeduerfnissen"></a>

Die neue erweiterte Lagerverwaltung ermöglicht es Ihnen, eine Menge an Produkten zu verwalten. Diese Funktion hilft Ihrem Unternehmen, wenn:

* Sie einen Bestand von Artikeln verwalten, die Sie in Ihrem Shop verkaufen.
* Sie mindestens ein Lager(physisches Lagerhaus) verwenden, das Sie selbst verwalten.
* Sie die meisten oder alle Ihrer Artikel von einem oder mehreren Lieferanten bestellen.
* Sie Statistiken über den Zustand Ihres/er Lager/s und Lagerhauses/häuser führen.

Diese Funktion hilft Ihren Unternehmen nicht, wenn:

* Sie Ihren Produktbestand nicht selbst regeln.
* Sie bereits ein Lagerverwaltungssystem / Werkzeug / Programm verwenden, mit dem Sie zufrieden sind, und das Sie weiter fortführen möchten, ohne etwas zu ändern.
