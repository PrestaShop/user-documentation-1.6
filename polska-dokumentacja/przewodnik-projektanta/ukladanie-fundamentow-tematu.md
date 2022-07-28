# Układanie Fundamentów Tematu

* [Układanie Fundamentów Tematu](ukladanie-fundamentow-tematu.md#UkładanieFundamentówTematu-UkładanieFundamentówTematu)
  * [Odkrywanie prawdy, opierając się na wcześniejszych odkryciach: Kopiowanie domyślnego motywu](ukladanie-fundamentow-tematu.md#UkładanieFundamentówTematu-Odkrywanieprawdy,opierającsięnawcześniejszychodkryciach:Kopiowaniedomyślnegomotywu)
    * [Z Panelu administracyjnego](ukladanie-fundamentow-tematu.md#UkładanieFundamentówTematu-ZPaneluadministracyjnego)
    * [Z poziomu systemu operacyjnego/ serwera FTP](ukladanie-fundamentow-tematu.md#UkładanieFundamentówTematu-Zpoziomusystemuoperacyjnego/serweraFTP)
    * [Czyszczenie](ukladanie-fundamentow-tematu.md#UkładanieFundamentówTematu-Czyszczenie)
      * [Niezbędne moduły](ukladanie-fundamentow-tematu.md#UkładanieFundamentówTematu-Niezbędnemoduły)
      * [Konieczne moduły](ukladanie-fundamentow-tematu.md#UkładanieFundamentówTematu-Koniecznemoduły)
      * [Moduły które dobrze mieć](ukladanie-fundamentow-tematu.md#UkładanieFundamentówTematu-Modułyktóredobrzemieć)
    * [Tworzenie treści](ukladanie-fundamentow-tematu.md#UkładanieFundamentówTematu-Tworzenietreści)
    * [Projekt !](ukladanie-fundamentow-tematu.md#UkładanieFundamentówTematu-Projekt!)
      * [Pliki CSS](ukladanie-fundamentow-tematu.md#UkładanieFundamentówTematu-PlikiCSS)
      * [Obrazy](ukladanie-fundamentow-tematu.md#UkładanieFundamentówTematu-Obrazy)
      * [Pliki Szablonu](ukladanie-fundamentow-tematu.md#UkładanieFundamentówTematu-PlikiSzablonu)
      * [Pliki PDF](ukladanie-fundamentow-tematu.md#UkładanieFundamentówTematu-PlikiPDF)
  * [Rozdrapywać daną rzecz: Tworzenie wszystkich plików od zera](ukladanie-fundamentow-tematu.md#UkładanieFundamentówTematu-Rozdrapywaćdanąrzecz:Tworzeniewszystkichplikówodzera)

Dwa pierwsze rozdziały tego przewodnika były teoretyczne; ten będzie praktyczny.

Zamierzamy stworzyć fundamenty plików i folderów dla twojego tematu, są dwie drogi żeby to osiągnąc:

* Zduplikowac domyślny motyw i dostosuj pliki..
* Tworzenie każdego pliku od podstaw.

Nie trzeba dodawać, że radzimy wybrać pierwszą opcje:Minimalny PrestaShop wymaga wielu plików i lini kodu, o niektórych z nich możesz zapomnieć kiedy startujesz od zera.

Budowanie PrestaShop jest skomplikowanym przedsięwzięciem. Na przykład w porównaniu z motywem WordPress, który może pracować z pojedynczym plikiem `index.php`, minimalny PrestaShop wymaga wiele więcej stron: Stronę domową, stronę produktu, strony konta użytkownika, stronę koszyka, strony procesu zamówienia, itd. Budowanie motywu strony e-commerce oznacza o wiele bardziej skomplikowane zestawienie ze sobą stron i szablonów.

To dlatego radzimy, aby rozpocząć swój własny motyw za pomocą fundamentów położonych przez domyślny motyw. Kompletny i sprawdzony, domyślny motyw PrestaShop zapewnia, że wszystkie niezbędne strony są już na miejscu, pozostawiając swobodę przerobienia wyświetlanej strony, korzystając z własnych obrazów, w celu zwiększenia jej własnych skryptów.

## Odkrywanie prawdy, opierając się na wcześniejszych odkryciach: Kopiowanie domyślnego motywu <a href="#ukladaniefundamentowtematu-odkrywanieprawdy-opierajacsienawczesniejszychodkryciach-kopiowaniedomysln" id="ukladaniefundamentowtematu-odkrywanieprawdy-opierajacsienawczesniejszychodkryciach-kopiowaniedomysln"></a>

Duplikowanie plików z domyślnego motywu jest łatwe, a nawet jest to możliwe za pomocą dwóch różnych sposobów.

### Z Panelu administracyjnego <a href="#ukladaniefundamentowtematu-zpaneluadministracyjnego" id="ukladaniefundamentowtematu-zpaneluadministracyjnego"></a>

Panel administracyjny PrestaShop może pomóc stworzyć nowy katalog tematyczny na podstawie jakiegokolwiek innego zainstalowanego motywu, a to wszystko w kilka kliknięć:

1. Przejdź do "Szablony" strona preferencji.
2. Kliknij przycisk "Dodaj nowy szablon" w prawym górnym rogu ekranu.
3. W oknie "Importuj szablon" które zostanie otwarte, przejdź do sekcji "Utwórz nowy szablon" i kliknij przycisk "Tworzenie nowego szablonu".
4. W utworzonym formularzu wypełnij różne pola:
   * **Nazwa szablonu**.Daj mu swoją unikalną nazwę - można na przykład poprzedzić ją nazwą swojej firmy lub inicjałami. Upewnij się na stronie Addonsów, że żaden inny szablon nie używa tej nazwy, tym bardziej jeśli zamierzasz sprzedać ten szablon w internecie.
   * **Podgląd obrazu w szablonie**. Ponieważ nie masz jeszcze ostatecznego projektu do szablonu, można to zrobić póżniej&#x20;
   * **Domyślna lewa kolunma/Domyślna prawa kolumna**. Czy planujesz mieć na swoim szablonie boczny pasek tresći? Jeśli tak to po której stronie? Sprawdź odpowiednie opcje.
   * **Ilość produktów na stronie.**  Kolejne pole informacyjne które możesz edytować później.
   * **Nazwa katolgu szablonu.** Powinieneś użyć tej samej nazwy co nazwa szablonu, małymi literami spacje zastąpić myślnikami. Na przykład,"Mój Testowy Szablon" będzie się nazywał "mój testowy-szablon" jako nazwa folderu.
   * **Kopiowanie brakujących plików z istniejącego tematu**. W tym miejscu należy wskazać temat, aby skopiować pliki. To jest bardzo ważne! Możesz wybrać domyśny temat, albo wszystkie inne dostepne z których chcesz zbudować swój temat.
   * **Responsywność**. Czy planujesz, aby twój projekt szablonu dostosowywał się do każdego rozmiaru ekranu? Jeśli tak to włącz tą opcje na "Tak".
5. Kliknij przycisk "Zapisz".

PrestaShop utworzy folder szablonu i skopiuje wszystkie potrzebne pliki ze szablonu źródłowego, dzięki czemu można swobodnie eksperymentować z tymi plikami.

### Z poziomu systemu operacyjnego/ serwera FTP <a href="#ukladaniefundamentowtematu-zpoziomusystemuoperacyjnego-serweraftp" id="ukladaniefundamentowtematu-zpoziomusystemuoperacyjnego-serweraftp"></a>

Oczywiście, że można tworzyć kopie samemu:

1. Przejdź do folderu`/themes` w instalacji PrestaShop (online lub na pulpicie)
2. Stwórz nowy folder dla swojego szablonu. Powinna to być ostateczna nazwa twojego szablonu, w jednym słowie małymi literami. Upewnij się czy na stronie Addons żaden inny szablon nie używa już tej nazwy, tym bardziej jeśli masz plan ewentualnej sprzedaży szablonu przez internet.
3. Skopiuj treści folderu tematycznego (dla 1.6 motywu domyślnego, `/default-bootstrap`) i wklej go w nowo utworzonym folderze.

To wszystko!

### Czyszczenie <a href="#ukladaniefundamentowtematu-czyszczenie" id="ukladaniefundamentowtematu-czyszczenie"></a>

Zarówno domyślny motyw i twoja instalacja PrestaShop zawierają ładunek treści i stylów, które niekoniecznie są przydatne do twojego szablonu. Na przykład wiele, modułów jest zainstalowanych i aktywowanych domyślnie przez instalatora PrestaShop. Chociaż niektóre z nich są niezbędne do prawidłowego funkcjonowania kompletnego sklepu, inne mogą być po prostu odłożone na bok podczas budowania szablonu.\
To jest twój obowiązek jako twórcy motywu zbudować szablony i style przynajmniej dla wszystkich modułów domyslnego PrestaShop (albo dostosować te domyślne) wraz z tymi dodatkowymi modułami które mają wspierać twój szablon.

Chodzi o to, że motyw musi pochodzić z niestandardowych szablonów i plików CSS dla domyślnych modułów PrestaShop. Te pliki szablonów przechowywane są w podfolderze `/modules`  w folderze tematycznym subfolder, natomiast style są w podfolderze `/css/modules` .\
Na przykład, w domyśłnym motywie, pliki do modułu Layered Navigation mozna znaleźć w następujących ścieżkach:

* Plik szablonu: `/themes/default-bootstrap/modules/blocklayered/blocklayered.tpl` .
* Plik CSS: `/themes/default-bootstrap/css/modules/blocklayered/blocklayered.css` .

Jak widać, jeśli chcemy zmienić moduły występujące na stronie głównej, przy jednoczesnym zachowaniu jego układu, trzeba tylko zmienić swój plik CSS i zostawić sam plik szablonu. Na przykłąd aby zmienić stylistykę modułu Layered Navigation, należy umieścić swoją dostosowaną wersję w tym folderze: `/themes/YOUR_THEME/css/modules/blocklayered/blocklayered.css`. Wystarczy upewnić się że korzysta się z tej samej ścieżki dostepu do orginalnych plików modułu.

#### Niezbędne moduły <a href="#ukladaniefundamentowtematu-niezbednemoduly" id="ukladaniefundamentowtematu-niezbednemoduly"></a>

Niezbędne moduły szablonów to:

| Nazwa modułu    | Dlaczego jest niezbędny                       |
| --------------- | --------------------------------------------- |
| blok koszyka    | Wyświetla cały proces zamówienia i płatności. |
| blok moje konto | Wyświetla proces tworzenia użytkownika        |

Po prostu nie można sprzedać produktu, jeśli ywój szablon nie obsługuje tych modułów.

#### Konieczne moduły <a href="#ukladaniefundamentowtematu-koniecznemoduly" id="ukladaniefundamentowtematu-koniecznemoduly"></a>

Są również moduły, które nie są konieczne do funkcjonawania sklepu, ale powinny być uwględnione przy projektowaniu motywu. Należy starać się budować jak najlepiej swój szablon mając te moduły w pamięci.

Konieczne moduły szablonu to:

| Nazwa modułu                 | Dlaczego jest niezbędny                                                 |
| ---------------------------- | ----------------------------------------------------------------------- |
| blok kategorii               | Wyświetla kategorie produktów                                           |
| blok cms                     | Listy i wyświetlenia stron CMS (tj. Zasady i warunki, nota prawna itp.) |
| blok kontakt                 | Wyświetla informacje o Obsłudze Klienta                                 |
| blok informacji kontaktowych | Wyświetla informacje o kontakcie do sklepu.                             |
| blok kontaktu w stopce       | Wyświetla w stopce linki do stron konta użytkownika                     |
| blok wyszukiwania            | Wyświetla wyszukiwarkę i jej wyniki                                     |
| blok tagów                   | Wyśwuetla tagi produktów                                                |
| produkty wyróżnione          | Wyświetla produkty wyróżnione                                           |

#### Moduły które dobrze mieć <a href="#ukladaniefundamentowtematu-modulyktoredobrzemiec" id="ukladaniefundamentowtematu-modulyktoredobrzemiec"></a>

W końcu moduły które nie są tak ważne jak reszta z nich , ale moga przynieść dużo korzyści dla sklepu i pomoc klientom dowiedzieć się więcej o produktach i sklepie. Powinno się zaprojektować sklep z tymi aktywnymi modułami.

Moduły szablonu które dobrze mieć to:

| Nazwa modułu               | Dlaczego jest niezbędny                                                              |
| -------------------------- | ------------------------------------------------------------------------------------ |
| blok najlepiej sprzedające | Wyświetla produkty które się najlepiej sprzedają                                     |
| blok warstwowy             | Wyświetla warstwowe filtry nawigacji                                                 |
| blok linków                | Wyświetla dodatkowe linki niestandardowe                                             |
| blok producentów           | Lista i wyświetlenia producentów/marki z produktów sklepu                            |
| blok nowych produktów      | Wyświetla najnowsze produkty                                                         |
| blok newslettera           | Wyświetla formularz, w którym klienci mogą się zapisać do newslettera Twojego sklepu |
| blok kanałów rss           | Wyświetla zawartość kanału RSS z innej strony                                        |
| blok społecznościowy       | Wyświetla informacje o stronach społecznościowych w twoim sklepie                    |
| blok specjalny             | Wyświetla bieżące rabaty                                                             |
| blok sklepu                | Wyświetla link do znajdowanego sklepu                                                |
| blok dostawcy              | Listy i wyświetlenia dostawców sklepu                                                |
| blok ostatnio przeglądane  | Wymienia produkty, które klient ostatnio oglądał                                     |
| blok listy życzeń          | Wyświetla liste życzeń klienta                                                       |
| komentarz produktów        | Wyświetla sekcje komentarza na każdej stronie produktu                               |

Wszytkie te szablony modułu są włączane domyślnie w domyślnym folderze tematu `/modules`, ponieważ są one funkcją strony czołowej są one potrzebne do tego szablonu Można bezpiecznie włączyć/odinstlować dowolny inny moduł na stronie panelu admistracyjnego "Moduły". Dzięki temu można rozpocząc z czystym kontem.

W pełni czysty stan byłby wtedy kiedy wszystkie moduły zostałyby wyłączone i ponownie zainstalowane jeden po drugim, co pozwala na włączenie ich do swojego projektu podczas tworzenia szablonu. Jest to dobry sposób pracy, który pomaga ustalić jaka treść zepsuła układ strony, ale osiągniecie celu trwa dłużej.  Przechowując znany zestaw podstawowych modułów pomaga to zbudować swój szablon szybciej, jednocześnie ma się pewność że będzie to działać w większości konfiguracji

### Tworzenie treści <a href="#ukladaniefundamentowtematu-tworzenietresci" id="ukladaniefundamentowtematu-tworzenietresci"></a>

Twój temat będzie wyświetlał treść wzięte z bazy PrestaShop. Niezależnie czy planujecie zatrzymać szablon dla siebie albo podzielić się /sprzedać go aby inni mogli z niego skorzystać, nie można po prostu rozpocząć projektowania bez zawartości, wraz z aktywacją niektórych kluczowych cech, które w każdym sklepie można używać ze sobą.

Dane demo instalowane z PrestaShop wystarczą do pomocy, ponieważ obejmują produkty, kategorie, sklepy itd. Począwszy od świeżej instalacji PrestaShop daje Tobie przewagę z zawartością demo, pusty sklep będzie wymagał aby rozpocząć dodawanie zawartości (albo fałszywe lub prawdziwe) do sklepu, aby zobaczyć jak twój szablon na to reaguje.

### Projekt ! <a href="#ukladaniefundamentowtematu-projekt" id="ukladaniefundamentowtematu-projekt"></a>

Teraz gdy domyślny motyw został przekształcony we własnym folderze, to jest czas aby zbadać jego pliki: Szablony Smarty, zasady CSS, kody JavaScript, połozenie zaczepów i bloków treści... Wszytko można zmienić, a do Ciebie należy decyzja jak chcesz to przerobić!

#### Pliki CSS <a href="#ukladaniefundamentowtematu-plikicss" id="ukladaniefundamentowtematu-plikicss"></a>

Możesz edytować styl tematu poprzez edycje plików CSS.

Plik `global.css` zawiera globalną strukturę i najważniejszą część projektowania szablonu

Zazwyczaj jest jeden arkusz stylów na kontroler. Na przykład strona produktu ma plik `product.css` .

Jeśli używasz Sass/Compass, musisz najpierw edytować pliki SCSS, następnie zregenrować pliki CSS.\
Gdy arkusz stylów jest generowany z pliku SCSS, linia i plik SCSS są wymienione w pliku.**Sample code from product.css**

```
/* line 6, ../sass/product.scss */
.primary_block {
  margin-bottom: 40px;
}
/* line 9, ../sass/product.scss */
.top-hr {
  background: #c4c4c4;
  height: 5px;
  margin: 2px 0 31px;
}
```

```
.primary_block {
  margin-bottom: 40px;
}
.top-hr{
  background: $top-line-color;
  height: 5px;
  margin: 2px 0 31px;
}
```

#### Obrazy <a href="#ukladaniefundamentowtematu-obrazy" id="ukladaniefundamentowtematu-obrazy"></a>

Obrazy które są używane przez szablon (nie przez produkty) są przechowywane w folderze szablonu`/img` , natomiast obrazy które mają być użyte przez sklep są przechowywane w folderze głównym `/img` instalacji PrestaShop.

Ikony są szczególnym przypadkiem: PrestaShop 1.6 używa FontAwesome jako zestaw ikon: [http://fontawesome.io/](http://fontawesome.io/). Jest to trzcionka wykonana z ikon, co daje wektorowe skalowanie ikon, które można błyskawicznie dostosować.

Używanie FontAwesome pozwala na:

* użycie pojedynczego pliku do wyświetlania różnych ikon.
* cieszyć się elastycznością: Rozmiaru, koloru, cieni, i wszystkim tym co można zrobić z mocą CSS.
* doskonałe renderowanie na wszystkich rozmiarach ekranów: PC, TV, Retina, itd.)

#### Pliki Szablonu <a href="#ukladaniefundamentowtematu-plikiszablonu" id="ukladaniefundamentowtematu-plikiszablonu"></a>

Pliki szablonu Smarty  (`.tpl`) jest sposobem na odzielenie treści od sposobu w jaki treść jest prezentowana.\
Szablon ma tylko kilka dynamicznych elementów (gdzie idzie zawartość). Ułatwia to projektowanie i aktualizacje Twoich obydwu stron, za równo w odniesieniu do treści jak i jej prezentacji.**Template file for the HTTP 404 Error page**

```
<div class="pagenotfound">
    <div class="img-404">
        <img src="{$img_dir}/img-404.jpg" alt="{l s='Page not found'}" />
    </div>
    <h1>{l s='This page is not available'}</h1>
    <p>
        {l s='We\'re sorry, but the Web address you\'ve entered is no longer available.'}
    </p>
    <h3>{l s='To find a product, please type its name in the field below.'}</h3>
    <form action="{$link->getPageLink('search')|escape:'html':'UTF-8'}" method="post" class="std">
        <fieldset>
            <div>
                <label for="search_query">{l s='Search our product catalog:'}</label>
                <input id="search_query" name="search_query" type="text" class="form-control grey" />
                <button type="submit" name="Submit" value="OK" class="btn btn-default button button-small">
                    <span>{l s='Ok'}</span>
                </button>
            </div>
        </fieldset>
    </form>
    <div class="buttons">
        <a class="btn btn-default button button-medium" href="{$base_dir}" title="{l s='Home'}">
            <span><i class="icon-chevron-left left"></i>{l s='Home page'}</span>
        </a>
    </div>
</div>
```

Silnik szablonu używa {...} do obsługi instrukcji. Pozostała część dokumentu jest wysyłana do przeglądarki

Możliwe jest użycie szablonu do generowania plików HTML, a także plikó XML, plików tekstowych etc.

#### Pliki PDF <a href="#ukladaniefundamentowtematu-plikipdf" id="ukladaniefundamentowtematu-plikipdf"></a>

Pliki PDF są także generowane z szablonów Smarty (`.tpl` pliki). Główna różnica między tym jak pliki szablonów używają do generowania HTML, jest taka że szablony PDF nie pozwalają na zasoby zewnętrzne takie jak CSS. Dlatego należy użyć wewnętrznej stylizacji albo inline, aby zmienić styl twojej faktury, opóźnienia zamówienia, opóźnienia zwrotu, etc. Domyśłna isnatalcja PrestaShop pochodzi z dwóch stylów szablonów: `delivery-slip.style-tab.tpl` i `invoice.style-tab.tpl`. Możesz je w znaleźć folderze`/pdf/`. Poniższa tabela pokazuje jak zakładki stylu są powiązane:

| Szablon PDF         | Zakładka stylu                |
| ------------------- | ----------------------------- |
| Opóźnienia dostawy  | `delivery-slip.style-tab.tpl` |
| Kolejność dostawy   | `invoice.style-tab.tpl`       |
| Zwroty zamówienia   | `invoice.style-tab.tpl`       |
| Faktura             | `invoice.style-tab.tpl`       |
| Opóźnienia zamówień | `invoice.style-tab.tpl`       |

Zauważ, że jeśli chcesz zastosować inny szablon stylu, trzeba będzie zastąpić odpowiedni PDF Class w katalogu `/classes/pdf/`.

Wewnętrzna zakładka w katalogach stylu może być stosowana tylko do głównych plików szablonów PDF, takich jak `invoice.tpl`, `delivery-slip.tpl`, etc. W celu ponownego użycia zmiennych w szablonach które są włączone w szablonach, można przypisać zmienne Smarty lub zastosować stylizacje inline odzielnie w każdym z tych plików.

## Rozdrapywać daną rzecz: Tworzenie wszystkich plików od zera <a href="#ukladaniefundamentowtematu-rozdrapywacdanarzecz-tworzeniewszystkichplikowodzera" id="ukladaniefundamentowtematu-rozdrapywacdanarzecz-tworzeniewszystkichplikowodzera"></a>

Oh naprawdę? Chcesz zrobić to ręcznie? To odważne, ale postaramy się pomóc

Po pierwsze, jets lista niezbędnych plików szablonów (First, here is the list of necessary template files (spoiler alert: istnieje z ich 60, Tak wszystkie są konieczne do różnych funkcji PrestaShop):

| Nazwa pliku                              | Dlaczego jest niezbędny                                                                       | Inne pliki szablonów używane przez ten szablon w domyślnym temacie                                                                                                                                                                       |
| ---------------------------------------- | --------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 404.tpl                                  | Wyświetla się kiedy plik nie może być znaleziony                                              |                                                                                                                                                                                                                                          |
| address.tpl                              | Umożliwia kientowi stworzyć nowy adres.                                                       | <ul><li>errors.tpl</li></ul>                                                                                                                                                                                                             |
| addresses.tpl                            | Umożliwia klientowi oglądanie aktualnych adresów                                              |                                                                                                                                                                                                                                          |
| authentication.tpl                       | Umożliwia klientowi zalogować się do jego konta.                                              | <ul><li>order-steps.tpl</li><li>errors.tpl</li></ul>                                                                                                                                                                                     |
| best-sales.tpl                           | Wyświetla najlepiej sprzedające się produkty.                                                 | <ul><li>product-sort.tpl</li><li>nbr-product-page.tpl</li><li>product-compare.tpl</li><li>pagination.tpl</li><li>product-list.tpl</li></ul>                                                                                              |
| breadcrumb.tpl                           |  Wyświetla ścieżkę kategorii, do obecnego produktu/kategorii                                  | <ul><li>breadcrumb.tpl</li></ul>                                                                                                                                                                                                         |
| category-cms-tree-branch.tpl             | Biegnie przez kategorie CMS w celu ich wyświetlania.                                          | <ul><li>category-cms-tree-branch.tpl</li></ul>                                                                                                                                                                                           |
| category-count.tpl                       | Wyświetla liczbę produktów w kategorii                                                        |                                                                                                                                                                                                                                          |
| category-tree-branch.tpl                 | Biegnie przez kategorie produktów w celu ich wyświetlenia.                                    | <ul><li>category-tree-branch.tpl</li></ul>                                                                                                                                                                                               |
| category.tpl                             | Wyświetla zawartość kategorii: widoku, obrazu, tekstu, porównywarki produktów itd.            | <ul><li>errors.tpl</li><li>scenes.tpl</li><li>category-count.tpl</li><li>product-sort.tpl</li><li>nbr-product-page.tpl</li><li>product-compare.tpl</li><li>pagination.tpl</li><li>product-list.tpl</li><li>product-compare.tpl</li></ul> |
| cms.tpl                                  | Wyświetla zawartość strony CMS.                                                               |                                                                                                                                                                                                                                          |
| contact-form.tpl                         | Wyświetla formularz kontaktowy klienta.                                                       | <ul><li>errors.tpl</li></ul>                                                                                                                                                                                                             |
| discount.tpl                             | Wyświetla listę kuponów klienta                                                               |                                                                                                                                                                                                                                          |
| errors.tpl                               | Wyświetla aktualny błąd/błędy                                                                 |                                                                                                                                                                                                                                          |
| footer.tpl                               | Wyświetla stopkę                                                                              | <ul><li>global.tpl</li></ul>                                                                                                                                                                                                             |
| global.tpl                               | Definiuje kilka zmiennych Smarty, i najbardziej znaczące z nich JavaScript                    |                                                                                                                                                                                                                                          |
| guest-tracking.tpl                       | Wyświetla stronę śledzenia dla klientów gości (interesantów bez konta)                        | <ul><li>order-detail.tpl</li></ul>                                                                                                                                                                                                       |
| header.tpl                               | Wyświetla nagłówek: HTML doctype, linki do plikó CSS, itd.                                    | <ul><li>breadcrumb.tpl</li></ul>                                                                                                                                                                                                         |
| history.tpl                              | Wyświetla wszystkie swoje poprzednie zamówienia dla klienta                                   | <ul><li>errors.tpl</li></ul>                                                                                                                                                                                                             |
| identity.tpl                             | Wyświetla i aktualizuje dane osobowe klienta                                                  | <ul><li>errors.tpl</li></ul>                                                                                                                                                                                                             |
| layout.tpl                               | Uruchamia główne paczki tematu: Nagłówek, stopkę, kolumny, aktualny szablon i edycje na żywo. | <ul><li>header.tpl</li><li>footer.tpl</li></ul>                                                                                                                                                                                          |
| maintenance.tpl                          | Wyświetla specjalną stronę gdy sklep jest w konserwacji                                       |                                                                                                                                                                                                                                          |
| manufacturer-list.tpl                    | Wyświetla listę wszystkich producentów                                                        | <ul><li>errors.tpl</li><li>nbr-product-page.tpl</li><li>pagination.tpl</li></ul>                                                                                                                                                         |
| manufacturer.tpl                         | Wyświetla produkty od tego samego producenta.                                                 | <ul><li>errors.tpl</li><li>product-sort.tpl</li><li>nbr-product-page.tpl</li><li>product-compare.tpl</li><li>pagination.tpl</li><li>product-list.tpl</li></ul>                                                                           |
| my-account.tpl                           | Wyświetla stronę konta klienta                                                                |                                                                                                                                                                                                                                          |
| nbr-product-page.tpl                     | Wyświetla liczbę produktów na bierzącej stronę                                                |                                                                                                                                                                                                                                          |
| new-products.tpl                         | Displays a block with the new products.                                                       | <ul><li>product-sort.tpl</li><li>nbr-product-page.tpl</li><li>product-compare.tpl</li><li>pagination.tpl</li><li>product-compare.tpl</li><li>pagination.tpl</li></ul>                                                                    |
| order-address-multishipping-products.tpl | Wyswietla adresy dostarczenia produktów w sytuacji multishippingu                             | <ul><li>order-address-product-line.tpl</li></ul>                                                                                                                                                                                         |
| order-address-multishipping.tpl          |                                                                                               | <ul><li>order-steps.tpl</li><li>errors.tpl</li><li>order-address-multishipping-products.tpl</li></ul>                                                                                                                                    |
| order-address-product-line.tpl           |                                                                                               |                                                                                                                                                                                                                                          |
| order-address.tpl                        |                                                                                               | <ul><li>order-steps.tpl</li><li>errors.tpl</li></ul>                                                                                                                                                                                     |
| order-carrier.tpl                        |                                                                                               | <ul><li>order-steps.tpl</li><li>errors.tpl</li></ul>                                                                                                                                                                                     |
| order-confirmation.tpl                   |                                                                                               | <ul><li>errors.tpl</li><li>order-steps.tpl</li></ul>                                                                                                                                                                                     |
| order-detail.tpl                         |                                                                                               |                                                                                                                                                                                                                                          |
| order-follow.tpl                         |                                                                                               |                                                                                                                                                                                                                                          |
| order-opc-new-account.tpl                |                                                                                               |                                                                                                                                                                                                                                          |
| order-opc.tpl                            |                                                                                               | <ul><li>shopping-cart.tpl</li><li>order-address.tpl</li><li>order-opc-new-account.tpl</li><li>order-carrier.tpl</li><li>order-payment.tpl</li><li>errors.tpl</li></ul>                                                                   |
| order-payment.tpl                        |                                                                                               | <ul><li>errors.tpl</li><li>order-steps.tpl</li><li>shopping-cart-product-line.tpl</li></ul>                                                                                                                                              |
| order-return.tpl                         |                                                                                               | <ul><li>errors.tpl</li></ul>                                                                                                                                                                                                             |
| order-slip.tpl                           |                                                                                               |                                                                                                                                                                                                                                          |
| order-steps.tpl                          |                                                                                               |                                                                                                                                                                                                                                          |
| pagination.tpl                           |                                                                                               |                                                                                                                                                                                                                                          |
| password.tpl                             |                                                                                               | <ul><li>errors.tpl</li></ul>                                                                                                                                                                                                             |
| prices-drop.tpl                          |                                                                                               | <ul><li>product-sort.tpl</li><li>nbr-product-page.tpl</li><li>product-compare.tpl</li><li>pagination.tpl</li><li>product-list.tpl</li><li>product-compare.tpl</li><li>pagination.tpl</li></ul>                                           |
| product-compare.tpl                      |                                                                                               |                                                                                                                                                                                                                                          |
| product-list-colors.tpl                  |                                                                                               |                                                                                                                                                                                                                                          |
| product-list.tpl                         |                                                                                               |                                                                                                                                                                                                                                          |
| product-sort.tpl                         |                                                                                               |                                                                                                                                                                                                                                          |
| product.tpl                              |                                                                                               | <ul><li>errors.tpl</li><li>product-list.tpl</li></ul>                                                                                                                                                                                    |
| products-comparison.tpl                  |                                                                                               |                                                                                                                                                                                                                                          |
| restricted-country.tpl                   |                                                                                               |                                                                                                                                                                                                                                          |
| scenes.tpl                               |                                                                                               |                                                                                                                                                                                                                                          |
| search.tpl                               |                                                                                               | <ul><li>errors.tpl</li><li>product-sort.tpl</li><li>nbr-product-page.tpl</li><li>product-compare.tpl</li><li>pagination.tpl</li><li>product-list.tpl</li></ul>                                                                           |
| shopping-cart-product-line.tpl           |                                                                                               |                                                                                                                                                                                                                                          |
| shopping-cart.tpl                        |                                                                                               | <ul><li>order-steps.tpl</li><li>errors.tpl</li><li>shopping-cart-product-line.tpl</li></ul>                                                                                                                                              |
| sitemap.tpl                              |                                                                                               | <ul><li>category-tree-branch.tpl</li><li>category-cms-tree-branch.tpl</li></ul>                                                                                                                                                          |
| stores.tpl                               |                                                                                               |                                                                                                                                                                                                                                          |
| store\_infos.tpl                         |                                                                                               |                                                                                                                                                                                                                                          |
| supplier-list.tpl                        |                                                                                               |                                                                                                                                                                                                                                          |
| supplier.tpl                             | Umożliwia wyświetlanie produktów za dostawcę                                                  | <ul><li>errors.tpl</li><li>product-sort.tpl</li><li>nbr-product-page.tpl</li><li>product-compare.tpl</li><li>pagination.tpl</li><li>product-list.tpl</li></ul>                                                                           |
