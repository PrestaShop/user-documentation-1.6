# Aktualizacja PrestaShop

**Table of contents**

* [Aktualizacja PrestaShop](./#AktualizacjaPrestaShop-AktualizacjaPrestaShop)
  * [Kopia zapasowa i możliwe problemy](./#AktualizacjaPrestaShop-Kopiazapasowaimożliweproblemy)
  * [Wsparcie PrestaShop](./#AktualizacjaPrestaShop-WsparciePrestaShop)
  * [Sprawdzanie wymagań, jakie trzeba spełnić, żeby zaktualizowana wersja PrestaShop działała poprawnie](./#AktualizacjaPrestaShop-Sprawdzaniewymagań,jakietrzebaspełnić,żebyzaktualizowanawersjaPrestaShopdziałałapoprawnie)
  * [Informacja dla osób chcących aktualizować sklep w wersji niższej niż 1.4.x ](./#AktualizacjaPrestaShop-Informacjadlaosóbchcącychaktualizowaćsklepwwersjiniższejniż1.4.x)

## Aktualizacja PrestaShop <a href="#aktualizacjaprestashop-aktualizacjaprestashop" id="aktualizacjaprestashop-aktualizacjaprestashop"></a>

Nowe wersje PrestaShop pojawiają się co kilka miesięcy, czasem nawet co tydzień. Niektóre z nich znacząco różnią się od wersji poprzednich, wiekszość zawiera tylko drobne poprawki, ale wszystkie aktualizacje sprawiają, że PrestaShop jest coraz doskonalszym narzedziem sprzedaży, w którym jest coraz wiecej ulepszeń i coraz mniej błędów. Dlatego też zalecamy używanie mozliwie najnowszej wersji tego oprogramowania.

Istnieją dwa sposoby aktualizowania PrestaShop:

* [Automatyczny](automatyczna-aktualizacja.md)
* [Ręczny](reczna-aktualizacja.md)

Automatyczna aktualizacja wykorzystuje darmowy moduł [1-Click Upgrade](http://addons.prestashop.com/en/administration-tools-prestashop-modules/5496-1-click-upgrade-autoupgrade.html).

Ręczna aktualizacja nie jest już wspierana, ale jej dokumentację zachowujemy dla celów archiwizacyjnych - oraz dla tych osób, które z jakichś względów nie mogą przeprowadzić aktualizacji automatycznej.

Uwaga

Proces aktualizacji może wpłynąć na wszystkie pliki i foldery, również te znajdujące sie w katalogu głównym sklepu. W tym zbiorze znajdują się także wszystkie kluczowe pliki niezbędne do działania sklepu, wszystkie domyślne moduły i domyślny szablon. Jeśli te pliki w Twoim sklepie zostały zmodyfikowane, po aktualizacji wszystkie te zmiany zostaną utracone.

Przeprowadzony prawidłowo, cały proces opisany w niniejszej instrukcji powinien zająć nie więcej niz pół godziny. Nie wolno pomijać żadnych kroków opisywanej tu procedury, ponieważ może to spowodować, że aktualizacja sie nie powiedzie.

### Kopia zapasowa i możliwe problemy <a href="#aktualizacjaprestashop-kopiazapasowaimozliweproblemy" id="aktualizacjaprestashop-kopiazapasowaimozliweproblemy"></a>

W razie gdyby cos poszło nie tak, trzeba wcześniej [utworzyć kopię zapasową danych i wiedzieć, jak w razie problemów ją przywrócić](../../english-documentation/updating-prestashop/making-and-restoring-your-own-backup.md).

Jeśli potrzebujesz rozwiązania innych problemów, [zapoznaj sie z tymi informacjami](../../english-documentation/updating-prestashop/in-case-of-issues.md).  &#x20;

### Wsparcie PrestaShop <a href="#aktualizacjaprestashop-wsparcieprestashop" id="aktualizacjaprestashop-wsparcieprestashop"></a>

W celu **rozwiązania jakichkolwiek problemów** ze swoim sklepem, albo **uzyskania pomocy przy instalacji** sklepu, skontaktuj sie z nami i poznaj nasza ofertę profesjonalnego wsparcia.

Nasz zespół ekspertów jest do Twojej dyspozycji  w zakresie rozwiązywania wszystkich problemów związanych z aktualizacją twojego sklepu PrestaShop:

* Przez e-mail: mozesz użyć formularza znajdującego sie pod adresem [https://www.prestashop.com/en/support](https://www.prestashop.com/en/support)
* Telefonicznie: +33.1 40 18 30 04 (w godzinach: 9:00  – 18:00 czasu środkowoeuropejskiego)
* Dowiedz się więcej o naszej ofercie wsparcia: [http://support.prestashop.com](http://support.prestashop.com)
* I koniecznie odwiedź nasze bardzo pomocne [forum społeczności PrestaShop](http://www.prestashop.com/forums/)

### Sprawdzanie wymagań, jakie trzeba spełnić, żeby zaktualizowana wersja PrestaShop działała poprawnie <a href="#aktualizacjaprestashop-sprawdzaniewymagan-jakietrzebaspelnic-zebyzaktualizowanawersjaprestashopdzial" id="aktualizacjaprestashop-sprawdzaniewymagan-jakietrzebaspelnic-zebyzaktualizowanawersjaprestashopdzial"></a>

Zanim dokonasz jakichkolwiek zmian w Twoim obecnym sklepie, powinieneś sprawdzić, czy Twój serwer spełnia minimalne wymagania techniczne, konieczne do poprawnego działania nowej wersji PrestaShop. Wymagania te opisane są na tej stronie: [http://www.prestashop.com/en/system-requirements](http://www.prestashop.com/en/system-requirements).\
Powinieneś na przykład sprawdzić, czy na serwerze, na którym zainstalowany jest Twój sklep, działa wymagana wersja PHP czy MySQL. Jełśi nie, możesz samemu zaktualizowac to oprogramowanie do właściwego, albo poprosic Twojego dostawcę usług hostingowych, aby dokonał tej aktualizacji za Ciebie. Jeśli nie masz pewności, w jakich wersjach PHP i MySQL są zainstalowane Twoim serwerze, zapytaj Twojego dostawcę usług hostingowych.

Jeśli Twój dostawca hostnigu z jakichś przyczyn nie chce zaktualizować konfiguracji Twojego serwera, oznacza to, że może warto pomyśleć nad zmianą dostawcy. Prosimy NIE dokonywać żadnych aktualizacji, dopóki nie masz pewności, że Twój serwer spełnia minimalne wymagania techniczne.

### Informacja dla osób chcących aktualizować sklep w wersji niższej niż 1.4.x  <a href="#aktualizacjaprestashop-informacjadlaosobchcacychaktualizowacsklepwwersjinizszejniz1.4.x" id="aktualizacjaprestashop-informacjadlaosobchcacychaktualizowacsklepwwersjinizszejniz1.4.x"></a>

Starsze wersje PrestaShop mogą nie dawać aktualizować się tak łatwo jak wersje nowsze: ich kod jest zupełnie inny, lokalizacja wielu plików w międzyczasie zmieniła się, powstały nowe pliki, podczas kiedy inne zniknęły. Z tego względu ryzyko napotkania wielu błędów podczas aktualizacji ze starszych wersji do najnowszej jest niestety dość znaczne.

Mając starszy sklep jest się również ograniczonym do stosowania wyłącznie aktualizacji  [w trybie ręcznym](reczna-aktualizacja.md): moduł 1-Click Upgrade działa wyłącznie w PrestaShop w wersji 1.4 i nowszych.&#x20;

Należy zatem zachować szczególną ostrożność. Im starszą wersję PrestaShop aktualizujesz, tym więcej uwagi powinieneś poświęcić kopii zapasowej, plikach, które w toku prac deweloperskich zostały zmienione na wyłączny użytek w Twoim sklepie, czy unikalnemu szablonowi.&#x20;
