# Automatyczna aktualizacja

[Go to start of metadata](http://doc.prestashop.com/display/PS16/Automatic+update#page-metadata-start)

**Spis treści**

* [Automatyczna aktualizacja](automatyczna-aktualizacja.md#Automatycznaaktualizacja-Automatycznaaktualizacja)
  * [Pobieranie i instalacja modułu 1-Click Upgrade](automatyczna-aktualizacja.md#Automatycznaaktualizacja-Pobieranieiinstalacjamodułu1-ClickUpgrade)
  * [Panel konfiguracyjny](automatyczna-aktualizacja.md#Automatycznaaktualizacja-Panelkonfiguracyjny)
    * [Witaj](automatyczna-aktualizacja.md#Automatycznaaktualizacja-Witaj)
    * [Lista punktów do sprawdzenia przed dokonaniem aktualizacji](automatyczna-aktualizacja.md#Automatycznaaktualizacja-Listapunktówdosprawdzeniaprzeddokonaniemaktualizacji)
    * [Rozpocznij aktualizację](automatyczna-aktualizacja.md#Automatycznaaktualizacja-Rozpocznijaktualizację)
    * [Porównanie wersji](automatyczna-aktualizacja.md#Automatycznaaktualizacja-Porównaniewersji)
    * [Powrót](automatyczna-aktualizacja.md#Automatycznaaktualizacja-Powrót)
    * [Opcje kopii bezpieczeństwa](automatyczna-aktualizacja.md#Automatycznaaktualizacja-Opcjekopiibezpieczeństwa)
    * [Opcje aktualizacji](automatyczna-aktualizacja.md#Automatycznaaktualizacja-Opcjeaktualizacji)
  * [Procedura aktualizacji](automatyczna-aktualizacja.md#Automatycznaaktualizacja-Proceduraaktualizacji)
  * [Powrót do poprzedniej wersji](automatyczna-aktualizacja.md#Automatycznaaktualizacja-Powrótdopoprzedniejwersji)
  * [Powrót do poprzedniej wersji: przywracanie Twojej własnej kopii bezpieczeństwa](automatyczna-aktualizacja.md#Automatycznaaktualizacja-PowrótdopoprzedniejwersjiprzywracanieTwojejwłasnejkopiibezpieczeństwa)

## Automatyczna aktualizacja <a href="#automatycznaaktualizacja-automatycznaaktualizacja" id="automatycznaaktualizacja-automatycznaaktualizacja"></a>

Narzędzie Automatycznej aktualizacji pozwala administratorowi sklepu na utworzenie kopii zapasowej i aktualizację PrestaShop za pomocą kilku kliknięć i nie wymaga wiedzy technicznej.

Moduł 1-Click Upgrade jest częścią standardowej instalacji PrestaShop i powienien być dostępny w zakładce "Moduły" panelu administracyjnego. Wystarczy nacisnąć przycisk "Instaluj" znajdujący się obok ikonki tego modułu, żeby zyskać możliwość zaktualizowania sklepu do najnowszej wersji.

Nigdy nie powinno się aktualizować sklepu bez przygotowania. Automatyczna aktualizacja może w pewnych sytuacjach ulec awarii, a przywrócenie poprzedniej wersji może w tej sytuacji się nie powieść.\
Najbezpieczniejszą praktyką jest umieszczenie dokładnych kopii sklepu - jednej na Twoim komputerze lokalnym, a drugiej w osobnym folderze na Twoim serwerze WWW. Taka kopia powinna zawierać wszystkie produkty, kategorie, szablony, moduły, tłumaczenia, pliki konfiguracyjne itd.\
Zalecamy przeprowadzenie próbnej aktualizacji na kopii sklepu. Kiedy proces zostanie zakończony, należy dokładnie przejrzeć sklep i jego funkcjonowanie zarówno od strony użytkownika, jak i od strony panelu administracyjnego, aby upewnić się, że wszystko działa i wygląda jak należy. Jeśli tak nie jest, prawdopodobnie zachodzi jakiś konflikt między narzędziem Automatycznej aktualizacji, a ustawieniami sklepu. W tej sytuacji powinieneś zastosować metodę ręcznej aktualizacji, która choć nie jest już rozwijana i jej zastosowanie zabiera więcej czasu, może okazać się jednak pomocna.&#x20;

### Pobieranie i instalacja modułu 1-Click Upgrade  <a href="#automatycznaaktualizacja-pobieranieiinstalacjamodulu1-clickupgrade" id="automatycznaaktualizacja-pobieranieiinstalacjamodulu1-clickupgrade"></a>

Jeśli modułu 1-Click Upgrade nie ma w Twoim sklepie PrestaShop w wersji 1.4 lub 1.5, możesz pobrać go bezpłatnie ze strony Addons. &#x20;

Nawet jeśli moduł 1-Click Upgrade masz już zainstalowany, upewnij się, że jest to najnowsza wersja tego modułu.

* Jeśli Twój sklep to PrestaShop 1.4: Sprawdź numer wersji w zakładce "Moduły", a następnie porównaj go z numerem  wersji gotowej do pobrania na stronie Addons (więcej informacji na ten temat znajduje się poniżej). Jeśli numery różnią się, pobierz moduł ze strony Addons i zaktualizuj go.
  * W celu zaktualizowania modułu: odinstaluj, a następnie usuń "stary" moduł w zakładce "Moduły" panelu administracyjnego. Dalej, rozpakuj folder skompresowany "nowego" modułu, który pobrałeś ze strony Addons. W utworzonym w ten sposób folderze odszukaj folder "/autoupgrade", a następnie (używając na przykład protokołu ftp) skopiuj go do folderu "/modules" znajdującego się na Twoim serwerze. Następnie zainstaluj moduł 1-Click Upgrade w panelu administracyjnym Twojego sklepu.
* Jeśli Twój sklep to PrestaShop 1.5 lub nowszy: PrestaShop automatycznie sprawdzi, czy wersja modułu, którą posiadasz jest wersją najnowszą. Jeśli dostępna jest nowsza wersja, obok przycisku "Instaluj/Odinstaluj" pojawi się przycisk "Aktualizuj". Naciśnij ten przycisk, aby zaktualizować moduł.

Następnie postępuj tak, jak podczas instalacji typowego modułu:&#x20;

1. Pobierz moduł 1-Click Upgrade ze strony PrestaShop Addons: [http://addons.prestashop.com/en/administration-tools/5496-autoupgrade.html](http://addons.prestashop.com/en/administration-tools/5496-autoupgrade.html). Zapisz plik Zip na pulpicie Twojego komputera.
2. W panelu administracyjnym sklepu najedź kursorem myszy na pozycję "Moduły" w menu głównym, a następnie przejdź do zakładki "Moduły".&#x20;
3.  Kliknij w przycisk "Dodaj nowy moduł"; znajdziesz go w prawym górnym rogu ekranu, powyżej listy modułów.&#x20;

    Jeśli aktualizujesz sklep w wersji 1.4, kliknij w "Dodaj moduł z mojego komputera" umieszczony w w okolicach lewego górnego rogu ekranu, powyżej listy modułów.
4. W okienku, które sie pojawi, w sekcji "Plik modułu" wciśnij przycisk "Przeglądaj", po czym odszukaj i zaznacz plik Zip modułu 1-Click Upgrade, który właśnie pobrałeś.
5. Naciśnij przycisk "Prześlij moduł". PrestaShop prześle plik Zip na serwer, rozpakuje go i umieści pliki modułu w folderze `/modules`.

Moduł został dodany do listy dostępnych modułów. Teraz należy go zainstalować.

1. W zakładce "Moduły" znajdź moduł 1-Click Upgrade: wpisz do pola wyszukiwania w modułach (uwaga: nie do pola wyszukiwania w całym sklepie, znajdującego się u samej góry strony) "1-click upgrade" lub "autoupgrade". Moduł powinien zostać wyszukany jeszcze w momencie pisania. W PrestaShop w wersji 1.4 pojawi sie link do modułu, w który należy kliknąć.
2. Następnie wyświetlona zostanie miniatura modułu na liscie modułów.
3. Teraz wystarczy nacisnąć przycisk "Instaluj".

Moduł jest juz gotowy do konfiguracji i użycia.

### Panel konfiguracyjny <a href="#automatycznaaktualizacja-panelkonfiguracyjny" id="automatycznaaktualizacja-panelkonfiguracyjny"></a>

Panel konfiguracyjny modułu dostępny jest z pozimu listy modułów po naciśnieciu linku "Konfiguruj".&#x20;

Dostęp do panelu konfiguracyjnego modułu uzyskać można również:

* Jeśli Twój sklep to PrestaShop 1.4: po kliknięciu w zakładkę "Narzędzia"  w menu głównym, w pod-zakładce "1-Click Upgrade".
* Jeśli Twój sklep to PrestaShop  1.5 lub nowszy: po najechaniu kursorem na pozycję "Zaawansowane" w menu głównym i rozwinięciu podmenu, należy wybrać pozycję "1-Click Upgrade".

Panel konfiguracyjny składa się z kilku sekcji, zawierających informacje, narzędzia i ustawienia.

#### Witaj <a href="#automatycznaaktualizacja-witaj" id="automatycznaaktualizacja-witaj"></a>

To niewielkie pole zawiera przypomnienie, że aktualizacja nigdy nie jest procesem w stu procentach bezpiecznym, w związku z czym należy utworzyć kopię bezpieczeństwa wszystkich plików i danych składających sie na sklep. W przypadku niepowodzenia aktualizacji, kopia umozliwia przywrócenie Twojego sklepu do stanu początkowego - będzie to wymagało jedynie umieszczenia plików w odpowiednim katalogu na serwerze i wczytania kopii bazy danych.

Procedura przywrócenia sklepu z kopii bezpieczeństwa jest szczegółowo opisana w rozdziale "Tworzenie i przywracanie kopii bezpieczeństwa"  niniejszego przewodnika: [http://doc.prestashop.com/display/PS16/Making+and+restoring+your+own+backup](http://doc.prestashop.com/display/PS16/Making+and+restoring+your+own+backup).

![](<../../.gitbook/assets/23038081 (2).png>)

Należy odnotować, że moduł 1-Click Upgrade tworzy własny zestaw kopii bezpieczeństwa na wypadek konieczności zaniechania lub cofnięcia procesu aktualizacji. Niemnniej jednak zawsze powinno sie polegać przede wszystkim na własnej kopiii bezpieczeństwa.

#### Lista punktów do sprawdzenia przed dokonaniem aktualizacji <a href="#automatycznaaktualizacja-listapunktowdosprawdzeniaprzeddokonaniemaktualizacji" id="automatycznaaktualizacja-listapunktowdosprawdzeniaprzeddokonaniemaktualizacji"></a>

Pole "Lista punktów do sprawdzenia przed dokonaniem aktualizacji" ("The pre-Upgrade checklist") zapewnia rzetelne informacje o Twojej bieżącej instalacji PrestaShop, oraz o możliwych interakcjach między Twoim sklepem, a procedurą automatycznej aktualizacji.

![](<../../.gitbook/assets/23038082 (2).png>)

Przed rozpoczęciem procesu aktualizacji należy upewnić się, że przy każdej pozycji na liście widnieje zielony "ptaszek".

* **W sklepie została zainstalowana najnowsza wersja modułu 1-click upgrade ( twoja wersja v x.x)**. Pozycja ta wskazuje, czy moduł 1-click Upgrade wymaga aktualizacji. Jeśli dopiero co go zainstalowałeś, istnieje raczej niewielka szansa na to, że moduł jest nieaktualny.\
  Jeśli moduł wymaga aktualizacji, poniżej tego pola wyświetla się komunikat "Zainstaluj najnowszą wersję modułu" oraz przycisk "Dodaj moduł z mojego komputera". Naciśnięcie przycisku przeniesie Cię do zakładki "Moduły", W tym miejscu należy nacisnąć znów "Dodaj moduł z mojego komputera", aby wyświetlić wstepnie wypełniony formularz. Następnie należy wcisnąć przycisk "Pobierz ten moduł", aby rozpocząć aktualizację modułu. Po jej zakończeniu można znów przejść na stronę konfiguracji modułu 1-Click Upgrade w celu kontynuowania procedury automatycznej aktualizacji sklepu.
* **Posiadasz uprawnienia do zapisu w katalogu głównym Twojego sklepu (posiadasz właściwe uprawnienia CHMOD) / Your store root directory is writeable (appropriate CHMOD permissions)**. Parametr ten wskazuje, czy uprawnienia dotyczące operacji na plikach umieszczonych na serwerze są ustawione właściwie. Jeśłi nie są, należy zmienić ustawienia na poprawne używając klienta FTP - na przykład FileZilla.\
  Jeśli chcesz dowiedzieć się więcej na temat uprawnień i sposobu ich nadawania, zapoznaj się z sekcją "Kroki 3 i 4: zgodność z systemem i przechowywanie informacji" w przewodniku "[Instalacja PrestaShop](http://doc.prestashop.com/display/PS16/Instalacja+PrestaShop)".
* **Opcja "Tryb bezpieczny" PHP musi być wyłączon**a / The PHP "Safe mode" option must be turned off.
* **Opcja PHP "allow\_url\_fopen"** musi być włączona, lub CURL musi być zainstalowany. / The PHP "allow\_url\_fopen" option must be turned on or CURL must be installed.
* **Musisz ustawić tryb "Przerwa techniczna" w sklepie / You must put your store under maintenance**. Ta pozycja wskazuje, czy sklep jest aktywny, czy też jest w trybie "Przerwa techniczna". Powinieneś włączyć "Przerwę techniczną" na czas aktualizacji (tworzenie kopii zapasowych plików i bazy danych, sam proces automatycznej aktualizacji, weryfikacja), ponieważ zapobiegnie to utracie zamówień (a tym samym możliwe, że również klientów), które mogły by być złozone podczas aktualizacji. Przerwa techniczna sprawia, że nikt nie może złozyć zamówienia w sklepie. Możliwe jest łatwe ustanowienie Przerwy technicznej z poziomu modułu 1-Click Upgrade: wystarczy wcisnąć przycisk "Włącz Przerwę techniczną" ("Click here to put your shop under maintenance"). Możesz również włączyć Przerwę techniczną osobiście na przeznaczonej do tego stronie panelu administracyjnego:\

  * PrestaShop 1.4: włączanie i wyłączanie Przerwy technicznej odbywa sie w głównej zakładce "Ustawienia".
  * PrestaShop 1.5 i nowszy: włączanie i wyłączanie Przerwy technicznej odbywa sie w pod-zakładce "Przerwa techniczna" umieszczonej pod zakładką "Preferencje" w menu głównym.
* **Musisz wyłączyć funkcje PrestaShop związane z pamięcią cache. / You must disable the Caching features of PrestaShop**. Parametr ten wskazuje czy funkcje PrestaShop związane z pamięcią cache są włączone, czy też nie. Podczas aktualizacji powinny pozostać wyłączone; wyłączenie tych funkcji nie jest możliwe z poziomu modułu 1-Click Upgrade.&#x20;
  * PrestaShop 1.4: włączanie i wyłączanie tych funkcji odbywa się w sekcji "Cache" i "Ustawieniach dotyczących Smarty" na pod-zakładce "Optymalizacja" zakładki  "Ustawienia".
  * PrestaShop 1.5 i nowszy: włączanie i wyłączanie tych funkcji odbywa się w sekcji "Cache" i "Ustawieniach dotyczących Smarty" na pod-zakładce "Wydajność" zakładki "Zaawansowane".
* **Limit czasu wykonania skryptu PHP jest wysoki lub wyłączony (Bieżąca wartość: xxx) / The PHP time limit is high or disabled (Current value: xxx)**. Automatyczna aktualizacja może być długotrwałym procesem, ponieważ składają się na niego takie kroki jak pobranie plików instalacyjnych nowego sklepu ze strony [prestashop.com](http://prestashop.com), rozpakowanie pliku Zip., zamiana obecnie zainstalowanych plików na nowe, a następnie autoaktualizacja. Z tego powodu może się okazać, że bieżące (zbyt "niskie") ustawienia PHP spowodują przerwanie procesu aktualizacji i fiasko całego przedsięwzięcia. Z tego względu zanim jeszcze rozpocznie sie aktualizacja, PrestaShop daje swoim użytkownikom informację, jakie są obecne ustawienia PHP. Najlepiej byłoby, gdyby parametr "Limit czasu wykonania skryptu PHP" przybrał wartość "wyłączone" ("disabled").

Wszystkie powyższe pozycje listy kontrolnej musza być zaznaczone na zielono. W przeciwnym wypadku przycisk aktualizacji nie wyświetli się.&#x20;

Jeśli przeprowadzasz aktualizacje sklepu zainstalowanego na Twoim komputerze ([`http://localhost`](http://localhost/) lub [`http://127.0.0.1`](http://127.0.0.1/)), a nie na serwerze WWW, moduł 1-Click Upgrade wykrywa, że tryb Przerwy technicznej nie musi być wprowadzany, ponieważ nikt poza Tobą i tak nie ma dostępu do sklepu. Z tego względu, nawet jeśli nie włączyłeś w sklepie Przerwy technicznej, moduł oznaczą ten warunek na liście kontrolnej jako spełniony.

#### Rozpocznij aktualizację <a href="#automatycznaaktualizacja-rozpocznijaktualizacje" id="automatycznaaktualizacja-rozpocznijaktualizacje"></a>

W tej sekcji odbywa się porównanie bieżącej wersji Twojego sklepu z wersją najnowszą. Możesz dzięki temu szybko ocenić, czy aktualizacja jest naprawdę potrzebna. Jeśli wiesz, że opublikowano już wersję nowszą niż tę, którą moduł wyświetla jako najnowszą (obok pola "Latest official version for major channel"), możesz sprawdzić czy ta najnowsza wersja jest dostępna do wykorzystania dla modułu 1-Click Upgrade naciskając przycisk "Sprawdź czy jest dostępna nowa wersja".

![](<../../.gitbook/assets/23038083 (2).png>)

Moduł jest domyślnie ustawiony tak, aby jako docelową wskazywał wersję następną w ramach bieżącej "gałęzi" ("Gałęzie" to fundamentalne wersje PrestaShop: 0.9, 1.0, 1.1, 1.2, 1.3, 1.4 itd). Oznacza to, że jeśli używasz na przykład wersji 1.4.x, to moduł nie zasugeruje Ci aktualizacji do wersji 1.6.x, ale do najnowszej wersji gałęzi 1.4, czyli do 1.4.11.1. Dlatego też jeśli chcesz w tej sytuacji zaktualizować sklep do wersji 1.6.x, powinieneś wcisnąć przycisk "Więcej opcji (Tryb eksperta)", co zapewni Ci dostęp do wyższych gałęzi oprogramowania.\
Ta opcja jest szczególnie użyteczna, jeśli chciałbyś wypróbować wersję inną niż stabilną (czyli na przykład wersję beta czy RC).

Przed uruchomieniem aktualizacji należy dobrze zrozumieć jej parametry. Sekcje "Opcje kopii zapasowej"  i "Opcje aktualizacji" wyświetlane są u dołu strony konfiguracji modułu 1-Click Upgrade i opisane w dalszej części niniejszego przewodnika. Upewnij się, że wszystkie one są dla Ciebie zrozumiałe.

**Więcej opcji (Tryb eksperta)**&#x20;

Ta sekcja pozwala Ci na wybranie dokładnej wersji PrestaShop, do której będzie przeprowadzona aktualizacja.

![](<../../.gitbook/assets/23038084 (2).png>)

Mamy tu do czynienia z następującymi opcjami:

* **Kanał**. W tym miejscu wskazujesz kanał dystrybyucji, który chcesz użyć. Zalecanym wyborem jest "Wydanie poboczne". Oznacza ono "pierwszą w kolejności stabilną wersję nowszą niż wersja bieżąca". Pozostałe opcje to:
  * **Główne wydanie**. Pierwsza w kolejności stabilna wersja najnowszej gałęzi: ponieważ w chwili pisania tego przewodnika najnowszą gałęzią jest 1.6, moduł automatycznie wybierze wersję 1.6.0 - pierwszą wersję stabilną tej gałęzi.
  * **Wydanie poboczne**. Ten kanał dystrybucji jest zaznaczony jako domyślny. Oznacza on pierwszą w kolejności stabilną wersję nowszą niż wersja bieżąca. Jeśli chcesz zaktualizować PrestaShop 1.4.2 i zaznaczysz tę opcję, po aktualizacji otrzymasz wersję 1.4.9, mimo że najnowszą wersją w ogóle jest wersja 1.6.2.
  * **Kandydaci do wydania (RC)**. Wersje RC są stabilne na tyle, żeby mogła testować je większość użytkowników, ale zarazem na tyle niestabilne, że nie mogą jeszcze stać się oficjalnym wydaniem. Używasz ich na własne ryzyko.
  * **Wydania Beta i wydania Alpha**. Są to wersje deweloperskie. Używasz ich na własne ryzyko.
  * **Wydania prywatne ("Private release")**. Niekiedy deweloperzy PrestaShop udostępniają do pobrania prywatne wersje testowe. Jeśli znasz poprawny URL oraz klucz hash, możesz łatwo zaktualizować swój sklep do danej wersji używając tego kanału. Zaznaczając opcję "Pozwól na główną aktualizację" pozwalasz na aktualizację jedynie głównych wydań.
  * **Lokalne archiwum**. Kanału tego można użyć w sytuacji, kiedy chcemy zaktualizować sklep do jakiejś konkretnej wersji. Aby to zrobić, musimy plik instalacyjny (zip) sklepu w pożądanej wersji umieścić na naszym serwerze WWW w folderze `/admin/autoupgrade/download`. Po wskazaniu  na liście rozwijanej właściwego pliku Zip (jeśli w folderze /admin/autoupgrade/download znajduje się więcej niz jeden plik) należy w polu obok wpisać dokładny numer wersji (uwaga: należy zrobić to bardzo dokładnie!).&#x20;
  * **Lokalny katalog**. Ten kanał przeznaczony jest do przeprowadzenia aktualizacji z użyciem pobranej, a następnie wypakowanej do folderu /admin/autoupgrade/latest/prestashop instalacji PrestaShop. Katalog /prestashop musi być dokładnie tym, co otrzymujemy po rozpakowaniu pliku Zip z interesującą nas instalacją.&#x20;
* **gałąź**. Wskazuje, czy w wybranym kanale dostępna jest jakakolwiek gałąź.
* **nazwa (name)**. Nazwa najnowszej wersji dostępnej w wybranym kanale.
* **url**. Adres url najnowszej wersji dostępnej w wybranym kanale.
* **md5**. Hash do ewentualnej weryfikacji poprawności i autentyczności najnowszej wersji dostępnej w wybranym kanale.

#### Porównanie wersji <a href="#automatycznaaktualizacja-porownaniewersji" id="automatycznaaktualizacja-porownaniewersji"></a>

W tej sekcji wyświetlana jest liczba róznic między bieżącą wersją, a najnowszą wersją dostępną w wybranym kanale.&#x20;

![](<../../.gitbook/assets/23038085 (3).png>)

Jeśli w Twoim sklepie podczas prac deweloperskich zamiast wykorzystania możliwości związanych z metodą override zostały zmienione pliki kluczowe (core files), listy zmian dostępne pod przyciskiem "Zobacz lub ukryj listę" pomogą Ci przekonać się, czy zmiany te zostaną zachowane czy znikną po zakończeniu aktualizacji.\
Tak czy inaczej, możesz zwiększyć szanse zmian w Twoim sklepie na przetrwanie aktualizacji przez wprowadzanie ich do kodu sklepu metodą override. Więcej informacji na ten temat znajduje się w dokumentacji dla deweloperów.

#### Powrót <a href="#automatycznaaktualizacja-powrot" id="automatycznaaktualizacja-powrot"></a>

Ta sekcja pojawia się po przeprowadzeniu przynajmniej jednej aktualizacji.

Poniżej znajdziesz więcej informacji na ten temat.

#### Opcje kopii bezpieczeństwa <a href="#automatycznaaktualizacja-opcjekopiibezpieczenstwa" id="automatycznaaktualizacja-opcjekopiibezpieczenstwa"></a>

Poniższe opcje pozwalają Ci w pewnym stopniu kontrolować proces tworzenia kopii bezpieczeństwa:

* **Kopia plików i bazy danych / Backup my files and database**. Koniecznie trzeba zachować kopię swoich plików, toteż moduł automatycznie utworzy taką kopię. Nie należy wyłączać tej opcji w żadnym wypadku poza tym, kiedy zostanie to wprost wyrażone w instrukcji PrestaShop.
* **Kopia obrazów / Backup my images**. W celu zapewnienia sobie bezpiecznego powrotu do bieżącej wersji w razie gdyby aktualizacja nie powiodła się, ta opcja również powinna być włączona.

![](<../../.gitbook/assets/23038086 (2).png>)

#### Opcje aktualizacji <a href="#automatycznaaktualizacja-opcjeaktualizacji" id="automatycznaaktualizacja-opcjeaktualizacji"></a>

Poniższe opcje pozwalają w pewnej mierze kontrolować proces aktualizacji:

* **Wydajność serwera**. Niektóre usługi hostingu świadczone na współdzielonym serwerze WWW są w stanie zapewnić jedynie niewielką efektywność, która z kolei może utrudnić proces aktualizacji, a w pewnych przypadkach spowodować jego zupełne niepowodzenie. Z tego względu domyślna pozycją tej opcji jest "Niska (zalecana)". Jeśli jednak parametry Twojego serwera są odpowiednio wysokie, możesz zaznaczyć opcję "Średnia" lub nawet "Wysoka".&#x20;
* **Wyłącz nie-wbudowane moduły**. Zalecamy wybrać opcję "Tak" dla tego parametru, ponieważ niektóre moduły mogą utrudniać proces aktualizacji.
* **Aktualizuj domyślny szablon / Upgrade the "default" theme**. W procesie aktualizacji bieżący szablon domyślny zostaje wymieniony na najnowszy. Jeśli wprowadziłeś zmiany bezpośrednio do szablonu domyślnego, możesz zachować je zaznaczając opcję "Nie". Tytułem przypomnienia chcielibyśmy dodać, że NIE zaleca się dokonywania zmian bezpośrednio w szablonie domyślnym. Najpierw należy go skopiować, a następnie wprowadzać zmiany już na kopii.
* **Zaktualizuj domyślne e-maile**. Aktualizacja może zmienić domyślne szablony e-maili. Domyślnie, aktualizacja zastąpi istniejące szablony szablonami pobranymi z nowej instalacji PrestaShop. Jeśli korzystasz z własnych szablonów, zalecamy ich zachowanie. W przeciwnym razie będziesz musiał po aktualizacji spersonalizować nowe szablony tak, żeby odpowiadały Twoim potrzebom.
* **Tryb "Krok po kroku" / Step-by-step mode**. Tryb dla deweloperów. __ Włączenie tej opcji spowoduje, ze moduł będzie żądał potwierdzenia każdego kroku aktualizacji.
* **Wyświetlaj błędy PHP / Display PHP errors**. Tryb dla deweloperów. __ Włączenie tej opcji spowoduje, ze moduł będzie wyświetlał błędy PHP, co może pomóc w wykrywaniu problemów z serwerem, które w innych okolicznościach mogłyby pozostać nie wykryte.

![](<../../.gitbook/assets/23038087 (2).png>)

### Procedura aktualizacji <a href="#automatycznaaktualizacja-proceduraaktualizacji" id="automatycznaaktualizacja-proceduraaktualizacji"></a>

Kiedy wszystkie pozycje na liście punktów do sprawdzenia przed dokonaniem aktualizacji są zaznaczone na zielono, w sekcji Rozpocznij aktualizację pojawi się przycisk "Upgrade PrestaShop now!"powyżej adresu URL, po naciśnięciu którego można pobrać nową wersję PrestaShop.

Kliknięcie w przycisk "Upgrade PrestaShop now !" rozpocznie proces aktualizacji.

W toku aktualizacji strona konfiguracji modułu jest zastąpiona przez dwie sekcje: ("Logi aktywności") ("Activity Log") i "Powrót" ("Rollback").

Logi aktywności to szczegółowy, tworzony na bieżąco raport z postępu aktualizacji. Poszczególne dane zorganizowane są w następujących sekcjach:

* Usunięte pliki (Removed files): usuwane są jedynie pliki przykładowe, takie jak puste klasy i kontrolery.
* Nazwa plików zip. kopii bezpieczeństwa (Name of the backup archive): nazwa ta nadawana jest w formacie, który ilustruje następujący przykład - `auto-backupfiles_V1.6.0.2_20140127-120310-798d3a69.zip`. Analizując nazwę można poznać datę i godzinę powstania pliku.
* Pliki dodane do pliku zip. kopii bezpieczeństwa (Files added to the backup archive): wszystkie pozostałe pliki składające się na Twoja bieżącą wersję PrestaShop zostają dodane do pliku zip. kopii bezpieczeństwa.&#x20;
* Tabele bazy danych dodane do pliku zip. kopii bezpieczeństwa (Database tables added to the backup archive): jakkolwiek pliki składające się na Twoja bieżącą wersję PrestaShop są bardzo ważne, cały Twój katalog produktów zapisany jest w bazie danych. Dlatego też tabele bazy danych są również dodane do tego samego  pliku zip. kopii bezpieczeństwa.&#x20;
* Usunięte pliki (Removed files): są to głównie pliki modułów, kontrolery, klasy, pliki CSS i JavaScript. Na tym etapie aktualizacji, skoro wszystkie pliki sklepu zostały zapisane do pliku zip. kopii bezpieczeństwa, mogą teraz zostać bezpiecznie usunięte.&#x20;
* Pliki skopiowane z instalacji nowej wersji sklepu (Files copied from the new archive): wszystkie istniejące pliki są zastępowane przez ich nowe wersje pochodzące z nowej wersji PrestaShop.&#x20;
* Połączone pliki tłumaczeń (Merged translation files).
* Utworzone, usuniete, zmienione i zaktualizowane tabele bazy danych (Created, deleted, altered and updated database tables).
* Opróżnione katalogi czasowe (Emptied temporary folders): o ile to możliwe, moduł 1-Click Upgrade będzie próbował usunąć zawartość katalogów cache.

Podczas trwania procesu aktualizacji wyświetlone zostaną informacje o bardzo wielu plikach. Nie musisz czytać wszystkich powiadomień, ponieważ pojawiają się one na wypadek konieczności dochodzenia przyczyn ewentualnych błędów.

Pojawienie się komunikatu "Aktualizacja zakończona. Proszę sprawdzić czy sklep funkcjonuje poprawnie (spróbować złożyć zamówienie, sprawdzić poprawność szablonu)"  ("Upgrade complete. Please check your front office theme is functional (try to make an order, check theme)") oraz ostatniego wpisu na liście logów aktywności o treści "End of process" oznacza zakończenie procesu aktualizacji.\
Moduł automatycznej aktualizacji powinien teraz wyświetlić również komunikat o możliwości wyprowadzenia sklepu z trybu przerwy technicznej. Zanim jednak zdecydujesz się to zrobić, powinieneś sprawdzić, czy wszystko działa poprawnie w panelu administracyjnym: nie ma tam żadnych błędów, wszystkie produkty i kategorie, a także przypisane do nich zdjęcia, pliki załączników itp. są we właściwych miejscach. Dopóki nie sprawdzisz, że wszystko jest w porządku, lepiej jest utrzymywać sklep w trybie Przerwy technicznej.&#x20;

Podczas pierwszego załadowania strony sklepu mogą wyglądać na zniekształcone: jest tak dlatego, ponieważ Twoja przeglądarka internetowa przechowuje pliki często odwiedzanych stron w pamięci cache i próbuje załadować pliki CSS starej wersji sklepu, które trzyma w pamięci. W tej sytuacji, aby uzyskać prawidłowy widok strony sklepu, należy ją kilkukrotnie odświeżyć albo nawet opróżnić pamięć cache przeglądarki (w wielu przeglądarkach pomocne będzie jednoczesne wciśnięcie klawisza Ctrl i F5). &#x20;

Po zakończeniu aktualizacji z wersji 1.4 do wersji 1.6, Twoje menu nie będą zorganizowane tak, jak w "czystej", świeżo zainstalowanej wersji 1.6.&#x20;

Dzieje się tak, ponieważ menu występujące w PrestaShop 1.4 ma postać zakładek poziomych, a w PrestaShop 1.6 przyjmuje postać zakładek rozłożonych pionowo, przy czym wiele stron dotąd powiązanych z jednymi zakładkami, zostało powiązanych z innymi zakładkami po to, aby całe menu było lepiej czytelne i bardziej spójne. Dodatkowo, moduł 1-Click Upgrade działa zgodnie z założeniem, że zakładki pochodzące  z wersji 1.4 mogą zostać spersonalizowane, a także zmienić swoje położenie - zarówno wskutek działania samego modułu, jak i administratora sklepu. Z tego względu moduł aktualizacji zamiast burzyć porządek zakładek pochodzących z wersji 1.4, przenosi go w niezmienionym stanie do wersji 1.6.&#x20;

Jeśli dokonałeś aktualizacji z wersji 1.4 do wersji 1.6 i chcesz zmienić pozycję (czyli kolejność na liście lub przyporządkowanie zakładce nadrzędnej) poszczególnych stron w menu, przejdź do strony "Menu" dostępnej po najechaniu kursorem na pozycję "Administracja" w menu głównym. Edytując poszczególne elementy menu możesz posłużyć się metodą  "przeciągnij i upuść".

Kiedy uzyskasz pewność, że Twój  PrestaShop po aktualizacji działa poprawnie, możesz zacząć przywracać sklep do normalnego funkcjonowania odwołując tryb "Przerwa techniczna" na stronie "Przerwa techniczna" dostępnej po najechaniu kursorem na  na pozycję "Preferencje" w menu głównym. Po wyłączeniu Przerwy technicznej przeprowadź kilka testów: poprzeglądaj produkty, sprawdź, jak działa ich wyszukiwanie, sortowanie, filtrowanie. W skrócie: spróbuj zamówić jakiś produkt po to, by upewnić, się, że złożenie zamówienia w sklepie jest możliwe i przebiega bez problemów. Jeśli to możliwe, wypróbuj wszystkich przewoźników i wszystkie metody płatności.

**Czy wszystko działa prawidłowo? Gratulacje! Właśnie udało Ci się z powodzeniem zaktualizować Twój PrestaShop!**&#x20;

Błąd JavaScript (JavaScript error)&#x20;

Przy pewnych ustawieniach serwera, po wciśnięciu przycisku "Upgrade PrestaShop now !" może pojawić się komunikat błędu: "Javascript error (parseJSON) detected for action "upgradeNow". Starting restoration...".

Podjęcie następujących działań pozwoli Ci rozwiązać ten problem:

* Otwórz plik konfiguracyjny `php.ini` i włącz (aktywuj) rozszerzenia MySQLi i MySQL PDO. Jeśli nie masz dostępu do pliku php.ini, skontaktuj się w tej sprawie z Twoim dostawcą usług hostingowych.
*   W plikach Twojego sklepu otwórz plik `/modules/autoupgrade/db/Db.php` i znajdź poniższy kod (w okolicach 210 wiersza):

    | `public` `static` `function getClass(){    $class` `= 'MySQL';    /*if (PHP_VERSION_ID >= 50200 && extension_loaded('pdo_mysql'))        $class = 'DbPDO';    else if (extension_loaded('mysqli'))        $class = 'DbMySQLi';*/    return` `$class;}` |
    | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |

    Wystarczy, że "odkomentujesz" te wiersze (usuwając znaczniki /\* oraz \*/ ). Powinny one wyglądać teraz tak jak poniżej:&#x20;

    | `public` `static` `function getClass(){    $class` `= 'MySQL';    if` `(PHP_VERSION_ID >= 50200` `&& extension_loaded('pdo_mysql'))        $class` `= 'DbPDO';    else` `if` `(extension_loaded('mysqli'))        $class` `= 'DbMySQLi';    return` `$class;}` |
    | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |

Po zapisaniu zmian do pliku, możesz wznowić proces automatycznej aktualizacji.

### Powrót do poprzedniej wersji <a href="#automatycznaaktualizacja-powrotdopoprzedniejwersji" id="automatycznaaktualizacja-powrotdopoprzedniejwersji"></a>

Niestety, nie wszystkie aktualizacje kończą się powodzeniem - co między innymi jest powodem tego, że przystępując do aktualizacji należy **zawsze** tworzyć kopie bezpieczeństwa, mimo że PrestaShop w ramach procesu aktualizacji sam tworzy własną kopię wszystkich plików i tabel bazy danych. **Zanim przystąpisz do aktualizacji, zrób własną kopię bezpieczeństwa**. Jeśli potrzebujesz dodatkowych informacji na ten temat, znajdziesz je w rozdziale "Tworzenie i przywracanie kopii bezpieczeństwa" niniejszego przewodnika.

Kopie bezpieczeństwa, które w toku aktualizacji tworzy moduł 1-Click Upgrade, przechowywane są na tym samym serwerze, na którym zainstalowany jest sklep podlegający aktualizacji i jeśli aktualizacja nie powiedzie się, dokładną lokalizację tych kopii można odnaleźć w sekcji "Powrót" ("Rollback") panelu konfiguracyjnego modułu 1-Click Upgrade. \
Pliki kopii bezpieczeństwa są tworzone bezpośrednio po rozpoczęciu procesu aktualizacji i dostępne są natychmiast na liście rozwijanej obok napisu "Wybierz swoją kopię zapasową".

Wybieraj zawsze tę najnowszą. Data i godzina utworzenia kopii bezpieczeństwa jest zapisana w jej nazwie zgodnie ze schematem "Vwersja-data-godzina-inne dane". Na przykład z pliku o nazwie: "V1.4.9.0\_20120907-114024-f85f41a" możemy dowiedzieć się, że jest to kopia PrestaShop w wersji 1.4.9, utworzona 7 września 2012 o godzinie 11:40:24.

Naciśnięcie przycisku "Powrót" powoduje rozpoczęcie dwóch procesów:&#x20;

* Zastąpienie aktualnie istniejących plików składających się na sklep, plikami pobranymi z ostatnio utworzonej kopii bezpieczeństwa.&#x20;
* Zastąpienie aktualnie istniejących wpisów w bazie danych sklepu, wpisami pobranymi z ostatnio utworzonej kopii bezpieczeństwa.&#x20;

W celu przywrócenia sklepu do postaci sprzed aktualizacji zaznacz kopię bezpieczeństwa pochodzącą ze sklepu sprzed aktualizacji i wciśnij przycisk "Powrót". Podobnie jak podczas aktualizacji, na ekranie wyświetlają się jedynie sekcje "Logi aktywności" oraz "Powrót". Możesz śledzić postęp procesu powrotu do stanu sprzed aktualizacji w tworzonym na bieżąco raporcie, który po zakończeniu procedury wyświetli komunikat o jej końcu. Należy wówczas sprawdzić, czy przywrócenie wersji poprzedniej zakończyło się sukcesem i sklep działa prawidłowo - jak przed aktualizacją.

### Powrót do poprzedniej wersji: przywracanie Twojej własnej kopii bezpieczeństwa <a href="#automatycznaaktualizacja-powrotdopoprzedniejwersji-przywracanietwojejwlasnejkopiibezpieczenstwa" id="automatycznaaktualizacja-powrotdopoprzedniejwersji-przywracanietwojejwlasnejkopiibezpieczenstwa"></a>

Zagadnienie to wyjaśnione zostało szczegółowo w rozdziale niniejszego przewodnika zatytułowanym "Tworzenie i przywracanie Twojej własnej kopii bezpieczeństwa": [http://doc.prestashop.com/display/PS16/Making+and+restoring+your+own+backup](http://doc.prestashop.com/display/PS16/Making+and+restoring+your+own+backup).

&#x20;[ Like](http://doc.prestashop.com/display/PS16/Automatic+update)Be the first to like this

* No labels
* [Edit Labels](http://doc.prestashop.com/display/PS16/Automatic+update)
