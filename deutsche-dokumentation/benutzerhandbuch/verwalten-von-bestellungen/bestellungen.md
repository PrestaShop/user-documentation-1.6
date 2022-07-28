# Bestellungen

Auf der "Bestellungen"-Seite im Menü "Bestellungen" können Sie alle Informationen über alle Bestellungen in Ihrem Shop sehen. Alle Transaktionen Ihres Shops stehen dort zur Verfügung, nach Datum sortiert (standardmäßig wird von neu nach alt sortiert).

Sie können die Ergebnisse leicht filtern, um die Bestellungen, die Sie suchen, zu finden. Ein Beispiel: um Mr. Doe zu finden, geben Sie "Doe" nach dem Klicken auf den Button „NEU“ ein und klicken Sie auf die Lupe am rechten Rand.

Sie können Bestellungen nicht löschen. Es ist illegal, Zahlungen, Bestellungsinformationen und / oder Rechnungsinformationen in Europa zu entfernen. Daher würde die Umsetzung einer Schaltfläche "Löschen" bei Bestellungen eine juristische Problemlage erzeugen.

Um eine Standard-Bestellung sicher löschen zu können, installieren Sie das "Database Cleaner"-Modul (seit Standardinstallation v1.5.4 verfügbar), öffnen das Konfigurationsfenster und überprüfen die "Aufträge und Kunden"-Box, bevor Sie auf den "Bestellungen und Kunden löschen"-Button klicken.

Sie können eine Liste Ihrer Bestellungen exportieren, indem Sie auf den "Export"-Button oben klicken.\
Sie können keine Bestellungen importieren.

## Bestellungen anlegen <a href="#bestellungen-bestellungenanlegen" id="bestellungen-bestellungenanlegen"></a>

Eines der herausragenden Merkmale von PrestaShop ist die Möglichkeit, eine Bestellung direkt aus dem Back-Office zu erstellen. Zum Beispiel ist dies enorm hilfreich, wenn ein Kunde einen Artikel kaufen will, aber dabei nicht erfolgreich ist, und eine Bestellung während eines Telefongesprächs oder in einer E-Mail-Konversation aufgibt.

Durch Klicken auf "NEU" öffnet sich eine neue Seite mit einem einzelnen Textfeld mit der Bezeichnung " Kunden suchen". Beim Anlegen einer neuen Bestellung über das Backoffice ist Ihre erste Aufgabe, den Auftrag einem Kunden zuzuordnen. Geben Sie die ersten Buchstaben des Kundenvornamens, -Namens oder seiner E-Mail-Adresse ein und PrestaShop zeigt Ihnen die passenden Konten an.

Wenn der Kunde, dem Sie eine Bestellung zuordnen wollen, noch keine Daten hinterlegt hat, können Sie sofort neue Daten erzeugen: Klicken Sie auf den "Neuen Kunden hinzufügen"-Button, um ein Fenster zu öffnen, in dem Sie alle relevanten Kundendaten eintragen können. Sobald das Konto gespeichert wird, wird es automatisch die Rechnungsadresse für die Bestellung.

Beachten Sie, dass Sie auch die Adresse des Kunden hinzufügen müssen- hierfür steht der "Neue Adresse hinzufügen" -Button am unteren Rand der Seite zur Verfügung.

&#x20;Klicken Sie auf die Schaltfläche "Wählen", um den richtigen Kunden auszuwählen und das gesamte Auftragsformular wird angezeigt. Sein Hauptteil, "Warenkorb", zeigt an, welche Artikel für diese Bestellung relevant sind. Sie können auch eine frühere Bestellung des Kunden wählen, oder einen verwaisten Warenkorb.

Im "Artikel suchen"-Feld können Sie dynamisch Artikel hinzufügen und finden: geben Sie die ersten Buchstaben ihres Namens ein und PrestaShop wird eine Dropdown-Liste mit den passenden Artikeln anzeigen. Wählen Sie einen Artikel und eine Menge, und klicken Sie auf "In den Warenkorb". Selbstverständlich können Sie unter den Varianten der Artikel auch wählen, in diesem Fall wird die „Variante“-Liste angezeigt.

\
&#x20;Beachten Sie, dass PrestaShop Ihnen einen Hinweis auf die Restbestände für die Artikel gibt, mit dem Sie dem Kunden, unter Umständen mitteilen können, dass ein Artikel aktuell nicht auf Lager ist.

Die Seite ermöglicht Ihnen auch, die bisherigen Warenkörbe und Bestellungen für diesen Kunden zu sehen. Stellt sich heraus, dass ein Kunde aus irgendeinem Grund mit seinem Warenkorb nicht selbst bestellen kann, können Sie diesen Warenkorb nutzen, indem Sie auf den Button "benutzen" klicken.

Falls erforderlich, können Sie einen Gutschein  geltend machen, oder sogar einen kurzfristig erstellen, indem Sie auf den Button "Ermässigung hinzufügen" klicken.

Schließlich müssen Sie angeben, wohin die Bestellung geliefert werden soll(und möglicherweise auch in Rechnung gestellt). Auch hier können Sie kurzfristig neue Adressen mit dem "Neue Adresse hinzufügen "-Button erstellen.

## Anzeigen der Bestelldetails <a href="#bestellungen-anzeigenderbestelldetails" id="bestellungen-anzeigenderbestelldetails"></a>

Um die erhaltenen Bestellungen bearbeiten zu können, müssen Sie die darin enthaltenen Informationen anzeigen.\
&#x20;Klicken Sie auf die Bestellung oder auf den Button an der rechten Seite der Bestellung.

Nun Sehen Sie ein Detailblatt für den Auftrag.

Am oberen Rand der Seite ist eine kurze Zusammenfassung der Bestellung: Datum, die Anzahl der Kunden-Service-Tickets darüber, die Anzahl der Produkte in der Bestellung und der Gesamtbetrag.

Auf dem Detailblatt der Bestellung sehen Sie:

* Auf der linken Seite, Bestellinformationen:\

  * Der Status und die Statushistorie der Bestellung.
  * Die Versandinformationen: Gesamtgewicht der Bestellung und gewählter Lieferdienst.
* Auf der rechten Seite Kundeninformationen:\

  * Kauf-Historie.
  * Liefer- und Rechnungsadressen (mit einem groben Lageplan von Google Maps).
* Die Zahlungsmethode, die Kosten der Produkte und die Versandkosten.
* Verschiedene Details zu den bestellten Produkten.

## Bestellungen ändern <a href="#bestellungen-bestellungenaendern" id="bestellungen-bestellungenaendern"></a>

Bestellungen sind nicht endgültig. Es gibt viele Gründe, warum Sie eine Bestellung nachträglich ändern müssen, bevor seine Artikel gesammelt, verpackt und an den Kunden geschickt werden: ein Artikel ist nicht am Lager, der Kunde ändert seine Bestellung durch Anruf, usw.

### Hinzufügen eines Artikels <a href="#bestellungen-hinzufuegeneinesartikels" id="bestellungen-hinzufuegeneinesartikels"></a>

Am unteren Ende der Liste "Artikel" können Sie den "Artikel hinzufügen"-Button anklicken, der ein Feld zur Bestellung hinzufügt.

Beim Hinzufügen eines Artikels werden der Tabelle „Artikel“ einige neue Felder hinzugefügt. Das erste Textfeld ist eigentlich eine kleine Suchmaschine: Geben Sie die ersten Buchstaben eines Artikels ein, um eine Liste der entsprechenden Produkte zu sehen. Wählen Sie die, die Sie hinzufügen möchten. Wenn es eine Artikelvariante ist, können Sie die passende in einer Dropdown-Liste, die unter dem Namen angezeigt wird, auswählen. Legen Sie die Menge fest und klicken dann auf den "hinzufügen": der Artikel wird hinzugefügt.

Sie können keine größere Menge hinzufügen, als zur Verfügung steht.

### Entfernen von Artikeln <a href="#bestellungen-entfernenvonartikeln" id="bestellungen-entfernenvonartikeln"></a>

Um einen Artikel zu löschen, benutzen Sie die Buttons am rechten Rand des jeweiligen Artikels. Nutzen Sie den "Bearbeiten"-Button, wenn Sie nur die Menge ändern wollen.

Sie können die Menge von mehreren Artikeln zur gleichen Zeit bearbeiten.\
&#x20;Wenn die Menge eines Artikels 0 erreicht, wird er von der Bestellung ganz entfernt.\
&#x20;Sie können nicht mehr als die Menge eines Artikels zu entfernen.\
&#x20;Klicken Sie auf die Schaltfläche "Abbrechen", um Ihre Bearbeitung abzubrechen.

## Bearbeiten von Bestellungsdetails <a href="#bestellungen-bearbeitenvonbestellungsdetails" id="bestellungen-bearbeitenvonbestellungsdetails"></a>

Viele Abschnitte des Bestellscheins können bearbeitet werden, um Daten des Kunden zu korrigieren.

### Bestellstatus <a href="#bestellungen-bestellstatus" id="bestellungen-bestellstatus"></a>

Die erste Auswahlliste in der Auftragsseite ermöglicht es Ihnen, den Status zu ändern. Dies ist ein sehr wichtiger des Kontroll-Prozesses, denn bei jeder Statusänderung werden neue Funktionalitäten und Dokumentationen für die Bestellung freigeschaltet.

Sie können zwischen den folgenden Status wählen:

* Awaiting bank wire payment.
* Awaiting Cash on Delivery validation.
* Awaiting cheque payment.
* Awaiting PayPal payment.
* Canceled.
* Delivered.
* On backorder.
* Payment accepted.
* Payment error.
* Payment remotely accepted.
* Preparation in progress.
* Refunded.
* Shipped.

Um einen besseren Überblick über die Bestellung zu erhalten, wird jede Statusänderung aufgezeichnet und der log erscheint direkt unter der Dropdown-Liste der Statusänderung. Deshalb sollten Sie einen Status nur ändern, wenn eindeutig bestätigt: Markieren Sie eine Bestellung nicht als "Delivered" wenn Sie das Paket versendet haben, sondern als "Shipped"; und nutzen Sie nicht "Preparation in progress", wenn Sie nur einen kurzen Blick auf die Bestellung geworfen haben.

Seit Version 1.6.1.0 können Sie E-Mails für einen bestimmten Bestellstatus an den Kunden senden. Um diese E-Mail erneut zu senden, klicken Sie auf "E-Mail erneut senden", neben dem Auftragsstatus. Wenn Sie die Bestellung zu einem bestimmten Zeitpunkt bearbeitet haben, wird eine aktualisierte E-Mail gesendet.

### Aktions-Buttons <a href="#bestellungen-aktions-buttons" id="bestellungen-aktions-buttons"></a>

Die Aktionstasten ändern sich, je nach Zustand der Bestellung. Wenn die Bestellung z.B. den Status "delivered" hat, ändern sich "Artikel hinzufügen" und "Artikel löschen" in zwei neue Schaltflächen: "Warenrücksendung" und "Teilerstattung".

Warenrücksendung  ist standardmäßig nicht aktiviert. Um es zu aktivieren, navigieren Sie unter dem Menüpunkt "Bestellungen" zu „Warenrücksendungen“, und aktivieren Sie die Option unteren Rand der Seite. Dies wird für alle Artikel und Bestellungen gelten.

* **Standard-Rückerstattung**. Verfügbar, sobald die Bestellung den Status "Payment accepted" hat. Nicht mehr verfügbar, wenn die Artikel gesendet wurden. Nötig, um die gesamte Bestellung zurückzuerstatten, und kann, solange die Artikel noch immer im Lager sind, durchgeführt werden. Klicken Sie auf die "Standard Erstattung" und eine neue Spalte mit dem Titel "Rückzahlung" wird angezeigt. Tragen Sie den Betrag und die Menge für jeden der betroffenen Artikel ein, wählen Sie eine der Optionen im unteren Bereich der Liste (siehe unten), und klicken Sie auf "Teilerstattung" am unteren Rand der Tabelle.
* **Teilerstattung**. Verfügbar, sobald die Bestellung den Status „Payment accepted“ hat. Wird verwendet, wenn Sie nur einen Teil der Bestellung und nicht die ganze Bestellung zurückerstatten müssen, entweder weil der Kunde einen Artikel zurückgesendet hat, oder einfach als Zeichen des guten Willens für eine beschädigte Ware, für die sich der Kunde trotzdem entschied. Klicken Sie auf die "Teilerstattung" und eine neue Tabelle mit dem Titel "Teilerstattung" wird angezeigt. Tragen Sie den Betrag und die Menge für jeden der betroffenen Artikel ein, wählen Sie eine der Optionen im unteren Bereich der Liste (siehe unten), und klicken Sie auf "Teilerstattung" am unteren Rand der Tabelle.
* **Artikel zurücksenden**. Verfügbar, sobald die Bestellung den "Shipped"-Status erreicht. In PrestaShop muss das akzeptieren von Warenrücksendungen über Bestellungen> Warenrücksendungen erst aktiviert werden.\
  Nur verwenden, wenn der Kunde Artikel zurückgegeben hat: sobald der Artikel wieder empfangen wurde, können Sie ihn direkt in der Bestellung als zurückgegeben markieren..\
  Klicken Sie auf "Artikel zurücksenden" und eine neue Spalte in der Artikel-Tabelle mit dem Titel "Zurück" öffnet sich. Markieren Sie das Kästchen des betroffenen Artikels und geben Sie die Menge der Elemente, die zurückgegeben wurden, ein, und klicken Sie auf "Artikel zurücksenden" am unteren Rand der Tabelle.

Wenn Sie ein Produkt als zurückzugeben oder zu erstatten markiert haben, sind vier Optionen unter der Liste der Produkte verfügbar:

* **Auf Lager buchen**. Wenn markiert, wird PrestaShop den Lagerbestand für diesen Artikel wieder erhöhen. Sie sollten dies nicht markieren, wenn ein Artikel beschädigt ist.
* **Rückvergütung generieren**. Wenn markiert, wird eine Erstattung als Bestätigung von Ihrem Shop generiert, dass Waren zurückgegeben wurden und dass eine Erstattung erteilt wurde. Der Kunde kann Sie dann für seinen nächsten Einkauf verwenden.
*   **Gutschein erzeugen**. Wenn markiert, wird ein Gutschein für die Menge der ausgewählten Elemente erstellt. Ein Gutschein wird in Form eines Codes bereitgestellt, den der Kunde während der Kaufabwicklung eingeben kann.\
    Sie können vorhandene Gutscheine der Kunden einsehen, indem Sie sie auf der Kunden-Seite ändern: von der Seite der aktuellen Bestellung aus, klicken Sie auf den Link unter dem Namen des Kunden, um zur Kundeninformation zu gelangen. Einmal auf Kundenseite, können Sie diese im Abschnitt "Gutscheine" verwalten. Sie können jeden Gutschein bearbeiten, indem Sie auf das Symbol "Bearbeiten" klicken.

    In PrestaShop sind Gutscheine Teil einer besonderen Art von Nachlässen: "Warenkorb Preisregeln". Sie können erstellt und von der "Warenkorb Preisregeln"-Seite aus unter dem Menüpunkt "Preisregeln" bearbeitet werden. Der Erstellungsprozess von Warenkorb Preisregeln wird im nächsten Kapitel, "Erstellen von Preisregeln und Gutscheinen", erläutert.
* **Versandkosten rückerstatten**.Sie können auch die Versandkosten zurückerstatten, was immer als entschuldigende Geste gilt.

If the customer paid the order using a credit card, the payment system should refund the cart automatically. If the order was paid using a check or a bank transfer, you have to issue the refund yourself, then mark the order as having been refunded manually in the back office (in the order's page).

Unterschied zwischen einer Rückvergütung, einem Gutschein und einer PreisregelEine Rückvergütung ist in erster Linie eine schriftliche Bestätigung, dass ein Artikel zurückgegeben wurde. Man kann sie als Gutschein nutzen\


Ein Gutschein ist nicht an eine Warenrückgabe gebunden und kann mehr Formen als die Rückvergütung annehmen:

* Nachlass auf eine Bestellung (prozentual oder fester Wert).
* kostenloser Versand

Sie können einen Gutschein für alle Kunden, eine Kundengruppe oder einen einzelnen Kunden und das Ablaufdatum festlegen;

Eine Warenkorb Preisregel ist im Grunde eine erweiterte Version eines Gutscheins: zusätzlich zu dem, was ein Gutschein in PrestaShop 1.4 konnte, können Sie nun in PrestaShop 1.5 durch das Warenkorb Preisregeln-System:

* Einen Rabatt benennen.
* Dem Kunden zugestehen, nur einen Teil des Rabatts zu verwenden.
* Prioritäten zwischen Warenkorb Preisregeln vergeben.
* Kompatibilität zwischen Warenkorb Preisregeln setzen.
* Rabatt nur bei gewissen Versand-Diensten zulassen.
* Rabatt nur bei einer Auswahl von Produkten und / oder Kategorien und / oder Herstellern und / oder Lieferanten und / oder Varianten zulassen... oder alle zur gleichen Zeit, wenn nötig!
* Rabatt für kostenlosen Versand und / oder einen Rabatt auf eine bestimmte Bestellung und / oder ein Geschenk ... oder alles zur gleichen Zeit, wenn nötig!

### Dokumente <a href="#bestellungen-dokumente" id="bestellungen-dokumente"></a>

Sie können viele PDF-Dokumente aus der Bestellseite erzeugen. Wenn verfügbar, werden sie in der Spalte "PDF" auf der Seite aufgelistet.

Standardmäßig können Sie die Bestellung als PDF herunterladen, indem Sie einfach auf „Bestellung ausdrucken“ klicken.

Sie können eine Rechnung für die Bestellung anzeigen lassen, indem Sie auf "Rechnung zeigen" klicken. Diese wird erst erzeugt, wenn der Status „Payment accepted“ gesetzt wird.\
&#x20;Sobald sie erzeugt wurde, wird der Button "Rechnung anzeigen" in der oberen Leiste aktiviert.

Sie können das Rechnungslayout leicht anpassen: Die PDF-Template-Dateien liegen im Ordner /pdf. Diese .tpl Dateien sind in HTML mit Smarty-Tags geschrieben, um dynamische Daten zu unterstützen. Sie können das Layout der Rechnung ändern, indem Sie die Datei mit dem Namen invoice.tpl ändern.

Wenn Sie den Status der Bestellung in "Processing in progress" ändern, wird ein Lieferschein als PDF erzeugt, den Sie dann im Bereich "PDF" herunterladen können.

### Versand <a href="#bestellungen-versand" id="bestellungen-versand"></a>

Die Details der Versandkosten der laufenden Bestellung können teilweise bearbeitet werden. Genauer gesagt  können Sie die Tracking-Nummer ändern: Klicken Sie im Abschnitt "Versand" auf das Symbol "Bearbeiten" und geben Sie die neue Nummer ein.

### Lieferadresse <a href="#bestellungen-lieferadresse" id="bestellungen-lieferadresse"></a>

Im Abschnitt "Lieferadresse" können Sie die Zieladresse des Pakets bearbeiten, das versendet werden soll. Sie können entweder die Dropdown-Liste verwenden, um eine andere registrierte Adresse zu wählen, oder Sie klicken auf das Symbol "Bearbeiten", um die aktuell ausgewählte Adresse bearbeiten.

Wenn Sie das Paket an eine Adresse senden, die nicht bereits in PrestaShop registriert wurde, müssen Sie diese zunächst erstellen. Um dies zu tun, Sie die Seite "Adressen" im Menü „Kunden“ und klicken Sie auf den „NEU“-Button. Vergessen Sie nicht, die E-Mail des dazu passenden Kunden einzutragen, denn so weiß PrestaShop, dass die neue Adresse mit einem bestehenden Kunden verknüpft werden soll. Ist das erledigt, gehen Sie zurück zur Seite der Bestellung und ändern Sie die Adresse über die Dropdown-Liste.

Beachten Sie, die kleine Karte ermöglicht es Ihnen, das Ziel des Pakets auf Google Maps zu visualisieren.

### Rechnungsadresse <a href="#bestellungen-rechnungsadresse" id="bestellungen-rechnungsadresse"></a>

Im Abschnitt "Rechnungsadresse" können Sie die Rechnungsadresse der Bestellung bearbeiten. Ebenso wie bei der Versandadresse können Sie entweder mit dem Dropdown-Menü eine andere, im Shop bereits registrierte Adresse wählen oder die ausgewählte Adresse über das Symbol "Bearbeiten" editieren.

Wenn die Rechnungsadresse noch nicht in PrestaShop erstellt wurde, müssen Sie diese erst erstellen. Um dies zu tun, Sie die Seite "Adressen" im Menü „Kunden“ und klicken Sie auf den „NEU“-Button. Vergessen Sie nicht, die E-Mail des dazu passenden Kunden einzutragen, denn so weiß PrestaShop, dass die neue Adresse mit einem bestehenden Kunden verknüpft werden soll. Ist das erledigt, gehen Sie zurück zur Seite der Bestellung und ändern Sie die Adresse über die Dropdown-Liste.

Ermässigung

Am unteren Teil der Rubrik "Artikel" finden Sie den "Ermässigung hinzufügen"-Button. Dies erzeugt einen einfachen Rabatt, der nicht so fortgeschritten wie Gutscheine / Preisregeln ist, aber immer noch sinnvoll eingesetzt werden kann.

Durch Anklicken wird ein neues Formular geöffnet, das folgende Elemente enthält:

* **Name**. Geben Sie dem Rabatt einen kurzen Namen. Diesen wird der Kunde sehen können.
* **Typ** . Wählen Sie den Discount-Typ: "Prozent", "Betrag" oder "versandkostenfrei".
* **Wert**. Für die "Prozent"- oder "Betrag"- Typen setzen Sie hier den Wert des Rabatts.
* **Rechnung**. Wählen Sie, welche Rechnung dieser Bestellung von der Ermässigung profitieren soll. Wenn es mehr als eine Rechnung gibt, können Sie ein Kontrollkästchen setzen, um den Rabatt für alle Rechnungen geltend zu machen.

Der Rabatt wird vor den Versandkosten verrechnet.

## Eine Nachricht an die Bestellung anhängen <a href="#bestellungen-einenachrichtandiebestellunganhaengen" id="bestellungen-einenachrichtandiebestellunganhaengen"></a>

Im Abschnitt "Nachrichten" können Sie einen Kommentar zu der Bestellung für Ihr Team schreiben.

Sie können diesen Kommentar auch an den Kunden senden, um ihm oder ihr Informationen über die Bestellung, eine Verzögerung oder eine Überraschung zu geben, oder halten Sie Ihre Kunden einfach über Angebote und Specials auf dem Laufenden. Dies ist ein wichtiger Punkt der Kundenbeziehung.

Hier gibt es zwei Methoden:

*
  * Sie können einfach in das Nachrichtenfeld schreiben und auf "Nachricht Senden" klicken. Die Nachricht wird im Profil des Kunden in Ihrer Kundendienst-Datenbank gespeichert. Auf die Nachricht können Sie zugreifen, indem Sie entweder  auf die Seite des Kunden navigieren oder sie über die „Kundenservice“-Seite öffnen. Die Nachricht kann auch an die E-Mail-Adresse des Kunden gesendet werden, wenn Sie möchten.
  *   Vordefinierte Nachrichten können gespeichert und danach mehrmals verwendet werden, so sparen Sie sich den Aufwand, selbe Texte redundant erneut schreiben zu müssen. Wenn Sie eine vordefinierte Nachricht versenden möchten, wählen Sie sie aus der Dropdown-Liste. Sie können zu dieser Mitteilung noch weitere Details hinzufügen oder editieren, wenn nötig.

      Sie können vordefinierte Nachrichten erstellen indem Sie zur Seite "Bestellnachrichten" navigieren, zu finden im Menü "Bestellungen".
* **Alle Nachrichten anzeigen**. Dieser Link führt Sie auf die "Kundenservice"-Seite des Menüs "Kunden". Diese wird vollständig im Kapitel "Kundenverwaltung" erläutert.
