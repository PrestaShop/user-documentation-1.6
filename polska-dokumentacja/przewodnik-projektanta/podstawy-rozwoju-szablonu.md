# Podstawy rozwoju szablonu

/\*\<!\[CDATA\[\*/\
div.rbtoc1597140227583 {padding: 0px;}\
div.rbtoc1597140227583 ul {list-style: disc;margin-left: 0px;}\
div.rbtoc1597140227583 li {margin-left: 0px;padding-left: 0px;}\
\
/\*]]>\*/

* [Podstawy rozwoju szablonu](podstawy-rozwoju-szablonu.md#Podstawyrozwojuszablonu-Podstawyrozwojuszablonu)
  * [Koncepcja](podstawy-rozwoju-szablonu.md#Podstawyrozwojuszablonu-Koncepcja)
    * [Model](podstawy-rozwoju-szablonu.md#Podstawyrozwojuszablonu-Model)
    * [Widok](podstawy-rozwoju-szablonu.md#Podstawyrozwojuszablonu-Widok)
    * [Kontroler](podstawy-rozwoju-szablonu.md#Podstawyrozwojuszablonu-Kontroler)
    * [Jak działa szablon](podstawy-rozwoju-szablonu.md#Podstawyrozwojuszablonu-Jakdziałaszablon)
    * [Specyficzne foldery szablonu](podstawy-rozwoju-szablonu.md#Podstawyrozwojuszablonu-Specyficznefolderyszablonu)
  * [Generalne informacje](podstawy-rozwoju-szablonu.md#Podstawyrozwojuszablonu-Generalneinformacje)
    * [Jak działają szablony](podstawy-rozwoju-szablonu.md#Podstawyrozwojuszablonu-Jakdziałająszablony)
    * [Specyficzne foldery szablonów](podstawy-rozwoju-szablonu.md#Podstawyrozwojuszablonu-Specyficznefolderyszablonów)
    * [Podgląd na folder tematów](podstawy-rozwoju-szablonu.md#Podstawyrozwojuszablonu-Podglądnafoldertematów)
  * [Technologie](podstawy-rozwoju-szablonu.md#Podstawyrozwojuszablonu-Technologie)
    * [Podstawy](podstawy-rozwoju-szablonu.md#Podstawyrozwojuszablonu-Podstawy)
    * [Smarty 3](podstawy-rozwoju-szablonu.md#Podstawyrozwojuszablonu-Smarty3)
    * [Bootstrap v3](podstawy-rozwoju-szablonu.md#Podstawyrozwojuszablonu-Bootstrapv3)
    * [Sass i Compass](podstawy-rozwoju-szablonu.md#Podstawyrozwojuszablonu-SassiCompass)
  * [Porady](podstawy-rozwoju-szablonu.md#Podstawyrozwojuszablonu-Porady)
    * [Rozszerzenia przeglądarki](podstawy-rozwoju-szablonu.md#Podstawyrozwojuszablonu-Rozszerzeniaprzeglądarki)
    * [Najlepsze porady](podstawy-rozwoju-szablonu.md#Podstawyrozwojuszablonu-Najlepszeporady)

## Koncepcja <a href="#podstawyrozwojuszablonu-koncepcja" id="podstawyrozwojuszablonu-koncepcja"></a>

System szablonów PrestaShop pozwala developerom i programistom łatwo zbudować swój własny szablon, pod warunkiem, że mają solidne podstawy techniczne.

System szablonów jest zbudowany na 3 - warstwowej architekturze :

* **Poziom danych (obiekty danych).** Dostęp do bazy danych jest kontrolowany poprzez pliki w folderze  `/classes`.
* **Warstwa aplikacji (kontrola danych)**. Treści dostarczane przez uzytkowników są kontrolowane przez pliki w folderze głównym.
* **Poziom prezentacji (projekt)**.Wszystkie pliki tematu są w folderze `/themes`.

Szablon należy do warstwy prezentacji: Szablon plików znajduje się w folderze `/themes`, będzie obsługiwać dane dostępowe wysyłane przez warstwę aplikacji i ich powrót do warstwy aplikacji.

![](<../../.gitbook/assets/26738689 (1).png>)

Zobacz w Wikipedii więcej informacji na temat architektury 3 warstwowej: [http://en.wikipedia.org/wiki/Multitier\_architecture#Three-tier\_architecture](http://en.wikipedia.org/wiki/Multitier\_architecture#Three-tier\_architecture)

Architektura 3 - warstwowa ma wiele zalet:

* Ułatwia odczytanie kodu.
* Programiści mogą dodawać i edytować kod szybciej.
* Graficy i  integratorzy HTML mogą pracowć z zakresem powierzonych folderów `/themes` bez odczytania czy zrozumienia choćby jednej linijki kodu PHP.
* Programiści mogą pracować na dodatkowych danych i modułach, które mogą wykorzystać integratorzy HTML.

Jest to ta sama zasada jak  w Model-View-Controller (MVC) architektury, tylko jest to prostrzy i bardziej przystepny sposób.\
Dowiedz się więcej na temat MVC w Wikipedii: [http://en.wikipedia.org/wiki/Model-view-controller](http://en.wikipedia.org/wiki/Model-view-controller)

### Model <a href="#podstawyrozwojuszablonu-model" id="podstawyrozwojuszablonu-model"></a>

Model pokazuje zachowanie aplikacji: przetwarzania danych, interakcji bazy danych etc.

Opisuje lub zawiera dane które zostały przetworzone przez aplikacje. Zarządza tymi danymi i zapewnia ich integralność.

### Widok <a href="#podstawyrozwojuszablonu-widok" id="podstawyrozwojuszablonu-widok"></a>

Widok jest interfejsem użytkownika z którym użytkownik wchodzi w interakcje.

Jego pierwszym zadaniem jest wyświetlanie danych, które są udzielane przez model. Jego druga rola służy do obsługi wszystkich działań ze strony użytkownika (kliknięcia myszą, wyboru elementów, przyciski, etc.), a także wysyła te zdarzenia do kontrolera.&#x20;

Widok nie przetwarza, tylko wyświetla widok przetwarzania wykonywanego przez model i komunikuje się z użytkownikiem.

### Kontroler <a href="#podstawyrozwojuszablonu-kontroler" id="podstawyrozwojuszablonu-kontroler"></a>

Kontroler ma za zadanie synchronizować zdarzenia pomiędzy Modelem a Widokiem i aktualizować obydwa jeśli jest taka potrzeba. Otrzymuje on wszystkie zdarzenia użytkownika i inicjuje potrzebne czynności do wykonania.

Jeśli jest potrzeba zmian danych, Kontroler zapyta Model w celu zmiany danych, a Model z kolei powiadomi, że dane zostały zmienione, tak aby widok mógł się aktualizować samoczynnie.

### Jak działa szablon <a href="#podstawyrozwojuszablonu-jakdzialaszablon" id="podstawyrozwojuszablonu-jakdzialaszablon"></a>

Szablon PrestaShop to zestaw plików które można edytować w celu zmiany wyglądu sklepu internetowego.

Oto kilka ważnych informacji:

* Wszystkie tematy i pliki mają swoje lokalizacje w folderze głównym `/themes`.
* Każdy z motywów ma swój własny sub-folder w folderze głównym tematów.
* Każdy z tematów jest wykonany z pliku szablonów (`.tpl`), pliku obrazów (`.gif`, `.jpg`, `.png`), z jednego lub więcej plików CSS (`.css`), i czasami także z plików JavaScript (`.js`).
* Każdy z temtów ma podgląd 180\*200 `preview.jpg`  pliku w folderze umożliwiając właścicielowi sklepu zobaczenie wyglądu sklepu bezpośrednio z panelu adminstracyjnego, a następnie wybór odpowiedniego tematu.

### Specyficzne foldery szablonu <a href="#podstawyrozwojuszablonu-specyficznefolderyszablonu" id="podstawyrozwojuszablonu-specyficznefolderyszablonu"></a>

Trzeba być świadomym, że istnieje 5 głównych folderów PrestaShop:

* `/modules`: To gdzie moduły są zlokalizowane. Moduł zawiera pliki szablonów, które mogą być w części tematycznej przedefiniowane.
* `/themes`: Jest miejscem gdzie wszystkie tematy są zlokalizowane. Domyślny temat 1.5 jest w folderze `/default` (w 1.4, był w `/prestashop`).
* `/mails`: Tutaj są zlokalizowane wszystkie e-maile szablonu. E-mail szablonu  powinien dokładnie odzwierciedlać styl i projekt głównego szablonu. Każdy sub-folder zawiera szablony dla danego języka.
* `/img`: W tym miejscu są zlokalizowane wszystkie obrazy sklepu. **Specyficzne obrazy dotyczące szablonu są we własnym folderze `/img`**\
  ****
* `/pdf`: Tutaj są zlokalizowane wszystkie modele dokumentów.

## Generalne informacje <a href="#podstawyrozwojuszablonu-generalneinformacje" id="podstawyrozwojuszablonu-generalneinformacje"></a>

### Jak działają szablony <a href="#podstawyrozwojuszablonu-jakdzialajaszablony" id="podstawyrozwojuszablonu-jakdzialajaszablony"></a>

Szablon PrestaShop jest zestawem plików które można edytować w celu zmiany wyglądu własnego sklepu internetowego.

Oto kilka ważnych ciekawostek:

* Wszystkie motywy mają swoją lokalizacje w w folderze głównym `/themes`.
* Każdy z motywów ma swój własny sub-folder w głównym folderze tematów.
* Każdy z motywów jest wykonany z pliku szablonów  (`.tpl`), pliki obrazów (`.gif`, `.jpg`, `.png`), z jednego lub więcej plików CSS (`.css`), i czasami nawet z plików JavaScript (`.js`).
* Każdy z nich ma 180\*200 `preview.jpg` plik obrazka w folderze, umożliwiający właścicielowi sklepu zobaczenie wyglądu szablonu bezpośrednio z pozycji panelu adminstracyjnego i następnie wybór odpowiedniego motywu.

### Specyficzne foldery szablonów <a href="#podstawyrozwojuszablonu-specyficznefolderyszablonow" id="podstawyrozwojuszablonu-specyficznefolderyszablonow"></a>

Jako developer musisz zwrócić uwagę na 5 głównych folderów:

* `/modules`:to gdzie wszystkie moduły są zlokalizowane. Moduły szablonów  mają swoje pliki, możesz również przedefiniować części tematyczne.
* `/themes`: tutaj są zlokalizowane wszystkie motywy.\

  * Domyślny motyw 1.6 jest w folderze `/default-bootstrap`.
  * Domyślny motyw 1.5 był w folderze `/default`.
  * Domyślny motyw 1.4 był w folderze `/prestashop`.
* `/mails`: Tutaj są zlokalizowane wszystkie szablony. Szablony e-mail powinny idealnie odzwierciedlać styl i design głównego motywu. Każdy sub-folder zawiera szablony dla danego języka.
* `/img`: Tutaj są zlokalizowane obrazki sklepu. **Specyficzne motywy obrazków są zapisywane we własnym folderze  `/img`.**
* `/pdf`: Tutaj są zlokalizowane modele dokumentów.

### Podgląd na folder tematów <a href="#podstawyrozwojuszablonu-podgladnafoldertematow" id="podstawyrozwojuszablonu-podgladnafoldertematow"></a>

Oto podgląd na strukturę tematów w PrestaShop  (tutaj domyśny motyw):

![](<../../.gitbook/assets/26738690 (1).png>)

* Folder `/css`, zawiera wszystkie pliki CSS\

  * Folder `sass` zawiera wszystkie foldery Sass`.scss` Pliki źródłowe, za nim zostaną skompilowane w plikach CSS.
* Folder `/font` contkie potrzebuje plików trzcionek.
* Foder `/img` zawiera wszystkie obrazki.
* Folder`/js` zawiera wszystkie pliki JavaScript.
* Folder `/lang` zawiera wszystkie tłumaczenia tematu.Jego prawa dostępu powinny być ustawione na CHMOD 666 (na przykład), tak, że narzędzie panelu adminstracyjnego do tłumaczenia może odczytywać i zapisywać do niego.
* Folder`/mobile` zawiera mobilną wersje strony.
* Folder `/modules`  zawiera potrzebny szablon plików do wielu modułów.
* Folder główny zawiera tylko pliki TPL (pliki Smarty), jak również plik miniatur `preview.jpg`.

## Technologie <a href="#podstawyrozwojuszablonu-technologie" id="podstawyrozwojuszablonu-technologie"></a>

### Podstawy <a href="#podstawyrozwojuszablonu-podstawy" id="podstawyrozwojuszablonu-podstawy"></a>

Tak jak każda strona, szablony PrestaShop są wyświetlane jako mix HTML, CSS i JavaScript. Te trzy języki są podstawą każdej strony internetowej, dlatego powinienieś je znać za nim podejmiesz się edycji istniejącego tematu lub utworzysz nowy.

Domyślny szablon (`/themes/default-bootstrap`) używa HTML5, CSS3 i JQuery-steruje JavaScript ([http://jquery.com/](http://jquery.com/)). Używamy jQuery v1.11+.

### Smarty 3 <a href="#podstawyrozwojuszablonu-smarty3" id="podstawyrozwojuszablonu-smarty3"></a>

W swej istocie motyw PrestaShop jest oparty na silniku szablonu Smarty 3 ([http://www.smarty.net/](http://www.smarty.net/)), co pozwala programistą i developerom łatwo zabudować własnego motywu, z niewielką wiedzą techniczną  .

Smarty 2 jest od dawna przestarzała i nie powinna być używana do motywów w PrestaShop 1.6.

### Bootstrap v3 <a href="#podstawyrozwojuszablonu-bootstrapv3" id="podstawyrozwojuszablonu-bootstrapv3"></a>

Od kiedy wersja 1.6 PrestaShop zawiera strukturę czołową Bootstrap  ([http://getbootstrap.com/](http://getbootstrap.com/)). Jest to zbiór narzedzi HTML i CSS które pozwalają zbudować programiście ładną i responsywną  stronę (co oznacza, że można je łatwo dostosować do dowolnej wielkości ekranu). Początkowo służyło to do wewnętrznych wzorców i projektów w firmie Twitter, ale szybko urosło do najczęściej używanej ramy struktury czołowej.

PrestaShop używa Bootstrapa dla obydwu narzędzi szablonu zarówno czołowego jak i panelu administracyjnego.

Projektanci tworzący nowy panel administracyjny muszą używać Bootstrapa.

Projektanci tworzący nową stronę czołową powinni użyć Bootstrapa. Nie jest to obligatoryjne, ale Bootstrap jest mocno wkomponowany w PrestaShop.

Bootstrap początkowo używa mniej dynamicznego arkusza stylów LESS ([http://lesscss.org/](http://lesscss.org/)), ale PrestaShop używa Bootstrapa dla portu Sass ([https://github.com/twbs/bootstrap-sass](https://github.com/twbs/bootstrap-sass)), Sass jest językiem który inspiruje LESS. To umożliwia użycie ramy Compass.

Przewodnik dla projektanta poruszy ten temat głębiej o Bootstrapie w późniejszym rozdziale.

### Sass i Compass <a href="#podstawyrozwojuszablonu-sassicompass" id="podstawyrozwojuszablonu-sassicompass"></a>

Wersja 1.6 także daje możliwość użycia języka skryptu Sass ([http://sass-lang.com/](http://sass-lang.com/)), i komponuje się z ramką Compassa.

Sass (skrót składniowy arkusza stylów) jest preprocesorem CSSS3 czyli warstwą pomiedzy arkuszami stylów których jesteś autorem i`.css` plików które służą przeglądarce (jak powiedział Dan Cederholm: [http://alistapart.com/article/why-sass](http://alistapart.com/article/why-sass)). Ma on na celu ułatwianie życia podczas tworzenia plików CSS poprzez rozszerzenie języka CSS:

* Dodaje zmienne wstawek i funkcje (dziedziczy).
* To pomaga w zapobiec powtórzenia kodu.
* To sprawia, że łatwiej jest zachować kod.
* To sprawia, że piszę się go szybciej.
* etc.

Zamiast bezpośredniego tworzenia `plików .css`, projektant tworzy plik `.sass` albo`.scss` który jest interpretowany do standardu pliku CSS  przy użyciu wiersza polecenia lub narzędzia online.\
Należy pamiętać, że można to zrobic zmieniając sposób w jaki używane jest zwykły proces CSS: Jak znowu pisze Dan Cederholm, "Sass jest przedłużeniem CSS3, a jego SCSS (“Sassy CSS”) składnia jest rozszerzeniem CSS3. Oznacza to, że ważny dokument CSS3 jest również ważnym dokumentem SCSS."

Ze swej strony, Compass ([http://compass-style.org/](http://compass-style.org/)) jest ramą Sassa – czyli kombinacja narzędzi jest stworzoną, aby pomóc budować i zarządzać plikami CSS używając języka Sass. Jest napisany w Ruby.

Ten przewodnik projektanta zagłębi się mocniej w Sass i Compass w następnym rozdziale.

## Porady <a href="#podstawyrozwojuszablonu-porady" id="podstawyrozwojuszablonu-porady"></a>

### Rozszerzenia przeglądarki <a href="#podstawyrozwojuszablonu-rozszerzeniaprzegladarki" id="podstawyrozwojuszablonu-rozszerzeniaprzegladarki"></a>

Wszyscy projektanci stron i programiści powinni stosować następujące rozszeżenia przeglądarki:

* Firefox: używa narzędzi programistów (zobacz [https://developer.mozilla.org/en-US/docs/Tools](https://developer.mozilla.org/en-US/docs/Tools)). Mogą tobie nawet pomóc przy pracy z Sassem: [https://hacks.mozilla.org/2014/02/live-editing-sass-and-less-in-the-firefox-developer-tools/](https://hacks.mozilla.org/2014/02/live-editing-sass-and-less-in-the-firefox-developer-tools/)
* Firefox: alternatywnie instaluje wtyczkę Firebug ([http://getfirebug.com/](http://getfirebug.com/)), darmowe rozszerzenie dla łatwiejzego porównania i debugowania pomiędzy twoim CSS a wyjściem.
* Firefox/Chrome: zainstalować programistę stron ([http://chrispederick.com/work/web-developer/](http://chrispederick.com/work/web-developer/)), bezpłatne rozszerzenie dodające wiele ręcznie stworzonych narzędzi przez programistów do twojej przeglądarki.
* Safari 5+: używa inspektora stron (zobacz [https://developer.apple.com/library/safari/documentation/AppleApplications/Conceptual/Safari\_Developer\_Guide/Introduction/Introduction.html](https://developer.apple.com/library/safari/documentation/AppleApplications/Conceptual/Safari\_Developer\_Guide/Introduction/Introduction.html)).
* Chrome: używa narzędzi programisty (zobacz [https://developer.chrome.com/devtools/index](https://developer.chrome.com/devtools/index)).
* Opera 9.5+: używa Dragonfly, w pełni funkcjonalne środowisko debugowania (zobacz [http://www.opera.com/dragonfly/](http://www.opera.com/dragonfly/)).
* Internet Explorer 8+: używa narzędzi programisty (zobacz [http://msdn.microsoft.com/en-us/library/dd565628%28v=vs.85%29.aspx](http://msdn.microsoft.com/en-us/library/dd565628\(v=vs.85\).aspx)).
* Internet Explorer 6 and 7: install the IE Developer Toolbar (see [http://www.microsoft.com/en-us/download/details.aspx?id=18359](http://www.microsoft.com/en-us/download/details.aspx?id=18359)), albo użyj Firebug Lite (zobacz [https://getfirebug.com/firebuglite](https://getfirebug.com/firebuglite)).

Zapewniają one wiele przydatnych narzędzi, wśród których DOM explorer, edytor CSS, network inspector, itp., a to ogromna pomoc podczas debugowania HTML, CSS, JavaScript, i nawet żądań Ajaxa.

### Najlepsze porady <a href="#podstawyrozwojuszablonu-najlepszeporady" id="podstawyrozwojuszablonu-najlepszeporady"></a>

Tutaj znajduje się niewyczerpująca lista najlepszych porad którymi powinieneś się kierować kiedy kreujesz widok:

1. Nie mieszaj kodu HTML i PHP; używaj tagów Smarty w celu uzyskania dynicznej strony.
2. Nie mieszaj kodu HTML i CSS; kod CSS wstawiaj w separator pliku`.css`.
3. Zawsze uprawamacniaj swój kod HTML i CSS używając walidatora W3C: [http://validator.w3.org/](http://validator.w3.org/) dla HTML i XHTML, [http://jigsaw.w3.org/css-validator/](http://jigsaw.w3.org/css-validator/) dla CSS.
4. Nie rób zapytań SQL z kontrolera PHP (`.php` w pliku root PrestaShop); używaj istniejące metody z klasy PrestaShop, albo użyj nowej metody dla tej klasy.
5. Zawsze sprawdzaj czy metoda której potrzebujesz czasem już nie istnieje w dostępnych klasach.
6. Nigdy nie edytuj plików własnych PrestaShop, zawsze twórz swój kod w modułach w celu ułatwienia aktualizacji.
7. Zawsze upewnij się że tworzysz przejrzysty i czytelny kod, na przyszłość twój kod będzie łatwy do odczytania przez inne osoby.
8. Komentarze do kodu i nazwy metod napisz w prostym języku angielskim.
9. Kiedy edytujesz motyw na stronie produkcyjnej sklepu, zawsze pamiętaj żeby najpierw umieścić sklep w trybie konserwacji poprzez panel administracyjny "Konserwacja " w zakładce preferencje.
10. Używaj nowoczesnch przeglądarek takich jak, Firefox (najnowsza wersja non-beta), Google Chrome (najnowsza wersja non-beta), IE10+ albo Opera (najnowsza wersja non-beta) – i upewnij się że twoi znajomi rodzina również!
11. Jeśli to tylko możliwe używaj CSS sprites (czytaj [http://www.alistapart.com/articles/sprites](http://www.alistapart.com/articles/sprites) i  [http://www.alistapart.com/articles/sprites2/](http://www.alistapart.com/articles/sprites2/)).
12. Wyłącz pamieć podręczną swojej przeglądarki kiedy pracujesz.
