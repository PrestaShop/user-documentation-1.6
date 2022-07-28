# Czego potrzebujesz, by zacząć?

**Spis treści**

/\*\<!\[CDATA\[\*/\
div.rbtoc1597140204104 {padding: 0px;}\
div.rbtoc1597140204104 ul {list-style: disc;margin-left: 0px;}\
div.rbtoc1597140204104 li {margin-left: 0px;padding-left: 0px;}\
\
/\*]]>\*/

* [Wszystko, czego potrzebujesz](czego-potrzebujesz-by-zaczac.md#Czegopotrzebujesz,byzacząć?-Wszystko,czegopotrzebujesz)
  * [Aby rozpocząć szybką konfigurację](czego-potrzebujesz-by-zaczac.md#Czegopotrzebujesz,byzacząć?-Abyrozpocząćszybkąkonfigurację)
  * [Szczegółowe instrukcje](czego-potrzebujesz-by-zaczac.md#Czegopotrzebujesz,byzacząć?-Szczegółoweinstrukcje)
    * [Rejestracja domeny](czego-potrzebujesz-by-zaczac.md#Czegopotrzebujesz,byzacząć?-Rejestracjadomeny)
    * [Znalezienie dostawcy usług hostingowych](czego-potrzebujesz-by-zaczac.md#Czegopotrzebujesz,byzacząć?-Znalezieniedostawcyusłughostingowych)
    * [Wymagania sprzętowe](czego-potrzebujesz-by-zaczac.md#Czegopotrzebujesz,byzacząć?-Wymaganiasprzętowe)
    * [Narzędzia](czego-potrzebujesz-by-zaczac.md#Czegopotrzebujesz,byzacząć?-Narzędzia)
      * [Edytor tekstu](czego-potrzebujesz-by-zaczac.md#Czegopotrzebujesz,byzacząć?-Edytortekstu)
      * [Klient FTP](czego-potrzebujesz-by-zaczac.md#Czegopotrzebujesz,byzacząć?-KlientFTP)
    * [Planowanie](czego-potrzebujesz-by-zaczac.md#Czegopotrzebujesz,byzacząć?-Planowanie)
    * [Instalacja PrestaShop](czego-potrzebujesz-by-zaczac.md#Czegopotrzebujesz,byzacząć?-InstalacjaPrestaShop)

## Wszystko, czego potrzebujesz <a href="#czegopotrzebujesz-byzaczac-wszystko-czegopotrzebujesz" id="czegopotrzebujesz-byzaczac-wszystko-czegopotrzebujesz"></a>

### Aby rozpocząć szybką konfigurację <a href="#czegopotrzebujesz-byzaczac-abyrozpoczacszybkakonfiguracje" id="czegopotrzebujesz-byzaczac-abyrozpoczacszybkakonfiguracje"></a>

Poniżej przedstawiamy listę wymaganych rzeczy w celu rozpoczęcia instalacji PrestaShop 1.6. Jeśli po przeczytaniu tej sekcji nie wszystko będzie jasne, nie przejmuj się, szczegóły znajdziesz w kolejnych rozdziałach.

* Wymagania sprzętowe:
  * PHP 5.2 lub nowszy.
    * Przydatne ustawienia: `allow_url_fopen` = On, `register_globals` = Off, `magic_quotes_*` = Off, `safe_mode` = Off (wszystko w pliku the`php.ini`), `file_max_upload_size` = "16M".
    * Przydatne rozszerzenia PHP: PDO\_MySQL, cURL, SimpleXML, mcrypt, GD, OpenSSL, DOM, SOAP (wszystko w pliku `php.ini`).
    * Przydatne narzędzia serwerowe: cron/crontab, Memcached.
  * MySQL 5.0 lub nowszy.
  * Będzie lepiej, jeśli: \

    * Zdecydujesz się na hosting w oparciu o Unix/Linux.
    * Wybierzesz Apache Web Server 1.3 (lub nowszy), równie dobrym wyborem będzie nginx Web Server.
      * Ustawienia modułu Apache: `mod_rewrite` enabled, `mod_security` disabled, `mod_auth_basic` disabled.
    * Będziesz dysponował przynajmniej 64 Mb pamięci RAM dla PHP.
* Dane dostępowe do serwera FTP oraz bazy danych MySQL\

  * Dane te powinny być dostarczone przez dostawcę usług hostingowych - chyba, że wykonujesz instalację lokalną.
* Edytor tekstowy.
* Klient FTP.
* Dowolna współczesna przeglądarka internetowa (jeśli używasz Internet Explorer: przynajmniej IE8).

Musisz także wybrać adres URL ( adres domeny) dla Twojego sklepu.

Sprawdź oficjalne wymagania sprzętowe: [http://www.prestashop.com/pl/system-requirements](http://www.prestashop.com/pl/system-requirements).

Jeśli wszystkie powyższe wymagania zostały spełnione, możesz przejść do instrukcji instalacji: [http://doc.prestashop.com/display/PS16/Installing+PrestaShop](http://doc.prestashop.com/display/PS16/Installing+PrestaShop).

### Szczegółowe instrukcje <a href="#czegopotrzebujesz-byzaczac-szczegoloweinstrukcje" id="czegopotrzebujesz-byzaczac-szczegoloweinstrukcje"></a>

PrestaShop jest "aplikacją webową": trzeba ją zainstalować na serwerze, konieczna jest także domena, której Twoi Klienci będą używać, by dotrzeć do sklepu.

#### Rejestracja domeny <a href="#czegopotrzebujesz-byzaczac-rejestracjadomeny" id="czegopotrzebujesz-byzaczac-rejestracjadomeny"></a>

Zanim pobierzesz wersję instalacyjną PrestaShop musisz przygotować miejsce na swój sklep. W tym celu konieczne jest posiadanie domeny i miejsca na serwerze. Domena w jednoznaczny sposób określa lokalizację Twojej strony internetowej (np.: moj\_sklep.com lub przyklad.pl), a tym samym i Twojego sklepu.

Musisz kupić domenę dla Twojego sklepu. Prawdopodobnie będziesz w stanie kupić domenę przy zakupie serwisu hostingowego: wielu dostawców usług hostingowych oferuje darmowe domeny, dostępne po założeniu konta w ich serwisie. Możliwe, że domena będzie darmowa przez rok lub tak długo jak będziesz korzystał z usług danego dostawcy. Takie rozwiązanie pozwala na szybki i wygodny zakup pakietu usług (hosting+domena).

Może się tak zdarzyć, że domeny proponowane przez dostawcę hostingu nie będą spełniały Twoich oczekiwań. Możliwe również, że po pewnym czasie sam serwis hostingowy przestanie być odpowiedni i zaistnieje potrzeba jego zmiany, wówczas konieczne będzie przeniesienie wszystkich plików i domeny do nowego dostawcy.

Pliki i dane są łatwe do przeniesienia. Możliwe jednak, że przeniesienie domeny będzie nieco trudniejsze. Spowodowane jest to faktem, że dostawca usług hostingowych zakupił domenę dla Ciebie. Techniczne rzecz ujmując, domena należy do Twojego dotychczasowego dostawcy usług hostingowych, który może uniemożliwić przeniesienie jej do nowego serwisu hostingowego lub oczekiwać wykupienia domeny. Ponieważ nazwa domeny jest Twoją marką i adresem w sieci, musisz podporządkować się regulaminowi Twojego dostawcy usług hostingowych.

Dlatego też warto rozważyć zakupienie domeny niezależne od firmy oferującej hosting Twojego sklepu (zerknij: [http://en.wikipedia.org/wiki/Domain\_name\_registrar](http://en.wikipedia.org/wiki/Domain\_name\_registrar)). Tak naprawdę zawsze kupujesz domenę na określony czas (wynajmujesz ją), w większości przypadków będziesz musiał opłacać domenę w każdym kolejnym roku. Taki abonament daje Ci możliwość posługiwania się domeną, jeśli jednak przestaniesz uiszczać opłaty, ktoś inny będzie mógł przejąć Twoją domenę. Jeśli zaś płacisz abonament regularnie, masz swobodę wyboru (zmiany) dostawcy usług hostingowych: wystarczy zmienić adres domeny w DNS i poczekać 24 godziny, aż zmiana zostanie wprowadzona.

Jeśli zdecydujesz się na samodzielny zakup domeny, podajemy klika serwisów, z których możesz skorzystać:

* Gandi: [http://en.gandi.net/](http://en.gandi.net/)
* Namecheap: [http://www.namecheap.com/](http://www.namecheap.com/)
* PairNIC: [https://www.pairnic.com/](https://www.pairnic.com/)

Jest ich o wiele więcej. Zapytaj znajomych!

#### Znalezienie dostawcy usług hostingowych <a href="#czegopotrzebujesz-byzaczac-znalezieniedostawcyuslughostingowych" id="czegopotrzebujesz-byzaczac-znalezieniedostawcyuslughostingowych"></a>

Skoro już masz domenę, musisz sprawić by prowadziła ona do Twojego sklepu PrestShop. To znaczy, że pliki PrestaShop muszą zostać umieszczone na serwerze. Możliwe, że masz własny serwer, jednak bardziej prawdopodobne, że powierzysz pliki dostawcy usług hostingowych (zerknij: [http://pl.wikipedia.org/wiki/Hosting](http://pl.wikipedia.org/wiki/Hosting)), który w zamian za określoną opłatę abonamentową zajmie się Twoimi plikami.

Zanim rozpoczniesz budowę sklepu będziesz musiał wybrać dostawcę usług hostingowych. Tak naprawdę wszyscy dostawcy będą w stanie dostarczyć zadowalającą usługę, jednak tylko kilku oferuje serwis zoptymalizowany pod PrestaShop:

* [InMotion hosting](http://www.inmotionhosting.com/pl/prestashop-promo)
* [1&1](http://www.prestashop.com/pl/ecommerce-hosting)
* [A2 hosting](https://www.a2hosting.com/prestashop-hosting-options)\
  \


Możesz porównać oferowane usługi, klikając [tutaj](http://www.prestashop.com/pl/ecommerce-hosting)

Podczas wyboru dostawcy pamiętaj o podstawowych wymaganiach: dostawca musi zapewniać wsparcie PHP 5.2 (lub nowszego), języka w którym napisano PrestaShop, a także MySQL 5 (lub nowszego) bazy danych, w której PrestaShop przechowuje dane. Wymagań jest więcej. Aby się z nimi zapoznać przejdź do sekcji "Wymagania sprzętowe" poniżej.

PrestaBox

Dajemy możliwość utrzymania Twojego sklepu na naszych serwerach: rozwiązanie PrestaBox zostało stworzone, by umożliwić przedsiębiorcom proste i szybkie uruchomienie sklepu, bez konieczności manualnej instalacji czy aktualizacji sklepu. Aby zapoznać się ze szczegółami tej propozycji, odwiedź naszą stronę dedykowaną temu przystępnemu i bezpiecznemu rozwiązaniu hostingowemu. Jest to propozycja, którą powinni rozważyć zwłaszcza przedsiębiorcy mniej doświadczeni w kwestiach informatycznych.

Opis PrestaBox znajduje się pod adresem: [http://www.prestabox.com/](http://www.prestabox.com/)

#### Wymagania sprzętowe <a href="#czegopotrzebujesz-byzaczac-wymaganiasprzetowe" id="czegopotrzebujesz-byzaczac-wymaganiasprzetowe"></a>

PrestaShop jest aplikacją działającą na serwerze, została ona napisana za pomocą języka PHP. Przechowuje dane w bazie MySQL.\
PHP jest językiem programowania stworzonym w modelu otwartego oprogramowania (en. _open-source_), wykorzystywanym przeważnie w aplikacjach sieciowych. PHP został stworzony w 1995 roku i jest obecnie jednym z najczęściej używanych języków programowania. Wykorzystuje on składnię podobną do języka C, co sprawia, że łatwo się go nauczyć.\
MySQL jest systemem zarządzania bazami danych również opartym o filozofię otwartego oprogramowania. Podobnie jak PHP, zaistniał w 1995 roku i jest jednym z najpopularniejszych systemów. MySQL działa wykorzystując język SQL (jeden z najpopularniejszych języków przyrzeczony do pracy z bazami danych).\
Jeśli chcesz dowiedzieć się więcej:

* Otwarte oprogramowanie: [http://pl.wikipedia.org/wiki/Otwarte\_oprogramowanie](http://pl.wikipedia.org/wiki/Otwarte\_oprogramowanie)
* PHP: [http://pl.wikipedia.org/wiki/PHP](http://pl.wikipedia.org/wiki/PHP)
* MySQL: [http://pl.wikipedia.org/wiki/MySQL](http://pl.wikipedia.org/wiki/MySQL)
* SQL: [http://pl.wikipedia.org/wiki/SQL](http://pl.wikipedia.org/wiki/SQL)

Niezależnie od tego, jaki serwis hostingowy wybierzesz, musi on mieć zainstalowane następujące składniki:

* **System**: Unix, Linux lub Windows. Zalecamy Unix.
* **Web server**: Apache Web server 1.3 (lub nowszy).
* **PHP 5.2 (lub nowszy)**. Możliwe, że PHP5 trzeba będzie specjalnie aktywować (zapytaj dostawcę usług hostingowych).
* **MySQL 5.0 (lub nowszy)**.
* Co najmniej 64 Mb pamięci RAM na serwerze (128 Mb będzie bardziej komfortowym rozwiązaniem, generalnie im więcej, tym lepiej).

PrestaShop może także współpracować z serwerem Microsoft IIS 6.0 (lub nowszym), nginx 1.0 (lub nowszym).

Więcej informacji ważnych dla administratorów systemów znajdziesz w ["Podręczniku administratora"](http://doc.prestashop.com/display/PS15/System+Administrator+Guide).

#### Narzędzia <a href="#czegopotrzebujesz-byzaczac-narzedzia" id="czegopotrzebujesz-byzaczac-narzedzia"></a>

Będziesz potrzebował dwóch narzędzi: edytora tekstu (aby edytować pliki tekstowe) oraz klienta FTP, który będzie potrzebny do przesyłania Twoich plików z komputera na serwer i vice-versa.&#x20;

**Edytor tekstu**

Poniżej znajdziesz klika powszechnie znanych edytorów tekstu:&#x20;

* Windows:
  * Notepad++: [http://notepad-plus-plus.org/](http://notepad-plus-plus.org/)
  * UltraEdit: [http://www.ultraedit.com/](http://www.ultraedit.com/)
  * Crimson Editor: [http://www.crimsoneditor.com/](http://www.crimsoneditor.com/)
* OS X:
  * Textmate: [http://macromates.com/](http://macromates.com/)
  * Coda: [http://www.panic.com/coda/](http://www.panic.com/coda/)
  * Smultron: [http://www.peterborgapps.com/smultron/](http://www.peterborgapps.com/smultron/)
* Unix/Linux:
  * Vim: [http://www.vim.org/](http://www.vim.org/)
  * Emacs: [http://www.gnu.org/software/emacs/](http://www.gnu.org/software/emacs/)

Nie używaj zaawansowanych edytorów tekstu, takich jak Microsoft Word czy [OpenOffice.org](http://openoffice.org) Write

**Klient FTP**

FTP to skrót do  "protokół transferu plików" (en. _File Transfer Protocol_). Oznacza sposób przesyłania plików do i ze zdalnych lokalizacji, takich jak serwer.

W tym podręczniku będziemy wykorzystywać darmowy program FileZilla obsługujący FTP. Wspomniany program jest dostępny na platformy Windows, Mac OS X oraz Linux. Oprogramowanie możesz pobrać pod adresem [http://filezilla-project.org/](http://filezilla-project.org/). Pobierz FileZilla Client, a nie FileZilla Server!

Gdy już zainstalujesz FIleZilla, konieczna będzie konfiguracja programu zgodnie z danymi dostarczonymi przez dostawcę usług hostingowych. Prawdopodobnie informacje te zostały dostarczone po wykupieniu usługi hostingowej (możliwe, że e-mail z tymi informacjami trafił do folderu SPAM). Jeśli nie posiadasz koniecznych danych, skontaktuj się z firmą hostingową.

Dane, o których mówimy to:

* **nazwa hosta** lub **adres IP** : lokalizacja Twojego konta w serwisie hostingowym.
* **nazwa użytkownika**: nazwa Twojego konta w serwisie hostingowym
* **hasło**

Włącz FileZilla i otwórz "Menadżera stron". Menadżera można otworzyć na klika sposobów:

* wciskając kombinację klawiszy Ctrl-S,
* klikając na ikonę w lewym górnym rogu okna programu  "Otwórz Menadżera Stron",
* otwierając "Plik" i wybierając "Menadżer stron..."

Otwiera się okno.

Aby dodać dane swojego konta hostingowego do Menadżera Stron, należy:

1. Kliknąć na przycisk "Nowy adres". Na liście powyżej przycisku zostaje utworzona nowa pozycja, nazwij ją w sposób kojarzący się z Twoim sklepem.&#x20;
2. W prawej części okna "Menadżera stron" wybierz zakładkę "Ogólne" i wprowadź dane dostarczone przez Twojego dostawcę hostingu: "Serwer" (nazwa hosta, IP),  "Użytkownik" (nazwa użytkownika) i  hasło.  Prawdopodobnie nic więcej nie trzeba będzie zmieniać, chyba że otrzymałeś inne informacje od dostawcy hostingu.
3. Po uzupełnieniu danych kliknij na przycisk "Połącz" - spowoduje to zapisanie parametrów i ustanowienie połączenia z serwerem

Jeśli program FileZilla Ci się nie podoba, podpowiadamy klika alternatyw:&#x20;

* Windows:
  * CoreFTP: [http://www.coreftp.com/](http://www.coreftp.com/)
  * WinSCP: [http://winscp.net/](http://winscp.net/)
  * SmartFTP: [http://www.smartftp.com/](http://www.smartftp.com/)
* Mac OS X:
  * Cyberduck: [http://cyberduck.ch/](http://cyberduck.ch/)
  * Transmit: [http://www.panic.com/transmit/](http://www.panic.com/transmit/)
  * Fetch: [http://fetchsoftworks.com/fetch/](http://fetchsoftworks.com/fetch/)
* Unix/Linux:
  * gFTP: [http://gftp.seul.org/](http://gftp.seul.org/)
  * kasablanca: [http://kasablanca.berlios.de/](http://kasablanca.berlios.de/)
  * NcFTP: [http://www.ncftp.com/ncftp/](http://www.ncftp.com/ncftp/)

#### Planowanie <a href="#czegopotrzebujesz-byzaczac-planowanie" id="czegopotrzebujesz-byzaczac-planowanie"></a>

Na samym początku musisz się zdecydować, gdzie będzie Twój sklep. Masz klika możliwości:

* W głównej domenie: [http://www.przyklad.com/](http://www.example.com/)
* W folderze: [http://www.przyklad.com/sklep/](http://www.example.com/shop/)
* W sub-domenie: [http://sklep.przyklad.com/](http://store.example.com/)
* W folderze w sub-domenie: [http://ubrania.przyklad.com/sklep/](http://clothes.example.com/boutique/)

Dzięki funkcji "multistore" dostępnej w PrestaShop 1.6 możesz stworzyć tyle sklepów, ile tylko chcesz, opierając się na pojedynczej instalacji PrestaShop. Każdy ze sklepów może mieć swoją domenę. Domyślnie sklep będzie umieszczony tam, gdzie znajduje się folder z PrestaShop.

#### Instalacja PrestaShop <a href="#czegopotrzebujesz-byzaczac-instalacjaprestashop" id="czegopotrzebujesz-byzaczac-instalacjaprestashop"></a>

Teraz, gdy spełniłeś wszystkie powyższe warunki, możesz przejść do rozdziału opisującego instalację PrestaShop: [Instalacja PrestaShop](http://doc.prestashop.com/display/PS16/Instalacja+PrestaShop)
