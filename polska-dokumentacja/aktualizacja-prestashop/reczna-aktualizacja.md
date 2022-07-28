# Ręczna aktualizacja

**Spis treści**

* [Ręczna aktualizacja](reczna-aktualizacja.md#Ręcznaaktualizacja-Ręcznaaktualizacja)
  * [Szybkie instrukcje](reczna-aktualizacja.md#Ręcznaaktualizacja-Szybkieinstrukcje)
  * [Krok 1 - Utwórz kopię bezpieczeństwa Twojego sklepu i zapisz ją ](reczna-aktualizacja.md#Ręcznaaktualizacja-Krok1-UtwórzkopiębezpieczeństwaTwojegosklepuizapiszją)
  * [Krok 2 - Przygotuj się na nową wersję](reczna-aktualizacja.md#Ręcznaaktualizacja-Krok2-Przygotujsięnanowąwersję)
  * [Krok 3 – Rozpoczęcie Aktualizacji](reczna-aktualizacja.md#Ręcznaaktualizacja-Krok3–RozpoczęcieAktualizacji)
  * [Krok 4 - QA i Testowanie](reczna-aktualizacja.md#Ręcznaaktualizacja-Krok4-QAiTestowanie)
  * [Krok 5 - Rozpoczęcie aktualizacji na twoim sklepie](reczna-aktualizacja.md#Ręcznaaktualizacja-Krok5-Rozpoczęcieaktualizacjinatwoimsklepie)
  * [Krok 6 - QA i Testowanie](reczna-aktualizacja.md#Ręcznaaktualizacja-Krok6-QAiTestowanie)
  * [Krok 7 - Aktywacja twojego sklepu](reczna-aktualizacja.md#Ręcznaaktualizacja-Krok7-Aktywacjatwojegosklepu)

**TA METODA AKTUALIZACJI NIE JEST JUŻ ROZWIJANA I WSPIERANA.**\
**JEŚLI TO TYLKO MOŻLIWE, NALEŻY UŻYĆ DARMOWEGO MODUŁU** [**1-CLICK UPGRADE**](http://addons.prestashop.com/en/administration-tools-prestashop-modules/5496-1-click-upgrade-autoupgrade.html)**.**

Przeczytaj [instrukcję automatycznej aktualizacji](http://doc.prestashop.com/display/PS16/Automatyczna+aktualizacja). Automatyczna aktualizacja jest jedyną oficjalnie zalecaną metodą aktualizowania PrestaShop.

## Ręczna aktualizacja <a href="#recznaaktualizacja-recznaaktualizacja" id="recznaaktualizacja-recznaaktualizacja"></a>

Przeprowadzanie ręcznej aktualizacji jest długim i złożonym procesem, który powinien być stosowany jedynie z konieczności - na przykład kiedy dokonanie automatycznej aktualizacji nie jest możliwe.&#x20;

Z tego względu ręczna aktualizacja powinna być procedurą zarezerwowana dla ekspertów, czyli osób potrafiących korzystać z narzędzi deweloperskich takich jak WAMP, phpMyAdmin itp. Jeśli nie jesteś ekspertem, możesz poprosić o pomoc kolegę, lub zapłacić za pomoc zawodowemu deweloperowi. Należy spodziewać się, że ręczna aktualizacja może potrwać dwie godziny, lub nawet więcej. Zarezerwuj sobie czas, żeby doprowadzić procedurę do końca.

Główna idea ręcznej aktualizacji jest prosta: zamiast ryzykować bezpośrednią aktualizację Twojego sklepu, przeprowadzimy całą procedurę na Twoim komputerze lokalnym, używając zainstalowanego na nim serwera PHP i MySQL, takiego jak WAMP czy XAMPP. Jeśli uda się zaktualizować Twój sklep lokalnie, trzeba będzie przeprowadzić ten sam proces jeszcze raz - tym razem na Twoim serwerze WWW.

Od rozpoczęcia procesu, Twój sklep powinien być wyłączony (czyli działać w trybie "Przerwa techniczna") po to, aby klienci, którzy mogliby w tym czasie robić zakupy w Twoim sklepie, nie utracili swoich zamówień. Oznacza to, ze podczas wykonywania ręcznej aktualizacji, czyli w okresie około dwu godzin, w Twoim sklepie nie będzie można robić zakupów.

### Szybkie instrukcje <a href="#recznaaktualizacja-szybkieinstrukcje" id="recznaaktualizacja-szybkieinstrukcje"></a>

Ta niezbyt obszerna sekcja jest skierowana jest do osób już zaznajomionych z instalacją i aktualizacją na serwerze aplikacji web wykonanych w technologii PHP/MySQL. Jeśli nie czujesz się komfortowo ze względu na brak wiedzy o szczegółach, kompletne instrukcje postępowania znajdziesz w sekcjach poniżej.&#x20;

Wiele prezentowanych tu procedur wykonuje się na lokalnym serwerze WWW, zainstalowanym na Twoim komputerze. Zanim zaczniesz cokolwiek robić, pobierz i zainstaluj lokalny serwer. Może to być WAMP, XAMPP, EasyPHP, MAMP albo jeszcze inny. Jeśli nigdy wcześniej nie instalowałeś serwera na swoim komputerze, przeczytaj rozdział zatytułowany "Czego potrzebujesz, by zacząć" przewodnika "Początek", a zwłaszcza rozdział "Instalacja PrestaShop" dostępny pod adresem [http://doc.prestashop.com/display/PS16/Instalacja+PrestaShop](http://doc.prestashop.com/display/PS16/Instalacja+PrestaShop)

Proces aktualizacji ręcznej składa się z następujących kroków:

1. Utwórz kopię bezpieczeństwa Twojego sklepu i zapisz ją:
   * Wyłącz sklep (przejdź do trybu "Przerwa techniczna"; opcja ta dostępna jest na różnych stronach w zależności od wersji PrestaShop - dla wersji 1.4 na stronie "Ustawienia" w sekcji "Ustawienia ogólne" pozycja "Włacz sklep"; dla wersji 1.5 na stronie "Przerwa techniczna" pod pozycją "Preferencje" w menu głównym).
   * Korzystając z klienta FTP połącz się ze swoim zdalnym serwerem WWW i skopiuj wszystkie pliki i foldery wraz z zawartością umieszczone w folderze głównym Twojego sklepu do dopiero co utworzonego folderu  "prestashop-prod" na pulpicie Twojego komputera. Będzie to kompletna kopia plików składających się na Twój sklep.
   * Utwórz kopię bazy danych podłączonej do sklepu (w każdej wersji PrestaShop można do tego celu użyć phpMyAdmin, albo wbudowanego narzędzia w panelu administracyjnym sklepu: dla PrestaShop 1.4: strona "Narzędzia / Kopie zapasowe"; dla PrestaShop 1.5 - strona "Zaawansowane / Backup bazy danych").
   * Utwórz kopię specyficznych dla Twojego sklepu tłumaczeń (dla PrestaShop 1.4: sekcja "Export języka" na stronie "Narzędzia / Tłumaczenia"; dla PrestaShop 1.5 - sekcja "Export języka" na stronie "Lokalizacja / Tłumaczenia").
2. Przygotuj się na nową wersję:
   * Pobierz i rozpakuj najnowsza wersję PrestaShop: [https://www.prestashop.com/pl/pobranie](https://www.prestashop.com/pl/pobranie). Wypakowane pliki umieść w dopiero co utworzonym na pulpicie folderze "prestashop-prep".
   * Skopiuj Twoje "osobiste" pliki (zdjęcia produktów, loga, obrazki przypisane do kategorii, tłumaczenia, moduły itp) z "prestashop-prod" do "prestashop-prep" na pulpicie Twojego komputera. Szczegółowa lista dostępna jest w dalszej części tego przewodnika.
   * Skopiuj folder "prestashop-prep" do folderu web Twojego lokalnego serwera (`/htdocs`, `/www`, albo inny folder używany przez serwer, który zainstalowałeś). To właśnie w tej lokalizacji będziesz aktualizować swój sklep przy w pełni zachowanej kopii bezpieczeństwa (prestashop-prod)
   * Odtwórz bazę danych Twojego sklepu na serwerze lokalnym: korzystając z phpMyAdmin utwórz nową pustą bazę danych, do której skopiuj następnie dane z bazy skopiowanej w Twoim sklepie na samym początku procedury.&#x20;
3. Rozpocznij lokalną aktualizację:
   * Uruchom skrypt aktualizacji na Twoim lokalnym serwerze za pośrednictwem przeglądarki internetowej. W PrestaShop w wersji 1.6 skrypt ten umieszczony jest na końcu ścieżki  `/install/upgrade/upgrade.php`.
   * Sprawdź parametry aktualizacji przed jej rozpoczęciem: podążaj za wskazówkami wyświetlanymi na ekranie i upewnij się, ze serwer spełnia wymagania techniczne stawiane przez nową wersję.&#x20;
   * Zakończ aktualizację: po otrzymaniu komunikatu o zakończeniu aktualizacji, usuń folder `/install` i przejdź do widoku zarówno Twojego sklepu, jak i jego panelu administracyjnego, żeby upewnić się, ze wszystko funkcjonuje poprawnie.
4. Zapewnienie jakości i testy:
   * Zaimportuj do nowego sklepu tłumaczenia wyeksportowane ze starego sklepu (możesz tego dokonać używając funkcji "Ręczne importowanie pakietu językowego" dostępnego na stronie "Lokalizacja / Tłumaczenia").
   * Sprawdź, czy szablon zachowuje się zgodnie z oczekiwaniami. Jeśli nie, trzeba będzie zmieniać pliki szablonu.
   * Dokładnie przetestuj funkcjonowanie sklepu: utwórz konta, kup produkty, anuluj zamówienia, sprawdź faktury itd.
5. Rozpocznij aktualizację na zdalnym serwerze WWW:
   * Używając klienta FTP zastąp pliki Twojego sklepu plikami skopiowanymi z folderu  "prestashop-prep".
   * Uruchom skrypt aktualizacji na Twoim zdalnym serwerze za pośrednictwem przeglądarki internetowej. W PrestaShop w wersji 1.6 skrypt ten umieszczony jest na końcu ścieżki `/install/upgrade/upgrade.php`.
   * Sprawdź parametry aktualizacji przed jej rozpoczęciem: podążaj za wskazówkami wyświetlanymi na ekranie i upewnij się, ze serwer spełnia wymagania techniczne stawiane przez nową wersję.&#x20;
   * Zakończ aktualizację: po otrzymaniu komunikatu o zakończeniu aktualizacji, usuń folder `/install` i przejdź do widoku zarówno Twojego sklepu, jak i jego panelu administracyjnego, żeby upewnić się, ze wszystko funkcjonuje poprawnie.
   * Zaimportuj do nowego sklepu tłumaczenia wyeksportowane ze starego sklepu (możesz tego dokonać używając funkcji "Ręczne importowanie pakietu językowego" dostępnego na stronie "Lokalizacja / Tłumaczenia").
   * Sprawdź, czy nazwa domeny głównej jest poprawna (sekcja "Ustaw URL sklepu" na stronie "Preferencje / SEO\&URL").
   * Odtwórz pliki robots.txt  (sekcja "Generowanie pliku robots" na stronie "Preferencje / SEO\&URL").
   * Sprawdź, czy szablon w dalszym ciągu zachowuje się zgodnie z oczekiwaniami. Jeśli nie, trzeba będzie zmieniać pliki szablonu.
   * Dokładnie przetestuj funkcjonowanie sklepu: utwórz konta, kup produkty, anuluj zamówienia, sprawdź faktury itd.
6. Włączenie zaktualizowanego sklepu
   * Włącz Twój sklep (Strona "Przerwa techniczna" dostępna pod pozycją "Preferencje" menu głównego)

Udało się! Ciesz się nowymi funkcjonalnościami zaktualizowanej wersji Twojego sklepu!&#x20;

### Krok 1 - Utwórz kopię bezpieczeństwa Twojego sklepu i zapisz ją  <a href="#recznaaktualizacja-krok1-utworzkopiebezpieczenstwatwojegosklepuizapiszja" id="recznaaktualizacja-krok1-utworzkopiebezpieczenstwatwojegosklepuizapiszja"></a>

Uwaga

Poniechanie utworzenia kopii bezpieczeństwa Twojego sklepu naraża Cię na ryzyko utraty wszystkich danych bez możliwości ich odzyskania w przypadku wystąpienia problemów podczas aktualizacji.

**Nigdy nie pomijaj tego kroku**. Nie przechodź do kroku 2 dopóki nie masz absolutnej pewności, że kopia bezpieczeństwa jest kompletna i w pełni funkcjonalna. Sprawdź kilka razy, czy na pewno tak jest.

#### Wyłączenie Twojego sklepu - włączenie przerwy technicznej <a href="#recznaaktualizacja-wylaczenietwojegosklepu-wlaczenieprzerwytechnicznej" id="recznaaktualizacja-wylaczenietwojegosklepu-wlaczenieprzerwytechnicznej"></a>

Uwaga

Wyłączenie Twojego sklepu na czas aktualizacji jest **bardzo ważne**.\
&#x20;Daje ono pewność, że w czasie aktualizacji wszelka aktywność w sklepie będzie niemożliwa, a zwłaszcza składanie zamówień przez klientów. Nawet  jeśli aktualizacja się nie powiedzie i trzeba będzie wrócić do wersji sklepu sprzed aktualizacji, nie utracisz żadnych zamówień i żaden z twoich klientów nie będzie rozczarowany.

Przejdź do panelu administracyjnego i na stronie "Przerwa techniczna" dostępnej pod pozycją "Preferencje" w menu głównym, obok frazy "Włącz sklep" zaznacz opcję "Nie"

Jeśli aktualizujesz PrestaShop w wersji 1.4, opcja ta jest dostępna jako pierwsza na liście po wybraniu pozycji "Ustawienia" w menu głównym.

W polu "Adres IP do zarządzania" (w wersji 1.4 "Adres IP do otwartego dostępu") dostępnym zaraz poniżej opcji "Włącz sklep", należy wpisać adresy IP, które nie zostaną objęte trybem "Przerwa techniczna". Dzięki temu będzie można oglądać sklep od frontu w czasie, kiedy będzie on wyłączony. Obok pola "Adres IP do zarządzania" znajduje się przycisk "Dodaj mój IP". Po jego wciśnięciu, adres komputera, z którego korzystamy zostanie dodany do wyjątków "Przerwy technicznej". Jeśli z jakichś przyczyn nie chcemy korzystać z tego przycisku, adres IP urządzenia, z którego aktualnie korzystamy możemy uzyskać na stronie: [http://whatismyipaddress.com/](http://whatismyipaddress.com/)

#### Tworzenie kopii bezpieczeństwa plików  <a href="#recznaaktualizacja-tworzeniekopiibezpieczenstwaplikow" id="recznaaktualizacja-tworzeniekopiibezpieczenstwaplikow"></a>

Powinieneś wykonać kopię bezpieczeństwa wszystkich plików składających sie na Twój sklep PrestaShop i zapisać ją na dysku Twojego komputera.

Istnieją dwa najczęściej stosowane sposoby tworzenia kopii bezpieczeństwa:

* **Poproś Twojego dostawcę usługi hostingu o skopiowanie Twoich plików**.\
  Upewnij się, że kopia, którą otrzymałeś jest funkcjonalna (umożliwia bezproblemowe odtworzenie sklepu) i w pełni odzwierciedla aktualny stan twojego sklepu (zawiera aktualny stan produktów, kategorii, zamówień itd).

...lub...

* **Używając klienta FTP skopiuj wszystkie pliki sklepu z Twojego serwera na Twój komputer**.\
  Możesz użyć tego sposobu tylko wtedy, kiedy Twój dostawca hostingu zapewnia Ci dostęp do serwera za pośrednictwem protokołu FTP. Na pulpicie Twojego komputera utwórz folder "prestashop-prod", po czym używając klienta FTP (takiego jak FileZilla, którego możesz pobrać ze strony [http://filezilla-project.org/](http://filezilla-project.org/)), zaznacz wszystkie zamieszczone na serwerze pliki i foldery składające się na Twój sklep (użyj skrótu klawiszowego Ctrl + A) i skopiuj je do folderu "prestashop-prod" na pulpicie Twojego komputera.

#### Tworzenie kopii bezpieczeństwa bazy danych <a href="#recznaaktualizacja-tworzeniekopiibezpieczenstwabazydanych" id="recznaaktualizacja-tworzeniekopiibezpieczenstwabazydanych"></a>

Koniecznie powinieneś wykonać kopię bezpieczeństwa bazy danych Twojego sklepu.

Istnieją trzy sposoby wykonania tej czynności:

* **Poproś Twojego dostawcę usługi hostingu o skopiowanie bazy danych Twojego sklepu**.\
  Upewnij się, że kopia, którą otrzymałeś jest w pełni funkcjonalna, świeża i kompletna.

...lub...

*   **Pobierz kopię bazy danych w panelu administracyjnym sklepu.** \
    Przejdź do strony "Backup bazy danych" i dalej postępuj według wskazówek umieszczonych na tej stronie.

    Ta strona dostępna jest w zależności od wersji PrestaShop:

    * PrestaShop 1.4: zakładka "Kopie zapasowe" dostępna pod pozycją "Narzędzia" menu głównego.
    * PrestaShop 1.5 i nowszy: zakładka "Backup bazy danych" dostępna pod pozycją "Zaawansowane" menu głównego.

    Proces pobierania kopii może potrwać od 1 do 20 minut w zależności od jej rozmiaru. Kiedy na stronie tworzenia kopii pojawi się link do pobrania kopii bazy zatytułowany "Pobierz plik kopii zapasowej", naciśnij go i pobierz plik. Upewnij się, że kopia, którą pobrałeś jest w pełni funkcjonalna i przede wszystkim kompletna. Rozpakuj plik zip i zanim przejdziesz do następnego kroku upewnij się, że wyekstrahowany plik o rozszerzeniu .sql nie zawiera ŻADNYCH BŁĘDÓW.&#x20;

...lub...

* **Pobierz kopię bazy danych korzystając z** phpMyAdmin.\
  Upewnij się, że kopia, którą pobrałeś jest w pełni funkcjonalna, świeża i przede wszystkim kompletna, Jeśli baza danych Twojego sklepu jest zbyt duża, proces utworzenia jej kopii może zakończyć się niepowodzeniem. W takim przypadku skontaktuj się z Twoim dostawcą hostingu.

Zapisz kopie bazy danych w folderze "prestashop-prod" na pulpicie Twojego komputera znanym Ci już z poprzednich czynności w ramach niniejszej instrukcji - tym samym, w którym przechowujesz kopie plików Twojego sklepu.

#### Tworzenie kopii bezpieczeństwa Twoich unikalnych tłumaczeń <a href="#recznaaktualizacja-tworzeniekopiibezpieczenstwatwoichunikalnychtlumaczen" id="recznaaktualizacja-tworzeniekopiibezpieczenstwatwoichunikalnychtlumaczen"></a>

Jeśli nie edytowałeś domyślnych tłumaczeń, ani nie dodawałeś nowych (odnosi się to do wszystkich tłumaczeń - również tych wykorzystywanych przez moduły), przejdź do kroku 2.

Aby zachować Twoje tłumaczenia:&#x20;

1.  Przejdź do strony "Tłumaczenia" w panelu administracyjnym.

    Strona ta jest dostępna w zależności od wersji PrestaShop:

    * PrestaShop 1.4: jako podstrona pozycji "Narzędzia" menu głównego.
    * PrestaShop 1.5 i nowszy: jako podstrona pozycji "Lokalizacja" menu głównego.
2. W sekcji "Export języka" wyvierz język, w którym dokonałeś modyfikacji, następnie wybierz nazwę Twojego aktualnego szablonu i wciśnij przycisk "Eksportuj".
3. Zapisz pobrany plik w folderze "prestashop-prod" na pulpicie Twojego komputera.&#x20;

Całą procedurę powtórz dla każdego języka, który został przez Ciebie dodany, zmodyfikowany, albo poprawiony.&#x20;

Sprawdź zawartość folderu zawierającego Twoje kopie bezpieczeństwa

Czy folder "prestashop-prod" zawiera...

* ...kompletną i aktualną kopię wszystkich plików Twojego aktualnego sklepu?
* ...kompletną i wolną od błędów kopię bazy danych?
* ...kopię Twoich unikalnych tłumaczeń (opcjonalnie)?

Po sprawdzeniu zawartości folderu "prestashop-prod" i upewnieniu się, że wszystkie kopie bezpieczeństwa są poprawne, i że umożliwiają odtworzenie Twojego sklepu w razie, gdyby aktualizacja zakończyła się niepowodzeniem, przejdź do kroku 2.

### Krok 2 - Przygotuj się na nową wersję <a href="#recznaaktualizacja-krok2-przygotujsienanowawersje" id="recznaaktualizacja-krok2-przygotujsienanowawersje"></a>

#### Pobieranie i rozpakowywanie najnowszej wersji PrestaShop <a href="#recznaaktualizacja-pobieranieirozpakowywanienajnowszejwersjiprestashop" id="recznaaktualizacja-pobieranieirozpakowywanienajnowszejwersjiprestashop"></a>

Odwiedź stronę [https://www.prestashop.com/pl/pobranie](https://www.prestashop.com/pl/pobranie) i pobierz najnowszą wersję PrestaShop (podaj swój adres e-mail, odpowiedz na pytanie formularza, wybierz język Twojego sklepu i wciśnij przycisk "Pobierz teraz").

Powinieneś pobrać plik zip o nazwie: `prestashop_1.6.x.zip` (gdzie "x" jest cyfrą określającą numer wersji).

Na pulpicie Twojego komputera utwórz folder o nazwie "prestashop-prep". Następnie rozpakuj dopiero co pobrany plik zip i umieść jego zawartość w folderze "prestashop-prep". W tym folderze przygotujesz pliki, za pomocą których dokonasz aktualizacji.Uwaga: przenieś pliki tak, aby folder `/prestashop` z archiwum .zip nie znajdował się w folderze "prestashop-prep". Raczej przenieś pliki i foldery, które zawiera, tak aby mieć te same pliki dla folderów "prestashop-prod" oraz "prestashop-prep".\
\


Jeśli jeszcze nie posiadasz narzędzia do rozpakowywania archiwów .zip, możesz pobrać jeden z nich za darmo tutaj: [http://www.7-zip.org/](http://www.7-zip.org/).

W folderze "`/prestashop-prep`" zaznacz folder  "`/admin`" i nadaj mu tę samą nazwę, którą nosi ten sam folder w wersji produkcyjnej sklepu. Na przykład, jeśli Twój "prestashop-prod"  używa nazwy `admin123,` nadaj tę samą nazwę folderowi `/admin` w folderze "prestashop-prep".

#### Kopiowanie plików zapasowych z "prestashop-prod" do nowego katalogu "prestashop-prep"  <a href="#recznaaktualizacja-kopiowanieplikowzapasowychz-prestashop-prod-donowegokatalogu-prestashop-prep" id="recznaaktualizacja-kopiowanieplikowzapasowychz-prestashop-prod-donowegokatalogu-prestashop-prep"></a>

Przyszedł czas, aby skopiować pliki, które są unikalne dla Twojego sklepu produkcyjnego, do katalogów nowej wersji. W praktyce, pomysł polega na zbudowaniu folderu "prestashop-prep", który zawierać będzie najnowszą wersję standardowych plików PrestaShopa oraz wszystkich plików, które stworzyłeś i umieściłeś online odkąd PrestaShop został zainstalowany: obrazki, loga, zdjęcia, tłumaczenia, moduły itp.To ważny krok, ponieważ pozwala Ci na zachowaniu wszystkich zmian z twojego sklepu.Nie spiesz się z wykonywaniem niniejszych poleceń.Od tej pory będziesz przeglądać pliki i foldery, ktore były przechowywane w folderze "prestashop-prod", w tym samym porządku w folderze "prestashop-prep".Za każdym razem, gdy system zapyta Cię czy zastąpić pliki, odpowiedz "tak".

Następujące foldery muszą zostać skopiowane z katalogu "prestashop-prod" do niedawno rozpakowanego folderu "prestashop-prep":

* **`/mails`**. Zawiera szablony maili, także te, które zmodyfikowałeś.\
  Jeśłi nigdy nie dokonałeś żadnej modyfikacji szablonu maila, nie przejmuj się tym folderem.
* **`/img`**. Zawiera logo i  wszystkie obrazki sklepu (kategorie, produkty itp.). Zadbaj w szczególności o poniższe pliki i foldery:
  * `logo.jpg` - logo sklepu
  * `favicon.ico` - favicon sklepu
  * `logo_stores.gif` - Logo sklepu na mapie
  * `/c` - obrazy kategorii
  * `/cms` - obrazki stron CMS
  * `/co` - kolory atrybutów
  * `/m` - logo producentów&#x20;
  * `/p` - zdjęcia produktów
  * `/scenes` - zdjęcia mapy kategorii
  * `/st` - zdjęcia sklepów fizycznych&#x20;
  * `/su` - logo Twoich dostawców
  * ...po prostu skopiuj wszystkie katalogi oprócz  `/img/admin` oraz `/img/jquery-ui`.
* **`/modules`**. Skopiuj tylko te moduły, które zainstalowałeś odkąd zainstalowałeś PrestaShopa po praz pierwszy (a które nie były częścią domyślnej instalacji).
  * Niektóre z tych modułów mogą nie być aktualnie włączone, albo nawet zainstalowane: to do Ciebie należy, czy są one nadal użyteczne dla Ciebie i zasługują na skopiowanie ich do zaktualizowanej wersji.
  * Ponadto zwróć uwagę, że prawdopodobnie, będziesz musiał zaktualizować moduły, które nie zostały stworzone z myślą o nowej wersji PrestaShopa.
* **`/themes/themeName`**. Skopiuj Twój aktualny szablon.
  * Jeśli korzystasz z domyślnego (niezmienionego) szablonu PrestaShopa, nie kopiuj jego katalogu (`/themes/prestashop`) : musisz skorzystać z tego w nowej wersji (`/themes/default`).
  * Jeśli dokonałeś zmian w domyślnym szablonie, skopiuj jego katalog.
* **`/download`** oraz **`/upload`**. Zawierają wszystkie pliki możliwe do pobrania przy produkcie, jego załączniki itp. Jeśli nie korzystasz z tych funkcjonalności, nie kopiuj tych katalogów.
*   **`/classes`**. Jeśli dodałeś, zmieniłeś klasy, skopiuj je do nowego katalogu `/classes`.

    Podczas aktualizacji z wersji poniżej 1.4, musisz ręcznie edytować klasy, które zmieniłeś. **Nie musisz zmieniać klas, w których nie dokonano zmian.** Aby wszystko działało prawidłowo w najnowszej wersji PrestaShopa, wszystkie te pliki klas muszą zawierać końcówkę "Core". _Nie rób tego, jeśli nie jesteś zaznajomiony z PHP._

    Oto jak powinieneś zmienić pliki klas, które chcesz zatrzymać:

    1. Skopiuj pliki klas, w których dokonałeś zmian do katalogu `/classes` w "prestashop-prep".
    2. Otwórz każdy plik klasy i znajdź te, które nie posiadają końcówki `Core`. Jeśli aktualizujesz z wersji 1.4.x, nie powinieneś mieć żadnej, (oprócz spersonalizowanych klas).
    3. Zmień nazwę klasy, dodając końcówkę "Core", na przykład: "MyClass" stanie się "MyClassCore".\
       Zmień nazwę tylko w klasie PHP, nie nazwę samego pliku!
    4. Jeśli wszystkie pliki mają już końcówkę "Core" w ich nazwie klasy (jak "`class AttributeCore extends ObjectModel`"), to nie musisz już zmieniać niczego.
    5. Zachowaj wszystkie edytowane pliki.
* **`/config`**. Musisz skopiować tylko jeden plik, ale najważniejszy:  `settings.inc.php` .
* `/translations` - jeśli korzystasz z innego języka, niż te dostępne w domyślnej instalacji , musisz skopiować katalog języka do kataogu  w nowej instalacji. Jeśli Ci się to nie uda, to aktualizacja nie będzie działać prawidłowo.

Twój katalog "prestashop-prep" jest gotowy. Nie dotykaj go więcej, od tej pory będziemy pracować tylko na jego kopii.

#### Przenoszenie katalogu "prestashop-prep" na Twój lokalny serwer <a href="#recznaaktualizacja-przenoszeniekatalogu-prestashop-prep-natwojlokalnyserwer" id="recznaaktualizacja-przenoszeniekatalogu-prestashop-prep-natwojlokalnyserwer"></a>

Katalog "prestashop-prep", który pierwotnie rozpakowałeś z archiwum najnowszej wersji PrestaShopa, zawiera obecnie wszystkie Twoje modyfikacje z katalogu "prestashop-prod"(czyli cały Twój sklep, który jest online, ale działa w trybie konserwacji) W tym kolejnym kroku, skopiujesz ten katalog na swój serwer lokalny, aby sprawdzić czy aktualizacja funkcjonuje bez żadnych problemów.

Uruchom serwer lokalny(WAMP, XAMPP, EasyPHP, MAMP albo jakikolwiek inny), i upewnij się, że Apache i MySQL działają.

Podstawowym założeniem jest sprawdzenie lokalnie, czy sklep może zostać zaktualizowany bez problemów na serwerze lokalnym, aby zminimalizować ryzyko błędów podczas uruchomiania aktualizacji Twojego sklepu. Dlatego powinieneś odtworzyć środowisko serwera, na którym znajduje się sklep, na serwerze lokalnym, aby zminimalizować ryzyko nieprzyjemnych niespodzianek podczas aktualizacji online.

Skontaktuj się z administracją hostingu, aby uzyskać informacje o konfiguracjach Apache, PHP i MySQL na Twoim serwerze, oraz edytuj odpowiednio pliki  `httpd.conf` (Apache), `php.ini` (PHP) oraz `my.ini` (MySQL), jeśli możesz. W przypadku ekstremalnym będziesz musiał zmienić wersję każdego z komponentów lokalnego serwera, aby zduplikować swój serwer online.

Gdy to zrobisz, zresetuj serwer lokalny, aby zmiany zostały wprowadzone.

Jeśli nie możesz edytować plików konfiguracji na lokalnym serwerze, to pamiętaj, że różnice pomiędzy serwerem online, a lokalnym mogą mieć ogromny wpływ na aktualizację, ponieważ to co funkcjonuje poprawnie w jednym środowisku nie musi działać poprawnie w innym. Jak na przykład limity pamięci i ścieżki absolutne zamiast relatywne.

Otwórz katalog webowy na twoim serwerze lokalnym (`/htdocs`, `/www`, `/web` albo inna nazwa w zależności od serwera),  i skopiuj katalog "prestashop-prep" do niego.

Caution

Nie przenoś po prostu swojego katalogu "prestashop-prep" do katalogu webowego serwera lokalnego!

Upewnij się że zrobiłeś jego kopię, aby pozostawić oryginał nietkniętym.

W ten sposób, w przypadku problemu z aktualizacją lokalną, będziesz w stanie otworzyć katalog "prestashop-prep" i dokonać niezbędnych zmian, zanim skopiujesz go na serwer lokalny i i spróbujesz zaktualizować sklep ponownie.

Umieść katalog "prestashop-prep" w katalogu webowym na lokalnym serwerze.

#### Odtwarzanie lokalnie produkcyjnej bazy danych <a href="#recznaaktualizacja-odtwarzanielokalnieprodukcyjnejbazydanych" id="recznaaktualizacja-odtwarzanielokalnieprodukcyjnejbazydanych"></a>

Lokalne pliki powinny być teraz aktualne, ale baza danych wymaga aktualizacji. Do tego służy skrypt aktualizacji. Stanowi on część plików zktualizacji wersji 1.6 PrestaShopa.

Musisz posiadać znajomość phpMyAdmin zanim wykonasz kolejne kroki z tej części.

Wykorzystamy teraz plik `.sql`, który utworzyłeś jako kopię bezpieczeństwa wcześniej. Za pomocą tego pliku, odtworzysz bazę danych na lokalnym serwerze. Aby to zrobić postępuj w następujący sposób:

1. Otwórz narzędzie phpMyAdmin, które powinno być dostępne na Twoim lokalnym serwerze. Zazwyczaj znajduje się ono pod adresem [http://127.0.0.1/phpmyadmin](http://127.0.0.1/phpmyadmin), albo [http://127.0.0.1/mysql](http://127.0.0.1/mysql).
2. Jeśli to nie ten przypadek, utwórz nową bazę danych dla tego projektu. Nadaj jej charakterystyczną nazwę, jak "prestashop\_update" albo nazwę bazy produkcyjnej.\
   Jeśli utworzyłeś już bazę danych dla poprzednich testów aktualizacji to usuń po prostu ich tabele.
3. Zaimportuj bazę danych z pliku do nowej bazy danych
4.  Naciśnij przeglądaj i wskaż plik .sql Twojego sklepu, który powinien się znajdować w katalogu "presashop-prod".\
    Sprawdź czy wartość "Max." wyświetlana w panelu jest większa od rozmiaru pliku `.sql.` jeśli nie to musisz edytować plik `php.ini`, a dokładnie wartość `upload_max_filesize`, the `post_max_size` albo nawet `memory_limit` w ostateczności. Gdy to zrobisz zrestartuj lokalny serwer, aby zmiany zostały zastosowane..

    Zamiast zmian ustawień serwera możesz także spróbować skompresować plik `.sql` za pomocą narzędzia Zip jak [http://www.7-zip.org/](http://www.7-zip.org/). phpMyAdmin powinien akceptować pliki typu `.sql.zip` i zajmie się samodzielnie rozpakowaniem ich.
5. Naciśnij przycisk "Go" i zaimportuj zawartość pliku SQL.

Poczekaj aż phpMyAdmin załaduje plik i doda tabele do bazy danych. Gdy skończy, zobaczysz tabele, które pojawią się po lewej stronie.

Wszystko co pozostało, to połączyć pliki PHP PrestaShopa z danymi serwera lokalnego. Aby to zrobić, musisz edytować informacje dotyczące bazy danych, aby wskazać lokalną bazę danych.

Otwórz plik `/config/settings.inc.php` i edytuj następujące linie:

* `_DB_SERVER_`: zastąp adres serwera MySQL sklepu, na lokalny serwer. Powinno to być "localhost", albo "127.0.0.1".
* `_DB_NAME_`: zamień nazwę bazy danych, na tę gdzie importowałeś tabele bazy produkcyjnej.
* `_DB_USER_`: zamień nazwę użytkownika z produkcyjnej na lokalną. Prawdopodobnie to powinno być "root".
* `_DB_PASSWD_`: zamień hasło użytkownika z bazy produkcyjnej na lokalną. Prawdopodobnie powinno to być puste pole "" .

PrestaShop może teraz uzyskać dostęp do Twojej bazy dancyh produkcyjnej na serwerze lokalnym, wszystko co teraz musisz zrobić to uruchomić skrypt aktualizacji.

#### Sprawdzanie wszystkiego zanim przejdziesz dalej <a href="#recznaaktualizacja-sprawdzaniewszystkiegozanimprzejdzieszdalej" id="recznaaktualizacja-sprawdzaniewszystkiegozanimprzejdzieszdalej"></a>

Czy postępowałeś według poniższych kroków?

1. Pobrałeś najnowszą wersję PrestaShopa.
2. Rozpakowałeś tę wersję i zachowałeś jej pliki w nowym katalogu "prestashop-prod".
3. Skopiowałeś pliki niestandardowe z lokalnej kopii zapasowej ("prestashop-prod") do  "prestashop-prep" folder.
4. Skopiowałeś  "prestashop-prep" folder w katalogu webowym na lokalnym serwerze..
5. Zaimportowałeś dane ze swojego sklepu produkcyjnego w lokalnym serwerze MySQL.
6. Umieściłeś poprawną informacje z baz danych w lokalnym pliku konfiguracyjnym.

Jeśli zrobiłeś je wszystkie, to możesz przejść do Kroku 3.

### Krok 3 – Rozpoczęcie Aktualizacji <a href="#recznaaktualizacja-krok3-rozpoczecieaktualizacji" id="recznaaktualizacja-krok3-rozpoczecieaktualizacji"></a>

#### Uruchamianie skryptu aktualizacji <a href="#recznaaktualizacja-uruchamianieskryptuaktualizacji" id="recznaaktualizacja-uruchamianieskryptuaktualizacji"></a>

Wejdź na stronę swojego sklepu, zmiana skryptu URL; na przykład: [http://127.0.0.1/prestashop-prep/install/upgrade/upgrade.php](http://127.0.0.1/prestashop-prep/install/upgrade/upgrade.php) (Zamień "prestashop-prep" z aktualnej nazwy folderu, który skopiowałeś na swój lokalny folder serwera).

Jeśli wraca problem 404, to możliwe, że nie skopiowałeś wszystkich plików z najnowszej wersji PrestaShop 1.6. Przejdź przez ten krok ponownie.

Jeśli adres pokazuje błąd 404, możliwe, że zapomniałeś o niektórych plikach z najnowszej wersji PrestaShop 1.6. Zrób ten etap ponownie: usuń folder który został skopiowany do folderu lokalnego, (ale uchyl plik `settings.inc.php`, dzięki czemu nie będziesz musiał zmieniać go ponownie), edytuj zawartość "prestashop-prep" folder zgodnie z tym co odkryłeś i skopiuj "prestashop-prep" ponownie do lokalnego serwera folderu webowego.

Gdy skrypt jest uruchamiany, **nie ruszaj swojej przeglądarki !** Nie zamykaj jej i nie klikaj przycisku "Wstecz": Skrypt Aktualizacja pracuje, to może zająć kilka minut. Niech wykona prace dla Ciebie!

W przeważającej części skrypt aktualizacji zajmuje się aktualizacją bazy danych SQL, która może się okazać sama w sobie bardzo żmudnym zadaniem. Obsługuje ona również aktualizacje `config/settings.inc.php`. Plik konfiguracyjny, w zależności od konfiguracji i środowiska, a także innych aspektów pracy wewnętrzej PrestaShop.

#### Zakończenie lokalnej aktualizacji <a href="#recznaaktualizacja-zakonczenielokalnejaktualizacji" id="recznaaktualizacja-zakonczenielokalnejaktualizacji"></a>

Po zakończeniu aktualizacji, plik XML powinen być wyświetlony w przeglądarce. Jest to normalne, ale może cię zaskoczyć, ponieważ nie wygląda jak zwykłe strony, a każda przeglądarka ma swój własny sposób wyświetlania go. Na przykład Firefox będzie najpierw wyświetlał komunikat ostrzegawczy."Ten plik XML nie zawiera żadnych informacji o stylach z nim związanych. Drzewo dokumentu zostanie przedstawione poniżej" nad treścią samego pliku XML. To ulegnie poprawie w kolejnych wersjach skryptu.

Należy zacząć od nastepującej lini:

```
<action result="ok" error="">
```

"Ok" udało się art: Działa! Najtrudniejsza część jest już za tobą, teraz ostatnie detale.

Na twoim lokalnym serwerze, w `/prestashop-prep` folder, powinieneś usunąć:

* &#x20;`/install` folder, który zawiera skrypt instalacyjny.
* &#x20;`README` pliki, które zawierają informacje na temat instalacji PrestaShop.
* `CHANGELOG` plik, który zawiera informacje na temat najnowszych zmian w PrestaShop.

Możesz teraz uzyskać dostęp do adresu lokalnego sklepu (w naszym przykładzie [http://127.0.0.1/prestashop-prep/](http://127.0.0.1/prestashop-prep/)), który powinien wyświetlić strone konserwacji ze swoim logo. Jest to normalne, ponieważ twój sklep powinien być w trybie konserwacji.

Jeśli motyw twojego sklep się nie wyświetla, ale zamiast tego pojawi się  biała strona z ostrzeżeniem "Twoa '_nazwa motywu_ ' temat nie jest dostepny. Sprawdź nazwę i uprawnienia folderu prywatnego", Prawdopodobnie zapomniałeś o etapie w którym miałeś skopiować swój motyw do `/prestashop-prep` folder.

Idź do swojego "prestashop-prod" folderu" `/themes` folder,  i kopiuj swój temat do folderu `/themes` w "pretashop-prep". Odśwież stronę, aby zobaczyć stronę Konserwacja - lub twój motyw.

Jeśli logo twojego sklepu się nie wyświetla, ale zamiast tego  widzisz "Twoje logo Tutaj" logo, musiałeś zapomnieć o kroku w którym powinieneś skopiować swoje niestandardowe obrazy z "prestashop-prod" folder ponad "prestashop-prep" folder.

Zapoznaj sie z Krokiem 2 niniejszego rozdziału ("Krok 2 - Przygotowanie do nowej wersji") aby skopiować odpowiednie pliki i foldery.

Teraz przejdź do strony administracyjnej swojego sklepu używając swojego spersonalizowanego `/admin` nazwy folderu. Musisz zalogować się używając zwykłych list uwierzytelniających. Przewertuj się przez różne strony adminstracyjne tam i z powrotem i sprawdź czy rzeczywiscie jest w nich zawartość i czy wszystkie strony panelu adminstracyjnego działają, nastepnie przejdź do sklepu z trybu konserwacji w celu wykrycia na witrynie sklepu drogi jaką przechodzi klient sklepu i upewnij się, że wszystko działa.

**Jeśli aktualizacja się nie powiodła**

Nie wszystkie aktualizacje działają sprawnie, z powodu różnych przyczyn. Dla pomocy skrypt aktualizacji wyświetla kod błędu na początku wyniku XML. W przypadku wystąpienia błędu, strona zaczyna się tak:

```
<action result="fail" error="27" />
```

Jak widzisz, atrybut "result" nie zawiera już "ok" ale "fail".

Oto niektóre z najczęstrzych błędów:

| Błąd kodu | Znaczenie                                      | Możliwe rozwiązanie                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| --------- | ---------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 5         | Nie można odczytać pliku konfiguracyjnego.     | Zmodyfikować prawa dostepu dla `/config/settings.inc.php` plików.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| 6         | Plik konfiguracyjny nie może być zapisany.     | Zmodyfikować prawa dostepu dla `/config/settings.inc.php` plików.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| 27        | Instalacja jest za stara.                      | Powinieneś użyć najnowszej wersji PrestaShop                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| 28        | Używasz już wersji docelowej.                  | <p>Wersja którą aktualizujesz jest taka sama którą już zainstalowałeś.<br>Jeśli były próby  zaktualizowania do najnowszej wersji PrestaShop, to nie jest to przeszkodą w aktualizacji jeśli nie pobierasz najnowszej wersji.<br><br>Ten błąd może być wywołany tym, że zaczynasz aktualizację odnowa, po tym jak już raz spróbowałeś. Jeśli tak jest należy sprawdzić, czy administracja działa i wskazuje najnowszy numer wersji. Jeśli, nie użyj starych kopii zapasowych (plików i baz danych), aby rozpocząć od nowa i wrócić do kroku 1 w procesie aktualizacji.</p> |
| 29        | Nie ma starszych wersji.                       | Czy skopiowałeś `config/settings.inc.php` plik taki jaki jest?                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| 31        | SQL aktualizacja nie może być znaleziona.      | Sprawdź `/install/upgrade/sql` czy folder nie jest pusty.Jeśli jest, uzyskaj pliki aktualizacji SQL z archiwum najnowszej wersji.                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| 32        | Nie można zaktualizować.                       | Część z plików może brakować albo źle się skopiowały. Zrestartuj cały proces od początku.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| 33        | Błąd przy wczytywaniu plików aktualizacji SQL. | Sprawdź czy pliki rzeczywiście są w folderze`/install/upgrade/sql` i czy mogą być odczytane.                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| 34        | Błąd wewnętrzny  SQL.                          | Pliki aktualizacji SQL mogą być uszkodzone. Pobierz ponownie najnowszą wersje archiwum i użyj plików z `/install/upgrade/sql`.                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| 35        | Cache jest włączony.                           | Wyłącz pamięć podręczną w PrestaShop przed uruchomieniem skryptu aktualizacji: otwórz w `config/settings.inc.php` plik i sprawdź  `define('`_`PS_CACHE_ENABLED`_`', '0');` czy rzeczywiście jest ustawiony na 0.                                                                                                                                                                                                                                                                                                                                                          |

Gdy aktualizacja skryptu się niepowiodła, trudno jest sprawdzić czy było możliwe zrobienie choćby części aktualizacji. Przed ponowną próbą aktualizacji, należy przywrócić pliki i bazy danych do stanu kopii zapasowej:

* Usuń wszystkie pliki z lokalnego folderu sieciowego i zastąp je tymi z folderu "prestashop-prep", które są czyste, ponieważ były one nietknięte.
* Usuń wszystkie tabele z bazy danych i zastąp je tymi które były orginalnie zainstalowane.

### Krok 4 - QA i Testowanie <a href="#recznaaktualizacja-krok4-qaitestowanie" id="recznaaktualizacja-krok4-qaitestowanie"></a>

#### Importowanie Tłumaczeń <a href="#recznaaktualizacja-importowanietlumaczen" id="recznaaktualizacja-importowanietlumaczen"></a>

Jeśli nie wyeksportowałeś swoich własnych tłumaczeń podczas 1 kroku (Kopie zapasowe), importuj je ponownie do swojego nowego sklepu przechodząc przez "Lokalizacje" menu, następnie stronę "Tłumaczenia", następnie użyj sekcji "importowanie pakietu językowego manualnie".

#### Testy do zrobienia w lokalnym sklepie testowym <a href="#recznaaktualizacja-testydozrobieniawlokalnymsklepietestowym" id="recznaaktualizacja-testydozrobieniawlokalnymsklepietestowym"></a>

By mieć pewność, że wszytko działa prawidłowo w twojej aktualizacji sklepu lokalnego, należy wykonać kilka testów :

* Upewnij się, że wszystkie typy stron ładują się prawidłowo (strona tytułowa, kategorie, produkty, porównywarka, CMS, etc.)
* Stwórz konto klienta
* Złóż zamówienie (dodaj do koszyka i zatwierdź)
* Zweryfikuj czy płatność działa prawidłowo (karty kredytowe, PayPal, etc.)
* W Panelu administracyjnym, sprawdź czy zamówienie było prawidłowo złożone i odebrane
* Wyślij email ze strony kontaktowej albo kliknij "Zapomniałem hasła"
* Sprawdź uzyskaną fakturę
* Sprawdź wszystkie moduły które aktywowałeś

To nie jest kompletna lista, powinieneś przeprowadzić jak najwięcej testów.

Jeśli zauważysz, że nie wszystkie aspekty aktualizacji sklepu działają prawidłowo:

1. Edytuj treść folderu "pretashop-prep" w celu rozwiązania problemów (brakujące pliki, złe konfiguracje, etc.)
2. Ponownie uruchom proces dla lokalnej aktualizacji:
   1. Usuń test podfolderu w lokalnym folderze webowym,
   2. Usuń tabele MySQL do aktualizacji testowych,
   3. Skopiuj pliki  "prestashop-prep" do lokalnego katalogu stron internetowych,
   4. Przenieś kopię zapasową SQL z pliku "prestashop-prod" ido lokalnego serwera MySQL,
   5. Ponownie uruchom skrypt aktualizacji.

Jeśli każdy z testów zakończył się sukcesem, to gratulujemy! Przejdź do kroku 5.

### Krok 5 - Rozpoczęcie aktualizacji na twoim sklepie <a href="#recznaaktualizacja-krok5-rozpoczecieaktualizacjinatwoimsklepie" id="recznaaktualizacja-krok5-rozpoczecieaktualizacjinatwoimsklepie"></a>

Jeśli osiągnołeś ten etap, to znaczy, że udało się zaktualizować twójj sklep na lokalnym serwerze. Stąd masz gwarancje, że aktualizacja na twoim hostingu sieciowym będzie działała dobrze. Twój  folder "prestashop-prep" zawiera wszytkie potrzebne pliki, ponieważ zmieniłeś zawartość na podstawie wcześniej zauważonych problemów w trakcie testów w poprzednim kroku.

Nigdy nie ma 100% gwarancji, że obydwa środowiska (lokalny serwer i hosting) będą się różnić. Najprościej jest skonfigurować lokalny serwer, tak aby pasował do serwera produkcyjnego najlepiej jak to tylko możliwe.

Twój sklep był w trybie konserwacji od początku procesu, dzięki temu nie straciłeś zamówień, koszyków, ani nowych klientów podczas procesu aktualizacji. Jeśli jeszcze tego nie zrobiłeś, to włącz sklep na tryb konserwacji teraz i powtórz proces od początku - chyba, że nie obawiasz się utraty zmian wprowadzonych od początku.

Czym innym jest umieszczenie plików w internecie a czym innym umieszczenie na lokalnym serwerze, proces umieszczenia w internecie rózni się trochę od tego testowanego lokalnie.

1. Korzystając z klienta FTP, zastąp pliki w swoim sklepie tymi z folderu "prestashop-prep".\
   Nie bój się o nic, ponieważ twoje wszystkie pliki zostały zabezpieczone z początkiem procesu w folderze "prestashop-prod" , więc możesz wrócić do swojej kopii zapasowej w każdej chwili. Ditto dla twojej bazy danych, które również zostało zachowane w folderze "prestashop-prod"  jako plik  `.sql`.
2. Uruchom skrypt aktualizacji na swoim sklepie produkcyjnym, otwierając go za pomocą przeglądarki. W wersji 1.6 na skrypcie z lokalizowanym w `/install/upgrade/upgrade.php`.
3. Sprawdź wszystkie ustawienia za nim zaktualizujesz: Postępuj zgodnie z instrukcją na ekranie i upewnij się, że serwer spełnia wymagania techniczne nowej wersji.
4. Zakończenie aktualizacji: Po zakończeniu aktualizacji usuń `/install`  i przejrzy swój sklep od strony zewnętrznej oraz od panelu administracyjnego upewniając się, że wszystko działa.

### Krok 6 - QA i Testowanie <a href="#recznaaktualizacja-krok6-qaitestowanie" id="recznaaktualizacja-krok6-qaitestowanie"></a>

Trzeba ponownie wykonać wszystkie czynności z przeprowadzonych na miejscu, aby upewnić się, że nic się nie zepsuło, pomimo zmiany z lokalnego środowiska na środowisko produkcyjne.

#### Importowanie tłumaczeń <a href="#recznaaktualizacja-importowanietlumaczen" id="recznaaktualizacja-importowanietlumaczen"></a>

Jeśli nie zaeksportowałeś swoich własnych tłumaczeń podczas kroku 1 (Kopie zapasowe), zaimportuj je z powrotem do nowego sklepu, przechodząc do menu "Lokalizacja", następnie strony "Tłumaczenia", a następnie skorzystaj z sekcji  "Importowanie pakietu językowego ręcznie".

#### Sprawdź główną nazwę domeny <a href="#recznaaktualizacja-sprawdzglownanazwedomeny" id="recznaaktualizacja-sprawdzglownanazwedomeny"></a>

Należy sprawdzić, czy nazwa domeny przypisana do bazy danych jest rzeczywiście tą na której pracujesz. Żeby to zrobić, przejdź do menu "Preferencje" następnie do strony "SEO & URLs".

Musisz sprawdzić następujące informacje z seksji "Ustawienia URL sklepu":

* "Domena sklepu": Powinna być to tą domena z którą jesteś aktualnie połączony. W przeciwnym razie, wszystkie linki będą nieprawidłowe i będą używały nieprawidłowej nazwy domeny.
* "Baza URI": Ten folder powinien być tym który wytransferowałeś do swojego serwera FTP; w tym poradniku byłby to  `/prestashop/`

Jeśli nie możesz dotrzeć do interfejsu administracyjnego, trzeba będzie przejść przez narzędzie do zarządzania bazami danych wykorzytywanych przez usługodawce hostingowego, takiego jak  phpMyAdmin:

1. Otwórz bazę danych w swoim sklepie produkcyjnym,
2. O`twórz ps_shop_url`,
3. Edytuj `domain`, `domain_ssl` i  `physical_uri` kolumny, tak aby pasowały do lokalizacji sklepu produkcyjnego.

Jak widać adres i ścieżka do twojego sklepu nie są już przechowywane  `/config/settings.inc.php` ale plik z wersji 1.6 jest w bazie danych.

Dlatego można otworzyć w `/config/settings.inc.php` i usunąć `define('_`_`PS_BASE_URI`_`_', '/le_chemin_de_la_boutique/');` jeśli aktualizacja nie zrobiła tego.

#### Badania do wykonania na zaktualizowanym sklepie <a href="#recznaaktualizacja-badaniadowykonanianazaktualizowanymsklepie" id="recznaaktualizacja-badaniadowykonanianazaktualizowanymsklepie"></a>

Upewnij się, że wszystko działa prawidłowo na zaktualizowanym sklepie. Przeprowadź kilka testów:

* Upewnij się, że wszystkie strony ładują się prawidłowo (strona domowa, kategorii, produktów, porównywarki, CMS, etc.)
* Stwórz konto klienta
* Złóż zamówienie (dodaj do koszyka i zamów)
* Zweryfikuj czy płatności działają prawidłowo (karty kredytowe, PayPal, etc.)
* W panelu administracyjnym sprawdź czy zamówienie jest dobrze zapisane i odebrane.
* Wyslij email ze strony kontakowej lub kliknij "Zapomniałem hasła"
* Sprawdź czy wystawiona faktura się zgadza
* Sprawdź wszystkie aktywowane moduły

Nie jest to kompletna lista, przeprowadź jak najwięcej testów.

Jeśli stwierdzisz, że nie wszystkie aspekty aktualizacji sklepu działają prawidowo:

1. Edytuj zawartość folderu "pretashop-prep"  w celu rozwiązania problemu (brak plików, nieprawidłowa konfiguracja etc.),
2. Ponownie uruchom proces dla lokalnej aktualizacji:
   1. Usuń test podfolderu w lokalnym folderze sieciowym,
   2. Usuń tabele MySQL dla aktualizacji testowej,
   3. Skopiuj pliki "prestashop-prep" do lokalnego folderu sieciowego,
   4. Zaimportuj kopie zapasową pliku SQL z "prestashop-prod" do lokalnego serwera MySQL,
   5. Ponownie uruchom skrypt aktualizacyjny.

Jeśli wszystkie testy zakończyły się sukcesem, gratulacje!

### Krok 7 - Aktywacja twojego sklepu <a href="#recznaaktualizacja-krok7-aktywacjatwojegosklepu" id="recznaaktualizacja-krok7-aktywacjatwojegosklepu"></a>

Wspaniale! Jesteś na końcu procesu aktualizacji!

Wszystko co pozostało do zrobienia to ponownie włączyć sklep. Przejdź do strony "Konserwacja" z menu "Preferencje", i wybierz "Tak" dla "Włączenie sklepu".

Przejdź do strony domowej twojego sklepu, i przeglądaj strony jak gdybyś był zwykłym odwiedzającym, w celu sprawdzenia po raz ostatni czy wszystko działa poprawnie.

Gratulujemy! Uaktualnienia do najnowszej i najlepszej wersji PrestaShop

Aktualizacja ręczna jest długim i szczegółowym procesem, który powinien być używany tylko z konieczności - na przykład, jeśli nie możesz przeprowadzić aktualizacji automatycznej.

Dlatego ręczna aktulizacja powinna być zarezerwowana tylko dla specjalistów, czyli dla tych co wiedzą jak korzystać z narzędzi programistycznych takich jak WAMP, phpMyAdmin, etc.Jeśli nie masz takich umiejętności, poproś o pomoc znajomego lub zapłać programiście. On spędzi nad tym dwie lub więcej godzin, żeby zrobić to dobrze.

Idea ręcznej aktualizacji jest prosta, zamiast ryzykować bezpośrednią aktualizację na swoim sklepie internetowym, mamy zamiar wykonać całą pracę na twoim komputerze przy użyciu lokalnego serwera PHP/MySQL takich jak WAMP lub XAMPP. Gdy lokalna aktualizacja powiedzie się, będzie trzeba zrobić to jeszcze raz tym razem online.

Za nim zaczniesz całą procedurę, twój sklep powinien być wyłączony (w "trybie" konserwacja") upewnij się, że twoi klienci nie stracą swojego koszyka zamówień podczas procesu aktualizacji. W efekcie onacza to, że twój sklep będzie zamknięty dla klientów przez cały proces (na jedną albo dwie godziny).
