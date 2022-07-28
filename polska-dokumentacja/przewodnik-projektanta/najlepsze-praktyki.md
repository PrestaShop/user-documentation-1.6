# Najlepsze praktyki

**Spis treści**&#x20;

/\*\<!\[CDATA\[\*/\
div.rbtoc1597140228022 {padding: 0px;}\
div.rbtoc1597140228022 ul {list-style: disc;margin-left: 0px;}\
div.rbtoc1597140228022 li {margin-left: 0px;padding-left: 0px;}\
\
/\*]]>\*/

* [Najlepsze praktyki ](najlepsze-praktyki.md#Najlepszepraktyki-Najlepszepraktyki)
  * [Patrzeć w przyszłość](najlepsze-praktyki.md#Najlepszepraktyki-Patrzećwprzyszłość)
  * [Projektowanie w Photoshop](najlepsze-praktyki.md#Najlepszepraktyki-ProjektowaniewPhotoshop)
  * [Użyteczność](najlepsze-praktyki.md#Najlepszepraktyki-Użyteczność)
  * [Optymalizacja obrazów](najlepsze-praktyki.md#Najlepszepraktyki-Optymalizacjaobrazów)
  * [Najważniejsze wskazówki SEO](najlepsze-praktyki.md#Najlepszepraktyki-NajważniejszewskazówkiSEO)

## Najlepsze praktyki  <a href="#najlepszepraktyki-najlepszepraktyki" id="najlepszepraktyki-najlepszepraktyki"></a>

Istnieje kilka kroków, które można podjąć, od projektowania motywu w programie PrestaShop do optymalizacji kodu dla wyszukiwarek, które zostały określone jako konieczne do rozwoju tematu. Postepując zgodnie z tymi praktykami można zbudować lepszy motyw.&#x20;

### Patrzeć w przyszłość <a href="#najlepszepraktyki-patrzecwprzyszlosc" id="najlepszepraktyki-patrzecwprzyszlosc"></a>

Przed otwarciem Photoshop, GIMP lub innego edytora graficznego, należy usiąść przy biurku z piórem i arkuszem papieru i pomysleć o mapie strony/hierarchi dla swojego sklepu, dzięki czemu będzie on tak elastyczny jak to tylko mozliwe (nie wszystkie sklepy mają taką samą ilosc kategorii lub produktów w każdej kategorii)&#x20;

Kompletny temat PrestaShop wymaga co najmniej 30 stron i stron sekcji.

* Strona główna
* Strona kategorii&#x20;
* Strona produktu
* Strona porównywarki produktów
* Strona wyników wyszukiwania
* "Moje Konto" i jego wewnętrzne strony:
  * Moje kupony&#x20;
  * Historia zamówień&#x20;
  * Informacje osobiste&#x20;
* "Mój koszyk"
* Strona uwierzytelniena
* Utworzenie konta&#x20;
* Strony zamówienia:
  * Lista adresów Addresses list
  * Koszty wysyłki&#x20;
  * Wybór płatności Payment choice (czek, przelew bankowy)&#x20;
  * Zakup na jednej stronie&#x20;
* Stworzenie adresu&#x20;
* Strona dostawy&#x20;
* Strona konserwacji&#x20;
* Lista producentów i jedna strona producenta&#x20;
* Lista dostawców i strona jednego dostawcy&#x20;
* Strona 404 ("Strony nie znaleziono")&#x20;
* Strona "Najczęściej kupowane"
* Strona "Nowe produkty"&#x20;
* Strona "Aktualne promocje"&#x20;
* Strona "Zapomniałem chasła"&#x20;
* Nota prawna&#x20;
* Mapa strony&#x20;
* Strona sklepów&#x20;
* Formularz kontaktowy&#x20;

Weż te wszystkie sekcje i strony pod uwagę, tak aby o żadnym z nich nie zapomnieć. Nie uwględniając jednej ze stron, może spowodować, że temat będzie niekompletny, a więc będzie to złe doświadczenie dla twoich klientów.

W rzeczywistości, upewnij się, że te 30 plików zostało dodanych.  Aby uzyskać lepszy sens strony, należy wziąc pod uwagę i zgłębić domyślny temat, który zlokalizowany jest w folderze `/themes/default` .Nie ma więcej niż 60 plików szablonów, nie wspominając już o CSS, JavaScript i plikach graficznych wraz z wersją mobilną  (w folderze `/themes/default/mobile` ) który ma swój własny zestaw 58 plików szablonów, wraz z własnym CSS, JavaScript i plikami graficznymi.

Kiedy czujesz się dobrze w hierarchii swojego sklepu i obowiązkowych plików szablonów, zrób kilka szkiców interfejsu, aby zorientować się gdzie zostaną umieszczone różne elementy: Nowe produkty, promocje, obrazy, tekst, etc.). Ponadto zawierają one ważne dane, takie jak wzmianki na stronie produktu: w sprzedaży, promocji nowego produktu, obniżone ceny...)

Oczywiście są to tylko tylko ogólne wkażówki; niektórzy profesjonalisci wolą zrobić to bezpośednio w PrestaShop, a następnie przejść do PHP/Smarty , HTML, CSS

### Projektowanie w Photoshop <a href="#najlepszepraktyki-projektowaniewphotoshop" id="najlepszepraktyki-projektowaniewphotoshop"></a>

Rzadko jesteśmy sami podczas tworzenia tematu: Niezależnie czy robimy to z kolegą, lub klientem jest wiele sytuacji, kiedy będziesz musiał się dzielić swoim proejktem z innymi ludźmi. Dlatego będzie im łatwiej pracować jeśli będą myśleć niestandardowo.&#x20;

Jedną z pierwszych rzeczy do zrobienia jest dostarczenie prac w przestrzeni kolorów RGB w 72 dpi. i  zapewnienie niepłaskiego pliku ( chyba, że jest to dla kilenta końcowego, w takim przypadku, należy podać płaski plik, chyba, że wyraźnie zapłacił za nie spłaszczoną wersję)

Ogólnie rzecz biorąc, nigdy nie należy spłaszczać projektu, chyba że masz pewność, że nie będą chcieli edytować go ponownie.&#x20;

Przy budowie motywu PrestaShop, należy pracować z 980px szerokości w zależności od zastosowań, wraz z&#x20;

* Jeden folder Photoshop dla wszytkich warstw tekstowych, dzięki czemu developrzy mogą łatwo uzyskać dostęp do projektu.
* Jeden folder Photoshop na projektowany blok (nowe produkty, najlepiej sprzedające,etc.).

#### Przestrzeń kolorów <a href="#najlepszepraktyki-przestrzenkolorow" id="najlepszepraktyki-przestrzenkolorow"></a>

Zawsze polegać na RGB. Nigdy nie używać.CMYK, który jest przeznaczony do druku.

#### Jednostki  <a href="#najlepszepraktyki-jednostki" id="najlepszepraktyki-jednostki"></a>

Podczas projektowania strony, jednostką bazową jest piksel. Nie należy mierzyć w picach, punktach lub centymetrach.&#x20;

#### Czcionka <a href="#najlepszepraktyki-czcionka" id="najlepszepraktyki-czcionka"></a>

Nie używaj nietypowych czcionek! Tekst powinien być czytelny w kązdej chwili!

Standardowy teks (tytuł, podtytuł, zwykły tekst) powinny być ograniczone do następujących czcionek, w celu upewnienia się, że wszyscy odwiedzający mogą zobaczyć to samo:

* Arial
* Verdana
* Helvetica
* Georgia
* Tahoma

Sprowadzić liczbę czcionek do mininmum, z obawy przed tym aby strona nie była myląca i nieczytelna.&#x20;

Oczywiście można użyć dowolnej czcionki jakiej chcesz, kiedy projektujesz grafikę. takie jak obraz nagówka, albo pokaz slajdów.&#x20;

#### Rozmiar czcionki <a href="#najlepszepraktyki-rozmiarczcionki" id="najlepszepraktyki-rozmiarczcionki"></a>

Nigdy nie zapominaj, że użytkownik ma decydujący głos w sprawie rozmiaru tekstu, od kiedy w nowych przeglądarkach, można zwiększyć, lub zminiejszyć go za pomocą naciśnięcia jednego klawisza klawiatury&#x20;

W rzeczywistości, należy przetestować swoja stronę z róznymi odmianami przeglądarek, zauważ jak łatwo można złamać twój projekt i dlatego przerób go w celu uniknięcia takiego łatwego pękania.

Można zacząć od garści podstawowych rozmiarów tekstowych:

* Tytuły: 18px.
* Mniejsze tytuły: 14px.
* Regularny tekst: 10 to 12px.

#### Przezroczystości <a href="#najlepszepraktyki-przezroczystosci" id="najlepszepraktyki-przezroczystosci"></a>

Przejrzyste ilustracje nie działają dobrze na starszych przeglądarkach, zwłaszcza w internet Explorer, więc należy trzymać się zdala od 24- bitów PNG. W przypadku obrazów GIF z przezroczystością należy użyć w ciągu zwykłego tła, aby upewnić się, że działa poprawnie. Unikaj 50% krycia przy użyciu tego samego matowego koloru jako koloru tła.&#x20;

#### Różne  <a href="#najlepszepraktyki-rozne" id="najlepszepraktyki-rozne"></a>

* Przetestuj swój temat ze wszystkimi aktywnymi opcjami PrestaShop, aby zobaczyć jak reaguje temat.
* Edytuj produkt, aby zobaczyć jak różne opcje wpływają na projekt ( promocja, nowy produkt, itp...)... jeśli w ogółe.
* Upewnij się że mają jednorodny styl dla twojego sklepu.

### Użyteczność <a href="#najlepszepraktyki-uzytecznosc" id="najlepszepraktyki-uzytecznosc"></a>

Nie będziemy się zagłębiać w skomplikowane teorie interakcji człowiek - komputer, ale raczej będziemy się starali upewnić, że sklep jest dostępny jak to możliwe dla jak największej liczby potencjalnych klientów..Ostatecznym celem powinno być posiadanie zaufanych klientów, którzy będą gwiazdami zakupów.

Za każdym razem gdy użytkownik natrafia na problem użyteczności, witryna traci zaufanie. Ostatecznie jeśli zaufanie osiągnie najniższy punkt.przychodzi frustracja i użytkownik opuszcza stronę, bez kupowania oczywiście czegokolwiek. Takie jest znaczenie użyteczności w świecie e-commerce.

Kiedy projektujesz swój motyw sklepu, należy pamiętać o tym, że jego misją (oprócz oczywiście sprzedaży towarów) jest pokazanie odwiedzającym, że witryna jest zarządana przez poważnych i kompetentnych ludzi.

#### Strona główna <a href="#najlepszepraktyki-stronaglowna" id="najlepszepraktyki-stronaglowna"></a>

To jest **najważniejsza** strona twojego sklepu, która "zaskoczy albo nie". Jest to strona na której użytkownik otrzyma ogólną opinię o twoim sklepie i zdecyduje, czy ma zaufać Tobie swoimi pieniędzmi.&#x20;

Powinineś mieć pewność, że twój sklep jest łatwo rozpoznawalny, i twój katalog będzie pierwszą rzeczą, którą ludzie widzą.

Nagłówek strony jest miejscem, gdzie możesz umieścić najbardziej rozpoznawalne szczegóły: Logo, nazwa,unikalne obrazy...nie powinny być wyżej niż 250px, tak żeby twoi goście mogli obejrzeć twój katalog bez uciekania się do przewijania strony w dół. Innymi słowy główna treść nie powinna być niższa niż zakładka (dowiedz się więcej o zakładce na stronie Wikipedia:: [http://en.wikipedia.org/wiki/Above\_the\_fold](http://en.wikipedia.org/wiki/Above\_the\_fold)).

Wizualny aspekt twojej strony jest oczywiście bardzo ważny (stąd nasza sekcja "Myślenie o przyszłości jest powyżej"): Musisz znaleźć sposób aby umieścić swoje produkty z przodu przewijania strony. Ponadto należy użyć jednorodne kolory i układ w obrębie strony i między stronami. Na przykład, jeśli przycisk ma wpływ na efekt strony, to upewnij się że zastosowałeś ten efekt na wszystkich innych stronach tej witryny.&#x20;

Wyszukiwarka musi być łatwa do znalezienia. Odwiedzający często wiedzą po co przychodzą, i nie chcą przeglądać kategorie i pod kategorie w poszukiwaniu tego po co przyszli.

Mimo to, podczas budowania zawartości witryny, należy, pomyśleć o użytkowniku, który przeszukuje kategorie, i zrobić je proste i intuicyjne.

Można wzmocnić poziom zaufania poprzez wyświetlanie loga lub wzmianki o swoich partnerach (banków, przewoźników), oraz o ocenę od znanych instytucji e-commerce, takich jak  FIA-NET we Francji

Wyświetlaj swoje dane kontaktowe takie jak, numer telefonu albo system chatu.jeśli jest dostępny. To pokaże ci które są prawdziwe, a które mogą stanowić ogormną różnice. \
Oczywiście nie używaj swojego prywatnego numeru telefonu, muszą czuć, że dzwonią do zespołu wsparcia firmy i nie przeszkadzają Tobie w gotowaniu.

Wyświetl wyraźnie warunki zwrotu towaru, swoje ogólne OWU oraz inne obowiązujące przepisy prawa które respektujesz.

#### Strona produktu <a href="#najlepszepraktyki-stronaproduktu" id="najlepszepraktyki-stronaproduktu"></a>

Odwiedzajacy zmierzaja tylko do strony produktu jeśli są zainteresowani tym co on mówi, to chcą więcej szczegółów. Dlatego nie powinno być ich dużo.

Zrób jasny i widoczny przycisk "Dodaj do koszyka". Musi się odróżniać od reszty układu zarówno swoim rozmiarem jak i kolorem - lecz należy zachować jednorodny wygląd: Jeśli przycisk za bardzo różni się od ogólnego projektu, odwiedzjący mogą go łatwo przeoczyć, w taki sam sposób ludzie uczą się nie dostrzegać reklam w internecie.

Upewnij się, że wyświetlają się wszystkie potrzebne etykiety: "Nowy produkt", "Promocje", "Voucher", itp. Ponadto nie zapomnij dodać opóźnień dostawy.

#### Tunel konwersji: "Moje konto"  i strony pokrewne <a href="#najlepszepraktyki-tunelkonwersji-mojekonto-istronypokrewne" id="najlepszepraktyki-tunelkonwersji-mojekonto-istronypokrewne"></a>

Tunel konwersji to miejsce gdzie twoi goście staja się klientami (stąd użycie "konwersji" albo czasami "transformacji"). Jesli te strony są źle zaprojektowane albo źle zbudowane, może to oznaczać, stratę wielu potencjalnych klientów, i dlatego wszystkie zlecenia byłyby wykonane na twojej stronie. Aby dowiedzieć się więcej na temat tunelu konwersji przeczytaj stronę Wikipedii: [http://en.wikipedia.org/wiki/Conversion\_funnel](http://en.wikipedia.org/wiki/Conversion\_funnel).

**Utworzenie konta / "Moje konto"**

Domyślny temat motywu PrestaShop jest wyposażony w formę rachunku, który daje dobry procent transformcji. Ale wciąż może nie spełniać potrzeb twojej strony. Stąd, kilka wskazówek, które należy przestrzegać, jeśli zamierzasz aktualizować jego formę.

* Skup się na podstawach, zachowaj tylko esencje. Odwiedzający musi sie skoncentrować tylko na  stworzeniu konta i zamówieniu. Zobacz jak to robi Amazon.&#x20;
* Zredukuj liczbę kroków. Użytkownik musi wiedzieć ile kroków wciąż musi przejśc aby rzeczywiście zfinalizować zakup.&#x20;
* Wyrażnie wyświetl błedy użytkownika tuż obok pola formularza. Błędy muszą wyświetlać sie odrębnym kolorem (czerwony jest ulubiony), a pola obowiązkowe powinny być wskazane (na przykład gwiazdką \*).

**Płatności**&#x20;

Odwiedzajacy utworzył konto klienta, świetnie! Ale to jeszcze nie koniec, musi teraz przejść przez same zakupy.&#x20;

Tak samo jak w przypadku tworzenia fomularza konta:

* Zredukuj liczbę kroków (adresy dostarczenia, stronę płatności).
* Wyświetl błędy odrębnym kolorem.
* Strona płatności:
  * Jeśli odwiedzajacy używają karty kredytowej, ostrzeż ich, że będą przekierowani do bezpiecznego serwera banku. Na przykład,  dodaj mała ikonę kłódki, wraz z wyjaśnieniem.&#x20;
  * Jeśli wybierają płatność czekiem (lub jakąś inną metode płatności w trybie offline), wytłumacz jasno co mają robić dalejt:  Kwota, adres, etc.

Wszystkie te użyteczne wskazówki, są tylko częsćią całej historii, ale moga Ci przynieść solidną podstawę na której budujesz swój temat, aby poprawić swój sklep.&#x20;

### Optymalizacja obrazów <a href="#najlepszepraktyki-optymalizacjaobrazow" id="najlepszepraktyki-optymalizacjaobrazow"></a>

Ważne jest aby pamiętać, że obrazy spowalniają sklep, zwłaszcza jeśli zdjęcia nie są zooptymalizowane. Ten rozdział pokazuje jak optymalizować obrazy, ale w końcu celem optymalizacji jest zatrzymanie ważnych zdjęć i odpuszczenie innych.\
Jest tylko kilka ważnych obrazów w temacie sklepu: Zdjęcia produktów/miniatury, logo sklepu albo nagłówku, i może slajder strony głównej. Większość z resztą może być łatwo zastąpiona przez inteligentne użycie CSS i HTML, zwłaszcza jeśli należą do projektu sklepu. Zminilmalizuj liczbę obrazów na stronie do minimum, to sklep będzie się szybciej wczytywał. a potencjalny klient będzie skłony dłużej przeglądać twoją stronę.

Optymalizacja obrazu oznacza dwie rzeczy:

* Obniżenie rozmiaru obrazu w celu poprawy czasu ładowania.
* Upewnij się że są poprawnie indeksowane przez wyszukiwarka.

Aby poradzić sobie z rozmiarem obrazu należy dokonać zmian bezpośrednio w programie Photoshop: Nigdy nie używaj większego obrazu niż ten który jest wyświetlany w przeglądarce. Użyj odpowiedniej wielkości nie większej, ani nie mniejszej.\
Photoshop ma specjalne narzędzie "Zachowaj na stronie", które pomaga wykonywać kompresje i porównać format, i usuwa większość pozostałości po danych.

Istnieją też narzędzia online które pomagają optymalizować stratę jakości twojego zdjęcia, wykonując zadanie bezpiecznie i automatycznie:

* Yahoo! [Smush.it](http://smush.it) jest najbardziej znany: [http://www.smushit.com/ysmush.it/](http://www.smushit.com/ysmush.it/)
* Kraken jest kolejny, który czasami może dać lepsze rezultaty i ma rozszerzenia Firefoxa i Chrome: [http://kraken.io/](http://kraken.io/)
* Optymalizator zdjęć umożliwia także zmianę rozmiaru pliku: [http://www.imageoptimizer.net/](http://www.imageoptimizer.net/)

Jeśli przychodzi Ci łatwo użycie narzędzi wiersza polecenia można skorzystać z tych:

* Pngnq: zmienia 24-bitowe pliki PNG na 6 do 8-bitowe, tylko przez utrzymywanie potrzebnych kolorów.\
  Pobierz: [http://pngnq.sourceforge.net/](http://pngnq.sourceforge.net/)\
  Przykładowy wiersz poleceń: `pngnq -vf -s1 image.png`
* OptiPNG: istnieje kilka metod kompresji pliku PNG w celu znalezienia najlepszego.\
  Pobierz: [http://optipng.sourceforge.net/](http://optipng.sourceforge.net/)\
  Przykładowy wiersz poleceń: `optipng -o7 image-nq8.png`
* pngcrush: kolejne narzędzie optymalizacji PNG.\
  Pobierz: [http://pmt.sourceforge.net/pngcrush/](http://pmt.sourceforge.net/pngcrush/)\
  Przykładowy wiersz poleceń: `pngcrush image.png -rem all -reduce -brute result.png`
* jpegtran: Wykonuje bez strat operacje na obrazach JPEG.\
  Pobierz: [http://jpegclub.org/jpegtran/](http://jpegclub.org/jpegtran/)\
  Przykładowy wiersz poleceń: `jpegtran -copy none -optimize -perfect src.jpg dest.jpg`

### Najważniejsze wskazówki SEO <a href="#najlepszepraktyki-najwazniejszewskazowkiseo" id="najlepszepraktyki-najwazniejszewskazowkiseo"></a>

Poprawa pozycji witryny w rankingu jest kluczem do uzyskania nowych klientów. Nie zagłębimy się w tym rozdziale w SEO, istnieje kilka wskazówek do których należy dążyć:

* Poprawa swojego adresu URL i innych meta tagów, upewnij się że wypełnione są wszystkie pola tekstowe w panelu administracyjnym, zarówno dla produktów jak i kategorii. Użyj krótkich i zwięzłych opisów; wypełnij tytuł najważniejszymi szczegółami, aby te dane pojawiły się w adresie URL etc.
* Poprawić wyświetlanie obrazu używając odpowiednich napisów i tytułów.
* Nie wachaj się korzystać z  list HTML podczas nazywania różnych komponentow/cech produktów.
* Użyj ważnych słów kilka razy w opisie produktu..
* Umieść ważny tekst na przodzie za pomocą \<strong> i \<em>.
* Optymalizacja wyświetlanie strony: upewnij sie, że załaduje się ona szybko, albo zminimalizuj rozmiar obrazu za pomocą lepszego narzędzia hostingu. .

Zobacz także bezpłatny przewodnik o SEO PrestaShop: [https://www.prestashop.com/pl/white-paper-seo](https://www.prestashop.com/pl/white-paper-seo)
