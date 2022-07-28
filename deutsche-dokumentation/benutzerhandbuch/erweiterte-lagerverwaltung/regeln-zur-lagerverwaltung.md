# Regeln zur Lagerverwaltung

In diesem Abschnitt werden die Lagerverwaltungsregeln erklärt, die automatisch angewendet werden.

Jede Lager-Ein- und Ausbuchung muss einbezogen werden. Deshalb muss jede Einheit eines lagernden Artikels mit einem Einheitspreis (entweder Anschaffungs- oder Herstellungskosten)(Steuer ausgeschlossen) verbunden werden, sei es eine Bestellung bei einem Lieferanten oder eine manuelle Eingabe. Jede Artikelausbuchung muss auch betrachtet werden.

Es gibt drei Hauptbewertungsmethoden, die Sie wählen können, je nach Tätigkeit oder bezogen auf die Steuergesetze der Standorte der einzelnen Lager:

* FIFO (first in, first out).
* LIFO (last in, first out).
* AVCO (Average Cost, or Weighted Average Cost per Unit).

Mit den FIFO und LIFO-Methoden hat jede Einheit eines Artikels aus dem Lager einen Kaufpreis, der festgelegt wurde, als er in den Lagerbestand aufgenommen wurde. Auf diese Weise können von 100 Einheiten eines bestimmten Artikels 40 einen Kaufpreis von X haben, und 60 einen Kaufpreis von Y. Wenn eine Bestellung durchgeführt wurde, wissen Sie, abhängig von der gewählten Methode, welchen Artikel Sie verschicken und mit welchem Einkaufspreis, dies ermöglicht Ihnen, eine Retour wieder präzise mit dem Einkaufspreis einzubuchen.

Die folgende Tabelle gibt ein Beispiel für die FIFO-Methode bei der Bestandsverwaltung. In diesem Beispiel haben Sie Zwei Eingänge (Die Spalten zeigen den Wert im Einkauf). Sie fügen immer neue Spalten hinzu, wenn Sie den selben Artikel mit neuen Preisen einkaufen.

| Price         | 4     | 6     | 7   |
| ------------- | ----- | ----- | --- |
| Initial stock | 1000  |       |     |
| Entry         |       | 500   |     |
| Exit          | (700) |       |     |
| Exit          | (300) | (400) |     |
| Entry         |       |       | 900 |
| Instant state | 0     | 100   | 900 |

Der Wert der Artikel beträgt dann im instant state in diesem Fall 6900(100\*6+900\*7).

Die folgende Tabelle zeigt, wie die LIFO-Methode verwendet werden kann. Wir verwenden die gleichen Werte wie im vorherigen Beispiel. Das Prinzip bleibt das gleiche wie in dem FIFO Beispiel, mit der Ausnahme, dass die Werte verwendet werden, die zuletzt eingebucht wurden.

| Price         | 4     | 6     | 7   |
| ------------- | ----- | ----- | --- |
| Initial stock | 1000  |       |     |
| Entry         |       | 500   |     |
| Exit          | (200) | (500) |     |
| Exit          | (700) |       |     |
| Entry         |       |       | 900 |
| Instant state | 100   | 0     | 900 |

Der Wert während des instant state ist in diesem Fall 6700.

Die dritte am häufigsten verwendete Methode zur Bestandsbewertung ist Weighted Average Cost (AVCO). Die AVCO Berechnung wird nach jedem neuen Eintrag im Lager durchgeführt.

Für einen gegebenen Artikel wird die AVCO Berechnung anhand der folgenden Formel durchgeführt:

AVCO = (QS \* vorherige AVCO + QA \* UP) / (QS + QA)

Es sei denn, QS negativ oder null, in diesem Fall gilt AVCO = UP.

Mit:

* QS = Anzahl der Artikel, die derzeit auf Lager sind, oder auch Anfangsbestand.
* Menge der Artikel, die dem Lager hinzugefügt werden.
* Einheitspreis (Kaufpreis ausgeschlossen Steuer oder Herstellungskosten).

Die Tabelle unten zeigt die Entwicklung der AVCO mit dem Beispiel eines Produkts zunächst mit 20 Einheiten auf Lager, und zu einem Preis von 2. Neue Ein-/Ausbuchungen werden wie folgt durchgeführt:

|               | Entry | Entry UP | Exit | Exit UP | AVCO | Stock valuation |
| ------------- | ----- | -------- | ---- | ------- | ---- | --------------- |
| Initial stock | 20    | 2        |      |         | 2    | 40              |
| X Date        |       |          | 12   | 2       | 2    | 16              |
| Y Date        | 20    | 3.4      |      |         | 3\*  | 84              |
| Z Date        |       |          | 10   | 3       | 3    | 54              |

\*: Berechnungsdetails: ((8 übrige Artikel auf Lager \* 2) + (20 Artikel hinzufügen \* 3,4)) / 28 Gesamtanzahl der Artikel = 3.

Am Y-Datum berechneten wir die AVCO abhängig von der Anzahl der Produkte im Lager bezogen auf die Einheitspreise neu. Deshalb haben alle Artikel auf Lager jetzt einen neu zugewiesenen Einheitswert, der von der neuen AVCO abhängt.
