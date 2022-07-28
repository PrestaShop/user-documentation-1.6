# Zasady zarządzania magazynem

Znajdziesz tutaj zasady zarządzania stosowane automatycznie przy zarządzaniu magazynem

Każdorazowe wejście i wyjście z magazynu  powinno być odnotowane. To dlatego każdy jednostkowy produkt wchodzący do magazynu musi posiadać cenę jednostkową netto (cenę zakupu lub produkcji) i być połączony z pośrednikiem zamówienia dostawy lub ręcznym wprowadzeniem. i każdorazowe wyjście produktu z magazynu musi zostać odnotowane.

Dlatego istnieją trzy sposoby podstawowej waloryzacji, które należy wybrać w zależności od działania lub zasad mających zastosowanie w kraju dla każdego magazynu:

* FIFO (pierwsze wejście, pierwsze wyjście).
* LIFO (ostatnie wejście, pierwsze wyjście).
* AVCO (średni koszt lub średni ważony koszt jednostkowy).

W przypadku metod FIFO i LIFO, każdy produkt jednostkowy w magazynie posiada ustaloną cenę zakupu w chwili dodania do magazynu. Zatem dla danego odniesienia dostępnego w 100 egzemplarzach, 40 egzemplarzy może posiadać cenę zakupu X, a kolejne 60 cenę zakupu Y. W chwili składania zamówienia i wg wybranej metody, wiadomo jaki produkt należy zarezerwować i w jakiej cenie , co pozwala na dokładne zarządzanie ewentualnymi zwrotami produktów i umieszczeniu ich  w magazynie z taką samą ceną początkową.

Tabela poniżej przedstawia użytkowanie metody LIFO, aby oszacować wartości magazynu. W tym przypadku mamy do czynienia z tabelą z dwoma hasłami “wejście” (cena i ilość pod względem typu ruchu). Stopniowo w miarę dokonanych odbiorów Dodawane zostają nowe kolumny.

| Cena          | 4     | 6     | 7   |
| ------------- | ----- | ----- | --- |
| Initial stock | 1000  |       |     |
| Entry         |       | 500   |     |
| Exit          | (700) |       |     |
| Exit          | (300) | (400) |     |
| Entry         |       |       | 900 |
| Instant state | 0     | 100   | 900 |

W tym przypadku wartość zapasów w czasie bieżącego stanu wynosi 6900.

Poniższa tabela pokazuje, w jaki sposób można użyć metody FIFO do obliczenia wartości magazynu. Używamy tych samych wartości wejścia i wyjścia, tak jak w poprzednim przykładzie. Główna zasada jest taka sama jak w przykładzie FIFO, wykluczając momenty wyjść, przede wszystkim używamy jednostek, które były ostatnio wprowadzone do magazynu.

| Cena          | 4     | 6     | 7   |
| ------------- | ----- | ----- | --- |
| Initial stock | 1000  |       |     |
| Entry         |       | 500   |     |
| Exit          | (200) | (500) |     |
| Exit          | (700) |       |     |
| Entry         |       |       | 900 |
| Instant state | 100   | 0     | 900 |

Wartość magazynu w chwili obecnej sesji w tym przypadku wynosi 6900.

Trzecią metodą najczęściej stosowaną do wyceny magazynu jest średnia ważona kosztów (AVCO). Obliczenie AVCO odbywa się po każdym nowym wpisie w magazynie.

Dla danego produktu, obliczenia AVCO odbywa się za pomocą wzoru:

AVCO = (QS \* previous AVCO + QA \* UP) / (QS + QA)\
&#x20;Unless QS is negative or null, in which case AVCO = UP.

gdzie:

* QS = Aktualna ilość produktów w magazynie lub magazyn pierwotny.
* QA = ilość przeznaczona do dodania do magazynu.
* UP = koszt jednostkowy (cena zakupu netto lub koszt produkcji).

Poniższa tabela ilustruje ewolucję AVCO na przykładzie produktu początkowo z 20 sztukami w magazynie, a kupony w cenie 2. Nowe wejścia / wyjścia będą wyceniane w następujący sposób:

|               | Entry | Entry UP | Exit | Exit UP | AVCO | Stock valuation |
| ------------- | ----- | -------- | ---- | ------- | ---- | --------------- |
| Initial stock | 20    | 2        |      |         | 2    | 40              |
| X Date        |       |          | 12   | 2       | 2    | 16              |
| Y Date        | 20    | 3.4      |      |         | 3\*  | 84              |
| Z Date        |       |          | 10   | 3       | 3    | 54              |

\*: Szczegóły obliczeniowe: ((8 pozostałe produkty w magazynie \* 2) + (20 produktów do dodania \* 3.4)) / 28 = 3 produktów ogółem.

Na dzień Y, obliczyliśmy AVCO według liczby produktów dodanych w magazynie z ich ceną jednostkową. Dlatego wszystkie produkty w magazynie mają teraz przypisaną wartość jednostkową, która zależy od nowego AVCO.
