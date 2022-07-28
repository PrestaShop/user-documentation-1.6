# Regels voor voorraadbeheer

In deze sectie, zullen we uitleggen wat de beheerregels zijn die automatisch worden toegepast op voorraadbeheer.

Elke keer als er voorraad wordt toegevoegd of verwijderd moet daar een waarde aan worden gekoppeld. Dat is waarom elk item gekoppeld moet worden met een artikelprijs zonder belasting (inkoopprijs of productiekosten), leveranciersbestelling of handmatig. Elke keer als er voorraad wordt verwijderd moet er ook een waarde aan worden gekoppeld.

Er zijn drie methoden om de voorraad aan te passen, waar u uit kunt kiezen, afhankelijk van uw bedrijfsactiviteiten of belastingwetten van de landen waar de magazijnen zich bevinden:

* FIFO (first in, first out).
* LIFO (last in, first out).
* AVCO (Average Cost, of Weighted Average Cost per Unit).

Met de FIFO- en LIFO-methoden heeft elk product uit de voorraad een vaste inkoopprijs die het heeft gekregen bij het toevoegen. Op deze manier kan een voorraad, bestaande uit 100 units, 40 units hebben met een inkoopprijs van X en 60 met een inkoopprijs van Y. Wanneer een bestelling is geplaatst en afhankelijk van de gekozen methode weet u welk product gebruikt moet worden en met welke inkoopprijs. Dit maakt het mogelijk om nauwkeurig om te gaan met mogelijke retourneringen en producten terug kunt plaatsten met de oorspronkelijke inkoopprijs.

De tabel hieronder geeft u een voorbeeld van de FIFO-methode. In dit voorbeeld hebt u een tabel met twee variabelen (prijs en hoeveelheid per type voorraadverplaatsing). U voegt in feite meer kolommen toe als u producten ontvangt met andere prijzen.

| Prijs                    | 4     | 6     | 7   |
| ------------------------ | ----- | ----- | --- |
| Oorspronkelijke voorraad | 1000  |       |     |
| Toegevoegd               |       | 500   |     |
| Verwijderd               | (700) |       |     |
| Verwijderd               | (300) | (400) |     |
| Toegevoegd               |       |       | 900 |
| Uiteindelijke voorraad   | 0     | 100   | 900 |

De voorraadwaarde gedurende de uiteindelijke staat is in dit geval 6.900.

De tabel hieronder illustreert hoe de LIFO-methode gebruikt kan woorden om de voorraad te taxeren. We gebruiken dezelfde waarden als in bovenstaand voorbeeld. Het principe blijft hetzelfde als FIFO, behalve dat gedurende het verwijderen van voorraad we hoofdzakelijk de units gebruiken die als laatste zijn toegevoegd aan de voorraad.

| Prijs                    | 4     | 6     | 7   |
| ------------------------ | ----- | ----- | --- |
| Oorspronkelijke voorraad | 1000  |       |     |
| Toegevoegd               |       | 500   |     |
| Verwijderd               | (200) | (500) |     |
| Verwijderd               | (700) |       |     |
| Toegevoegd               |       |       | 900 |
| Uiteindelijke voorraad   | 100   | 0     | 900 |

De voorraadwaarde gedurende de uiteindelijke staat is in dit geval 6.700.

De op twee na meest gebruikte methode om de waarde van de voorraad te bepalen is Weighted Average Cost (AVCO). De AVCO-berekening wordt uitgevoerd, nadat er voorraad is toegevoegd.

Voor een gegeven product wordt de AVCO-berekening als volgt gedaan:

AVCO = (QS \* vorige AVCO + QA \* UP) / (QS + QA)

Tenzij QS negatief of null is, in een dergelijk geval geldt AVCO = UP.

Met:

* QS = Aantal producten die momenteel op voorraad zijn, of oorspronkelijke voorraad.
* QA = Aantal producten dat wordt toegevoegd aan de voorraad.
* UP = Unitprijs (inkoopprijs zonder belasting of productiekosten).

De tabel hieronder illustreert de veranderingen in de AVCO met het voorbeeld van een product dat begint met 20 op voorraad en waarvan voorraad wordt ingekocht met een prijs van 2. De nieuwe toevoeg/verwijder waarden zijn als volgt:

|                          | Toegevoegd | Toegevoegd met UP | Verwijderd | Verwijderd met UP | AVCO | Waarde van voorraad |
| ------------------------ | ---------- | ----------------- | ---------- | ----------------- | ---- | ------------------- |
| Oorspronkelijke voorraad | 20         | 2                 |            |                   | 2    | 40                  |
| Datum X                  |            |                   | 12         | 2                 | 2    | 16                  |
| Datum Y                  | 20         | 3.4               |            |                   | 3\*  | 84                  |
| Datum Z                  |            |                   | 10         | 3                 | 3    | 54                  |

\*: Details van berekening: ((8 producten resterend op voorraad \* 2) + (20 producten om toe te voegen \* 3.4)) / 28 producten in totaal = 3.

Op datum Y hebben we de AVCO berekend volgens het aantal producten dat is toegevoegd aan de voorraad in hun oorspronkelijke unitprijs. Daarom hebben alle producten die nu nog op voorraad zijn een nieuwe unitprijs gekregen, welke afhankelijk is van de nieuwe AVCO.
