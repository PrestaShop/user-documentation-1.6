# Moduły Transportu i logistyki

## Oszacowanie przesyłki <a href="#modulytransportuilogistyki-oszacowanieprzesylki" id="modulytransportuilogistyki-oszacowanieprzesylki"></a>

Ten moduł pozwala klientowi na porównanie ofert dostawy przed dokonaniem finalizacji zakupu. Wystarczy go zainstalować a dodatkowe opcje pojawią się w koszyku.

Ten moduł jest bardzo prosty w instalacji, wystarczy tylko go zainstalować aby wyświetlić go na front- office.

Wszyscy dostawcy muszą mieć dobrze ustawione preferencje płatności. Sprawdź to w profilu przewoźników w menu "Wysyłka".

Strona konfiguracji ma tylko jedną opcję "Jak odświeżyć listę przewoźników". To pozwoli Ci określić w jaki sposób lista przewoźników będzie przedstawiana.

## Data Dostawy <a href="#modulytransportuilogistyki-datadostawy" id="modulytransportuilogistyki-datadostawy"></a>

Ten moduł wyświetla przybliżony czas dostawy podczas procesu składania zamówienia.

Konfiguracja  składa się z dwóch części:

* **Konfiguracji przewoźnika.** Ten moduł opiera się na informacjach od Twoich dostawców. Dlatego musisz dodać regułę dla każdego z przewoźników naciskając na przycisk "Add a new carrier rule"(Dodaj nową regułę dla przewoźnika)
* **Ustawienia:**\

  * **Dodatkowy czas kiedy produktu nie ma na stanie.** Określa czas, którego będzie potrzebować Twoja firma na sprowadzenia produktu do magazynu. Przydaje się tylko i wyłącznie, kiedy  klient ma możliwość zakupu produktów niedostępnych na magazynie (możesz uruchomić tę opcję w preferencjach Produktu, część "Ilości")
  * **Dodatkowy czas na przygotowanie zamówienia.** Określ czas, w którym zamówienie może zostać przygotowane do wysyłki.
  * **Opcja przygotowania.** Jeśli twój magazyn działa również w weekendy, określ to tutaj, ten moduł weźmie to również pod uwagę.
  * **Format daty.** Format w jakim jest wyświetlana oczekiwana data dostawy. Używa się tutaj formatu PHP date(): każda litera ma znaczenie, domyślnie "l j F Y" oznacza, że data wyświetli się w formacie: "Sobota 21 Stycznia 2012". Możesz zobaczyć wszystkie dostępne parametry na: [http://www.php.net/manual/en/function.date.php](http://www.php.net/manual/en/function.date.php)

Dodawanie nowej reguły do przewoźnika jest dość proste:

* &#x20;**Przewoźnik.** Wybierz dostawcę dla którego chcesz dodać zasadę, jeśli nie jest tutaj wymieniony, to musisz go dodać na stronie Wysyłka->Przewoźnicy.
* &#x20;**Dostawa pomiędzy**. Określ czas dostawy w którym przewoźnik zobowiązuje się dostarczyć przesyłkę. Tę informację pobierasz od dostawcy samodzielnie.
* &#x20;**Opcje przygotowania.** Niektórzy dostawcy przygotowują paczki w weekendy i wysyłają w poniedziałek rano. Pamiętaj, aby to zaznaczyć jeśli tak jest.

Należy stworzyć tyle reguł dostawy, ile tylko potrzeba.

## Globkurier <a href="#modulytransportuilogistyki-globkurier" id="modulytransportuilogistyki-globkurier"></a>

![](<../../../.gitbook/assets/23036725 (3).png>)

Moduł wysyłkowy [GlobKurier.pl](http://globkurier.pl) pomoże Ci zautomatyzować dostarczanie przesyłek. Dzięki temu modułowi będziesz mógł wysyłać paczki do 80% taniej, niż bezpośrednio z UPS, DHL. Usługa jest darmowa ! Załóż konto

Po zainstalowaniu moduł należy postępować według instrukcji.

## Śledzenie - strona sklepu <a href="#modulytransportuilogistyki-sledzenie-stronasklepu" id="modulytransportuilogistyki-sledzenie-stronasklepu"></a>

\
Ten moduł uzupełnia PrestaShop o integrację programu polecającego, który umożliwia polecającym dostęp do ich statystyk

Program polecający znajduje się na stroni "Polecający" menu Statystyki. Gdy zainstalowałeś moduł "Tracking - Front office"  (Śledzenie - strona sklepu), polecający mogą dotrzeć do programu za pomocą odnośnika: httt://adrestowjegosklepu.pl/[modules/trackingfront/stats.php](http://www.example.com/modules/trackingfront/stats.php)..

Aby utworzyć nowego polecającego naciśnij "Dodaj nowego polecającego", aby wyświetlić formularz. Tam podaj nazwę i hasło dla polecającego, a także opłaty za kliknięcie, zamówienie, oraz procent od sprzedaży.

Naciśnij w przycisk "pokaż więcej", albo 'Uzyskaj pomoc", aby dowiedzieć się jak skonfigurować polecające adresy URL.

Tryb ekspercki pozwala na korzystanie z wyrażeń regularnych zamiast pełnego tekstu adresu URL.\


## &#x20;DPD Poland <a href="#modulytransportuilogistyki-dpdpoland" id="modulytransportuilogistyki-dpdpoland"></a>

&#x20;Moduł umożliwia zarządzanie wysyłką zakupionych w sklepie produktów. Z jego pomocą przygotujesz dokumenty przewozowe jak również będziesz mógł śledzić losy przesyłek.

&#x20;Po zainstalowaniu modułu należy postępować według instrukcji.
