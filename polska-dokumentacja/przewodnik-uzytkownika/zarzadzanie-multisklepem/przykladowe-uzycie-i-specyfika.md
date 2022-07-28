# Przykładowe użycie i specyfika

/\*\<!\[CDATA\[\*/\
div.rbtoc1597140221743 {padding: 0px;}\
div.rbtoc1597140221743 ul {list-style: disc;margin-left: 0px;}\
div.rbtoc1597140221743 li {margin-left: 0px;padding-left: 0px;}\
\
/\*]]>\*/

* [Przykładowe użycie i specyfika](przykladowe-uzycie-i-specyfika.md#Przykładoweużycieispecyfika-Przykładoweużycieispecyfika)
  * [Zarządzanie katalogiem w trybie multisklep](przykladowe-uzycie-i-specyfika.md#Przykładoweużycieispecyfika-Zarządzaniekatalogiemwtrybiemultisklep)
  * [Wymiana danych pomiędzy sklepami](przykladowe-uzycie-i-specyfika.md#Przykładoweużycieispecyfika-Wymianadanychpomiędzysklepami)
    * [Wymiana danych pomiędzy sklepami](przykladowe-uzycie-i-specyfika.md#Przykładoweużycieispecyfika-Wymianadanychpomiędzysklepami.1)
    * [Dzielenie danych pomiędzy sklepami oraz grupami sklepów](przykladowe-uzycie-i-specyfika.md#Przykładoweużycieispecyfika-Dzieleniedanychpomiędzysklepamiorazgrupamisklepów)
    * [Współdzielenie produktów i kategorii](przykladowe-uzycie-i-specyfika.md#Przykładoweużycieispecyfika-Współdzielenieproduktówikategorii)
    * [Współdzielenie klientów oraz grup klientów](przykladowe-uzycie-i-specyfika.md#Przykładoweużycieispecyfika-Współdzielenieklientóworazgrupklientów)
    * [Inny szablon dla każdego sklepu/grupy sklepów](przykladowe-uzycie-i-specyfika.md#Przykładoweużycieispecyfika-Innyszablondlakażdegosklepu/grupysklepów)
    * [Specyficzne ustawienia dla każdego sklepu/grupy sklepów](przykladowe-uzycie-i-specyfika.md#Przykładoweużycieispecyfika-Specyficzneustawieniadlakażdegosklepu/grupysklepów)
  * [Zarządzanie stronami CMS w multisklepie](przykladowe-uzycie-i-specyfika.md#Przykładoweużycieispecyfika-ZarządzaniestronamiCMSwmultisklepie)
  * [Zarządzanie rabatami w trybie multisklepu](przykladowe-uzycie-i-specyfika.md#Przykładoweużycieispecyfika-Zarządzanierabatamiwtrybiemultisklepu)
  * [API i multisklep](przykladowe-uzycie-i-specyfika.md#Przykładoweużycieispecyfika-APIimultisklep)

## Zarządzanie katalogiem w trybie multisklep <a href="#przykladoweuzycieispecyfika-zarzadzaniekatalogiemwtrybiemultisklep" id="przykladoweuzycieispecyfika-zarzadzaniekatalogiemwtrybiemultisklep"></a>

W trybie multisklep, niektóre strony administracyjne PrestaShopa posiadają menu rozwijane wskazujące na wybraną konfigurację sklepu. To menu nadaje Ci kontekst: pozwala na określenie sklepu, lub grupy sklepów, dla których wprowadzasz odpowiednie zmiany.

Na przykład, gdy tworzysz nowy produkt, wybór w tym menu określi, czy dany produkt będzie dostępny dla wszystkich sklepów, dla grupy, czy może dla konkretnego sklepu.

Podczas edycji produktu, PrestaShop wyświetla powiadomienia, aby pomóc Ci zrozumieć zakres wprowadzanych zmian. Na przykład, podczas edycji produktu w sklepie A, pojawi się powiadomienie  "Uwaga, jeśli zmienisz wartość pól z pomarańczowym znakiem, ta wartość zostanie zmieniona w tym produkcie dla wszystkich sklepów". Pomarańczowe oznaczenie pojawia się przy wszystkich polach, których dotyczy ta kwestia, na przykład "Typ produktu", " Numer referencyjny" itd.

Podobnie będzie, jeśli zmienisz produkt w kontekście wszystkich sklepów, albo grupy sklepów, niektóre pola będą wyłączone: ponieważ ich zmiana ma wpływ globalny, nie można ich zmieniać. Jeśli naprawdę potrzebowałbyś zmienić ich zawartość, każde pole posiada przycisk, po zaznaczeniu którego  będziesz w stanie edytować dane pole w kontekście danego sklepu

&#x20;Jeśli dokonasz zmiany w wyłączonym polu, produkt będzie stworzony dla wszystkich sklepów określonych w danym kontekście, które jeszcze nie mają go w swoim katalogu.

## Wymiana danych pomiędzy sklepami <a href="#przykladoweuzycieispecyfika-wymianadanychpomiedzysklepami" id="przykladoweuzycieispecyfika-wymianadanychpomiedzysklepami"></a>

### Wymiana danych pomiędzy sklepami <a href="#przykladoweuzycieispecyfika-wymianadanychpomiedzysklepami.1" id="przykladoweuzycieispecyfika-wymianadanychpomiedzysklepami.1"></a>

Zduplikowane dane są określane podczas konfiguracji każdego poszczególnego sklepu,poprzez import części zawartości sklepu do nowego sklepu. Zawartość, którą można importować jest zróżnicowana: produkty, kategorie, pracownicy, moduły, reguły koszyka, dostawcy etc. Import danych jest jednorazowy, po utworzeniu sklepu nie ma prostej metody na zaimportowaniu danych ponownie z innego sklepu.

### Dzielenie danych pomiędzy sklepami oraz grupami sklepów <a href="#przykladoweuzycieispecyfika-dzieleniedanychpomiedzysklepamiorazgrupamisklepow" id="przykladoweuzycieispecyfika-dzieleniedanychpomiedzysklepamiorazgrupamisklepow"></a>

Sklepy mogą dzielić się informacjami. Dzielenie się nimi jest zarządzane przede wszystkim na poziomie grup sklepów: jedną z najważniejszych rzeczy, które należy zrozumieć podczas obsługi PrestaShopa w trybie multisklep, jest to, że wszystkie sklepy w ramach tej samej grupy mogą dzielić te same informacje - a dokładniej, trzy typy zawartości: klientów, dostępne ilości produktu, oraz zamówienia. Gdy sklep zostanie utworzony, dzielenie się danymi jest skończone: podczas gdy możesz zmienić ustawienia dotyczące ilości dostępnych produktów, nie możesz zmienić ustawień dotyczących klientów oraz zamówień.

### Współdzielenie produktów i kategorii <a href="#przykladoweuzycieispecyfika-wspoldzielenieproduktowikategorii" id="przykladoweuzycieispecyfika-wspoldzielenieproduktowikategorii"></a>

Kiedy tworzysz nowy sklep w ramach grupy, możesz określić, czy chcesz mieć wszystkie, czy tylko wybrane kategorie w nowym sklepie, które będą dokładnymi duplikatami kategorii w każdymi innym sklepie twojego PrestaShopa.

Podczas tworzenia kategorii, czy to dla konkretnego sklepu, czy dla wszystkich, PrestaShop zapisuje kategorię dla wszystkich sklepów - jest tylko po prostu ukryta w każdym sklepie gdzie nie jest ona ustawiona.

Przez przypisywanie nowych sklepów do określonej kategorii, każda zmiana w danej kategorii będzie miała wpływ na wszystkie związane z nią sklepu, nawet dla tych z innej grupy sklepów. Dlatego możesz zmienić zawartość kategorii raz dla wszystkich, także produkty.

### Współdzielenie klientów oraz grup klientów <a href="#przykladoweuzycieispecyfika-wspoldzielenieklientoworazgrupklientow" id="przykladoweuzycieispecyfika-wspoldzielenieklientoworazgrupklientow"></a>

Jak wspomniano powyżej, sklepy w tej samej grupie sklepów mogą dzielić klientów: wszystko, co musisz zrobić to ustawić odpowiednią opcję podczas tworzenia grupy sklepów.

Grupy są mniej zróżnicowane, jeśli zmienisz coś w jednym sklepie z domyślnej grupy, zmiana nastąpi również w innych sklepach, bez względu na grupę sklepów.

Jeśli chcesz mieć różne grupy klientów dla każdego sklepu, musisz utworzyć nową grupę i użyć menu rozwijanego, aby przypisać grupę z obecnym sklepem, albo grupą sklepów.

### Inny szablon dla każdego sklepu/grupy sklepów <a href="#przykladoweuzycieispecyfika-innyszablondlakazdegosklepu-grupysklepow" id="przykladoweuzycieispecyfika-innyszablondlakazdegosklepu-grupysklepow"></a>

Aby zainstalować szablon na PrestaShop, musisz skorzystać modułu importu/eksportu szablonu, aby pobrać go w pliku .zip. Gdy plik zostanie załadowany, moduł zada Ci pewne pytania dotyczące tego szablonu. W trybie multisklep, zapyta Cię również, czy chcesz włączyć ten szablon dla wszystkich sklepów, dla grupy sklepów, czy dla konkretnego sklepu w kontekście aktualnie zaznaczonych sklepów. Szablon ten będzie też dostępny dla innych sklepów, ale będzie wyłączony.

To ustawienie może być zmienione: gdy szablon jest zainstalowany w Twoim sklepie, możesz użyć strony Szablony w menu Preferencje, aby zmienić szablon w obecnym sklepie, albo w obecnej grupie sklepów, w zależności od wyboru w selektorze u góry strony.

### Specyficzne ustawienia dla każdego sklepu/grupy sklepów <a href="#przykladoweuzycieispecyfika-specyficzneustawieniadlakazdegosklepu-grupysklepow" id="przykladoweuzycieispecyfika-specyficzneustawieniadlakazdegosklepu-grupysklepow"></a>

Selektor z menu rozwijany u góry menu jest najszybszą opcją, aby bezpośrednio wprowadzać zmiany w konkretnym sklepie, albo zbiorze sklepów. Powinien być pierwszą opcją, dgo otwiera się strona administracyjna, ponieważ PrestaShop mienia dostępne opcje w zależności od kontekstu w jakim jest ustawiony: sklep, grupa sklepów, wszystkie sklepy.

To umożliwia Ci na:

* Używanie innych formatów zdjęć dla każdego sklepu/grupy
* Aktywacja/Konfiguracja modułu dla określonego sklepu
* Pozycjonowanie/wyświetlanie bloków front-office dla każdego sklepu indywidualnie
* ... i wiele więcej!

## Zarządzanie stronami CMS w multisklepie <a href="#przykladoweuzycieispecyfika-zarzadzaniestronamicmswmultisklepie" id="przykladoweuzycieispecyfika-zarzadzaniestronamicmswmultisklepie"></a>

Podczas przeglądania listy stron CMS w kontekście "Wszystkich sklepów", wyświetlone zostaną wszystkie strony wszystkich sklepów. Podobnie w kontekście grupy, wyświetlane są strony dla wszystkich sklepów z grupy.

Podczas tworzenia strony w kontekście grupy sklepów, wszystkie sklepy w tej grupie będą wyświetlać daną stronę, ale strona będzie unikalna: edytowanie jej w jednym sklepie wprowadzi zmiany w każdym z grupy.

Na stronie tworzenia strony pojawia się sekcja z listą wskazująca sklepy, których zmiany będą dotyczyć.

## Zarządzanie rabatami w trybie multisklepu <a href="#przykladoweuzycieispecyfika-zarzadzanierabatamiwtrybiemultisklepu" id="przykladoweuzycieispecyfika-zarzadzanierabatamiwtrybiemultisklepu"></a>

Podczas tworzenia reguł koszyka, albo katalogu, dostępny jest dodatkowy warunek, gdzie można określić sklep, którego dana zasada będzie dotyczyć.

## API i multisklep <a href="#przykladoweuzycieispecyfika-apiimultisklep" id="przykladoweuzycieispecyfika-apiimultisklep"></a>

Dostęp do API jest także konfigurowalny na poziomie pojedynczego sklepu i grupy sklepów. Podczas tworzenia klucza dostępowego można określić czy powiązać go ze wszystkimi sklepami, z grupą lub wybranym sklepem.
