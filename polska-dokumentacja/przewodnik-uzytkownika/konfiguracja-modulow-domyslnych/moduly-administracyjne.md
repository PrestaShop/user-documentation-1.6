# Moduły Administracyjne

## 1-Click Upgrade - AutoUpgrade (Auto aktualizacja) <a href="#modulyadministracyjne-1-clickupgrade-autoupgrade-autoaktualizacja" id="modulyadministracyjne-1-clickupgrade-autoupgrade-autoaktualizacja"></a>

Ten moduł ułatwia aktualizację oprogramowania PrestaShop do jego najnowszej wersji\
&#x20;Czytaj również rozdział "Automatyczna aktualizacja" podręcznika PrestaShop, aby dowiedzieć się więcej o tym module:

[http://doc.prestashop.com/display/PS16/Automatic+update](http://doc.prestashop.com/display/PS16/Automatic+update).

## Zaawansowana zgodność z przepisami UE <a href="#modulyadministracyjne-zaawansowanazgodnosczprzepisamiue" id="modulyadministracyjne-zaawansowanazgodnosczprzepisamiue"></a>

_Nowość w PrestaShop 1.6.1.0._

Moduł Zaawansowana zgodność z przepisami EU pomaga dostosować sprzedawcą swoje sklepy do najnowszych bardziej restrykcyjnych przepisów EU.

Jest on niezbędny dla sklepów w Europie..

Większość jego opcji ma na celu zapewnienie większej przejrzystości końcowym klientom przy czym.:

* Bardziej szczegółowe etykiety cen ( Począwszy od podatku, kosztach wysyłki, opóźnieniach, wagi produktu itd.)
* Zaawansowana strona wypłaty
* Uzupełnianie treści prawnych dla wiadomości email.

Nie wszystkie z tych opcji będą użyteczne we wszystkich krajach, ale one wszystkie pomagają Twojemu sklepowi bardziej szanować przepisy handlu elektronicznego w EU.\
Domyślne ustawienia to zalecane ustawienia. Możesz włączyć lub wyłączyć ustawienia.

### Opcje etykiet <a href="#modulyadministracyjne-opcjeetykiet" id="modulyadministracyjne-opcjeetykiet"></a>

Upewnij się, że zostały przetłumaczone wszystkie pola we wszystkich dostępnych językach..

* **Szacunkowa etykieta dostawy (dostępne pordukty)**. Wskazuje szacunkowy czas dostawy dla produktów w magazynie. Pozostaw puste pole,a by wyłączyć tę opcje Domyślnym tekstem jest "Dostawa: od 1 do 3 tygodni".
* **Szacunkowa etykieta dostawy (produkty dostępne w magazynie)** . Wskazuje przybliżony czas dostawy dla produktów dostępnych na składzie. Pozostaw puste pole, aby je wyłączyć. Domyślnym tekstem jest: "Dostawa od 3 do 6 tygodni".
* **'Przed' Bazą cenową**. Gdy produkt jest dostępny w sprzedaży wyświetla cenę bazową z etykietą "Przed"..
* **Podatek 'właczony./wyłączony.'** Wyświetla czy podatek jest wliczony w cenę produktu (etykieta Podatek włączony/ wyłączony")
* **Etykieta opłata za wysyłkę "włączona/wyłączona"**. Wyświetla czy ceny wysyłki są wliczone w cenę, obok ceny produktu (Włączone/wyłączone ceny przesyłki)\
  Po włączeniu upewnij się, że opcja "Wysyłka i płatność" jest powiązana ze stroną CMS w sekcji "Zarządzanie prawami autorskimi"  na ekranie konfiguracji. Etykieta będzie zawierać link do tej zawartości.
* **Etykieta waga produktu.** Wyświetla wagę produktu (kiedy informacja jest dostępna i waga produktu wynosi więcej niż 1 kg).
* **Precyzja wagi produktu.** Pomaga wybrać precyzyjny poziom wyświetlana produktu (na przykład: 1kg/1.01 kg) wartość nie może być ujemna.
* **Warunki odwoławcze w ToS**. Obejmuje treść strony CMS "Warunki wycofania w ramach warunków świadczenia usług (ToS).\
  Po włączeniu upewnij się, że opcja :Warunki wycofania"  jest powiązana z witryną CMS w sekcji " Zarządzanie prawami autorskimi" dalej w dół na ekranie konfiguracji. Etykieta będzie zawierać link do tej zawartości.
* **Odwołanie do wirtualnych produktów.** Dodaje obowiązkowe pole do wyboru, gdy koszyk zawiera produkt wirtualny. Użyj go aby zapewnić klientom świadomość, że nie można zwrócić produktu wirtualnego.&#x20;
* **'Z' etykiety cenowej (w przypadku kombinacji)** . Wyświetla etykietę 'Z" przed ceną produktów zawierających kombinacje. Ponieważ ceny mogą różnić się w zależności od kombinacji, ta etykieta wskazuje, że cena końcowa może być wyższa.
* **Górny tekst koszyka zakupów.** Dodaje niestandardowy tekst nad podsumowaniem koszyka.
* **Dolny tekst koszyka zakupów.** Dodaje niestandardowy teks na dole podsumowania koszyka.&#x20;

### Opcje funkcji <a href="#modulyadministracyjne-opcjefunkcji" id="modulyadministracyjne-opcjefunkcji"></a>

* **Włącz funkcje "Powiedz przyjacielowi"** Jeśli ta funkcja jest włączona, moduł  "Wyślij do przyjaciela" pozwala klientom wysłać do znajomego wiadomość e-mail z linkiem do strony produktu. Ta opcja zapewnia zgodność z prawodawstwem lokalnym, przed włączeniem upewnij się, że jest ono z nim zgodne inaczej e-maile można uznać za niechciane wiadomości komercyjne.
* **Włącz cechę 'Zmiana kolejności'**. Jeśli ta opcja jest włączona, opcja "zmień kolejność" pozwala klientom na kolejną zmianę w kolejności od strony historii zamówień.  \
  Przed włączeniem upewnij się jest ona zgodna z twoim lokalnym prawem, inaczej można ją uznać za towar nie zamówiony.
* **Włącz "Zaawansowaną stronę kontroli"**. Zastąp standardowy proces kontroli bardziej zgodnym z prawem (EU oczywiście). Ta opcja działa tylko w szablonie domyślnym- bootstrap, lub innymi kompatybilnymi metodami płatności (wiele modułów jest przystosowanych)  Po włączeniu zaawansowana strona transakcji zawiera następujące sekcje: metody płatności, podsumowanie adresów, umowę typu ToS, podsumowanie koszyka i przycisk "Zlecenie z obowiązkiem zapłaty".
* **Proponowany podatek od wysyłki i opakowania**. Zamiast przypisywać grupę podatkową dla przewoźników i pakowania prezentów, średni podatek od produktu w koszyku jest wykorzystywany do obliczenia podatku od przewoźników i pakowania prezentów. Jest to bardzo przydatne w Niemczech.  .\
  Po ich włączeniu podatek od kosztów wysyłki i pakowania prezentów będzie obliczany proporcjonalnie do podatków mających zastosowanie do produktów w koszyku. W efekcie oznacza to, że klient otrzyma ostateczną cenę "z podatkiem" na początku procesu zakupowego, a podatki z wysyłką i pakowaniem prezentów będą obliczane przez cały proces zakupów i pobierany na marginesie.&#x20;

### Zarządzenie treścią prawną <a href="#modulyadministracyjne-zarzadzenietresciaprawna" id="modulyadministracyjne-zarzadzenietresciaprawna"></a>

Kilka opcji tego modułu. wymaga aby system "wiedział" do czego służą strony CMS. Jeśli nie ma żadnej strony dla niektórych powiązań, musisz je utworzyć.&#x20;

### Integracja zawartości poczty elektronicznej  <a href="#modulyadministracyjne-integracjazawartoscipocztyelektronicznej" id="modulyadministracyjne-integracjazawartoscipocztyelektronicznej"></a>

Za pomocą tego interfejsu można wybrać dokumenty które mają być umieszczone na dole, do standardowych wiadomości e-mail wysyłanych przez sklep - na przykład na stronie wszystkich faktur można umieścić tekstową treść "Warunki umowy sklepu".

Zawartość jest wybierana z ustawień sekcji "Zarządzanie prawami autorskimi" tego modułu. Jeśli nie ustawiono żadnej opcji, nie można wybrać zawartości do wysłania.

**Menedżer zadań Cron**

Ten moduł udostępnia narzędzie typu Cron, dzięki niemu będzie można tworzyć zadania, które będą wywoływały określony zestaw bezpiecznych adresów URL dla sklepu PrestaShop, a tym samym uruchamia aktualizacje i inne zautomatyzowane zadania.

## CSV Export for Newsletters (newsletter) <a href="#modulyadministracyjne-csvexportfornewsletters-newsletter" id="modulyadministracyjne-csvexportfornewsletters-newsletter"></a>

Ten moduł powstał aby umożliwić eksportowanie kont e-mail zapisanych w twoim systemie do pliku CSV.\
Twoi klienci mogą przekazywać Tobie swoje adresy e-mail albo poprzez blok Newslettera znajdującego się na stronie głównej, albo zaznaczając pole "Tak" podczas rejestrowania się na stronie. Potrzebujesz tych adresów w celach marketingowych.\
Podczas rejestracji, Twoi klienci mają dwie opcje do wyboru podczas rejestracji, pierwsza to zapisać się na newsletter, druga to otrzymywać informacje handlowe od twoich partnerów (Opt-In).

### Eksportuj subskrybentów Newslettera <a href="#modulyadministracyjne-eksportujsubskrybentownewslettera" id="modulyadministracyjne-eksportujsubskrybentownewslettera"></a>

Pierwsza cześć pozwala na wyeksportowanie wszystkich adresów e-mail zapisanych z bloku Newsletter z twojej strony głównej. Plik CSV, który powstanie po naciśnięciu eksportuj, będzie się składał z kolumn: id klienta , adres e-mail, data rejestracji, oraz adres IP. Za pomocą Excela, lub innego programu do obsługi arkuszy danych, będziesz mógł łatwo przefiltrować i posegregować otrzymaną tabelę.

### Eksport klientów <a href="#modulyadministracyjne-eksportklientow" id="modulyadministracyjne-eksportklientow"></a>

W tej części możesz wstępnie przefiltrować swoją bazę danych klientów zanim utworzysz plik CSV. Na przykład filtrowanie według kraju pochodzenia jest przydatne przy wysyłaniu maila w prawidłowej wersji językowej.

Możesz również wziąć inne czynniki pod uwagę, użyj menu Subskrybenci newslettera, aby określić jedną z trzech możliwości:

* Wszyscy klienci: pozwala na zaznaczenie wszystkich adresów e-mail twoich klientów. To oznacza tych, którzy chcą otrzymywać od Ciebie wiadomości jak i tych, którzy sobie tego nie życzą.
* Subskrybenci: zaznaczy tylko tych klientów, którzy chcą otrzymywać newsletter.
* Nie zapisani: zaznaczy tylko tych klientów, którzy chcieli otrzymywać newslettera.

Następnie możesz użyć menu Subskrybenci Opt-In, gdzie możesz posortować klientów, którzy wyrazili chęć otrzymywania maili od Twoich partnerów:

* **Wszyscy klienci:** pozwala na zaznaczenie wszystkich adresów e-mail twoich klientów. To oznacza tych, którzy chcą otrzymywać wiadomości od twoich partnerów jak i tych, którzy sobie tego nie życzą.
* &#x20;**Subskrybenci:** zaznaczy tylko tych klientów, którzy chcą otrzymywać newsletter od twoich partnerów.
* &#x20;**Nie zapisani:** zaznaczy tylko tych klientów, którzy chcieli otrzymywać newslettera od twoich partnerów.

&#x20;Gdy tylko nałożysz odpowiednie filtry, naciśnij "Eksportuj plik CSV" aby otrzymać plik ze wszystkimi adresami. Plik będzie się składać z następujących kolumn: Id klienta, Nazwisko, Imię, adres e-mail, adres IP, oraz data rejestracji.

## Database Cleaner (pscleaner) <a href="#modulyadministracyjne-databasecleaner-pscleaner" id="modulyadministracyjne-databasecleaner-pscleaner"></a>

Ten moduł jest bardzo przydatny, kiedy skończysz odkrywać PrestaShop po raz pierwszy i jesteś gotów do dodawania własnych treści: Najpierw musisz usunąć wszystkie dane z wersji Demo, które zostały zainstalowane wraz z PrestaShopem, takie jak: kategorie, produkty, klienci.

Strona konfiguracji ma trzy części:

* **Katalog.** Ten proces wymaże wszystkie dane z bieżącego katalogu, także te produkty, które zostały dodane przez Ciebie. Zaznacz to pole i naciśnij "Usuń katalog", aby rozpocząć ten proces.
* **Zamówienia i klienci.** Tutaj usuniesz wszystkie dane dotyczące klientów oraz zamówień (nawet te, które sam dodałeś). Zaznacz to pole i naciśnij "Usuń zamówienia i klientów", aby rozpocząć ten proces.
* **Funkcjonalne ograniczenia integralności.** Ten proces sprawdzi Twoją bazę danych i upewni się, że wszystko jest prawidłowo ustawione, a jednocześnie spróbuje naprawić możliwe błędy.
* **Czyszczenie bazy danych.** To pozwoli na zredukowanie miejsca zajmowanego przez bazę danych i poprawi.

&#x20;**Uważaj:** każda czynność wywołana przez te funkcje, jest nieodwracalna. upewnij się że posiadasz świeżą kopię bezpieczeństwa zanim cokolwiek zrobisz.

## Email alerts (mailalerts) (Alarmy poczty) <a href="#modulyadministracyjne-emailalerts-mailalerts-alarmypoczty" id="modulyadministracyjne-emailalerts-mailalerts-alarmypoczty"></a>

PrestaShop pozwala na wysyłanie powiadomień do Ciebie i do klientów w kilku przypadkach:

* powiadomienie klientów, kiedy produkt jest niedostępny.
* powiadomienie sprzedawcy, kiedy pojawi się nowe zamówienie
* powiadomienie sprzedawcy, kiedy stan magazynowy jest poniżej pewnej granicy
* powiadomienie sprzedawcy, kiedy ponowna dostawa (pokrycie) jest poniżej pewnej ilości dni

### Powiadomienia klienta <a href="#modulyadministracyjne-powiadomieniaklienta" id="modulyadministracyjne-powiadomieniaklienta"></a>

Jest tylko jedno dostępne ustawienie:

* **Dostępność produktu** - jeśli to włączysz pojawi się informacja na stronie produktu, kiedy nie będzie go na stanie, żeby klient pozostawił swój adres email i kiedy sklep uzupełni stan magazynowy danego produktu, klient zostanie o tym poinformowany mailem.

Powiadomienia sprzedawcy

Istnieje kilka powiadomień:

* **Nowe zamówienie.** Włącz to, jeśli chcesz dostawać wiadomość za każdym razem, gdy pojawi się zamówienie.
* **Oczekiwanie na dostawię**.. Włącz to, jeśli chcesz być uprzedzany, gdy dostępność jakiegoś produktu spadnie poniżej określonego progu.
* **Ostrzeżenie pokrycia**. Jeśli to włączysz, to będziesz otrzymywać powiadomienie, jeśli jakiś produkt będzie miał inne pokrycie czasowe niż określone (domyślnie 0).

Powiadomienia mogą być wysłane jednocześnie na kilka różnych adresów, aby to zrobić zapisz każdy email w kolejnej linii.

## Google Analytics API (gapi) <a href="#modulyadministracyjne-googleanalyticsapi-gapi" id="modulyadministracyjne-googleanalyticsapi-gapi"></a>

Ten moduł pozwala na podłączenie twojego PrestaShopa do konta Google Analitics\
Najpierw musisz określić, której wersji API chcesz użyć:

* wersję 1.3 - wymaga podania Twojego adresu e-mail, hasła i profilu na Google Analitics
* wersja 3.0 - wymaga podania Twojego ID klienta, oraz profilu.

Polecamy wersję 3.0 ponieważ 1.3 jest już przestarzała. Aby nowsza wersja zadziałała musisz także uruchomić dostęp OAuth postępując według tych instrukcji: [https://developers.google.com/analytics/devguides/config/mgmt/v3/mgmtAuthorization](https://developers.google.com/analytics/devguides/config/mgmt/v3/mgmtAuthorization)

## Image watermark (watermark) Znak Wodny <a href="#modulyadministracyjne-imagewatermark-watermark-znakwodny" id="modulyadministracyjne-imagewatermark-watermark-znakwodny"></a>

Ten moduł umożliwia dodanie znaku wodnego do obrazów produktów pojawiających się w Twoim sklepie - i jednocześnie chronią je przed wykorzystywaniem przez innych.

Jeśli zamierzasz eksportować swoje produkty do Google Shopping, musisz wiedzieć, że serwis ten zakazuje używanie tekstów promocyjnych oraz znaków wodnych. Tak więc możesz przesyłać im jedynie zdjęcia bez logo i znaków wodnych.\
Przeczytaj więcej na ten temat tutaj: [https://support.google.com/merchants/answer/2700371?hl=en\&ref\_topic=2701481](https://support.google.com/merchants/answer/2700371?hl=en\&ref\_topic=2701481)

Strona konfiguracyjna poinformuje od razu o brakujących obecnie ustawieniach:

* **Plik znaku wodnego:** wybrany obraz musi być w formacie GIF.
* **Przeźroczystość (0-100)** - wartość 100 oznacza obraz nieprzeźroczysty, co oznacza, że Twoje logo będzie bardzo widoczne a jednocześnie pokryje całkowicie część obrazka, domyślna wartość 60 jest zazwyczaj dobrym kompromisem.
* **Wyrównanie w osi X**: określa położenie Twojego logo na obrazku w linii horyzontalnej
* **Wyrównanie w osi Y**: określa położenie Twojego logo na obrazku w linii wertykalnej
* **Wybierz typy obrazów dla których zastosować ochronę znakiem wodnym:** Możesz określić, które obrazy mają być chronione znakiem wodnym. Musisz to zrobić szczególnie dla dużych obrazów, ponieważ najprawdopodobniej te mogą być skradzione.

Gdy tylko zachowasz swoje ustawienia, konfiguracja zostanie zachowana, ale znak wodny nie zostanie jeszcze dodany do Twoich zdjęć. Idź najpierw do menu "Preferencje" strona "Zdjęcia", i tam naciśnij "wygeneruj ponownie miniatury". PrestaShop zajmie się wszystkimi twoimi zdjęciami i znak wodny pojawi się na typach obrazów, które zostały wybrane.

## Merchant Expertise <a href="#modulyadministracyjne-merchantexpertise" id="modulyadministracyjne-merchantexpertise"></a>

Ten moduł został specjalnie stworzony da użytkowników PrestaShopa aby pomóc im w śledzeniu ich postępów jako sprzedawców internetowych, dzięki temu mogą zobaczyć jak ich biznes rozrósł się i rozszerzył w ciągu kilku dni, tygodni, miesięcy i lat. Moduł ten jest zainstalowany domyślnie.

Ten moduł dodaje system odznak i punktów podzielonych na 3 poziomy, które są częściami składowymi Twojego sukcesu w Świecie e-commerce.

* **Funkcje**. Śledzi użycie funkcji e-commerce takich jak SEO, Site Performance, Płatności etc.
* **Osiągnięcia**. Śledzi uzyskanie pewnych określonych celów jak na przykład liczbę klientów, zamówień, obrót.
* **Międzynarodowe**. Śledzi obecność na rynkach międzynarodowych na całym świecie.

Im większy postęp odnotuje Twój sklep, tym więcej odznak i punktów otrzymasz.\
Nie ma potrzeby rejestrowania się czy wypełniania formularzy, wszystko odbywa się automatycznie, wiemy jak bardzo jesteś zajęty. Używaj tego narzędzia aby napędzać swój sklep, obserwować postępy oraz kolejne osiągnięcia.

## Wykresy NVD3 <a href="#modulyadministracyjne-wykresynvd3" id="modulyadministracyjne-wykresynvd3"></a>

NVD3 ([http://nvd3.org/](http://nvd3.org/)) jest biblioteką JavaScript, która została stworzona, aby tworzyć piękne wykresy za pomocą D3.js ([http://d3js.org/](http://d3js.org/)), biblioteką JavaScript stworzoną do obsługi dokumentów z danymi.\
Ten moduł włącza wykresy NVD3 dla Twojego użytku dostarczając efektowne wykresy.
