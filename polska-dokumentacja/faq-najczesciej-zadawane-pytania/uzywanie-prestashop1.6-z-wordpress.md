# Używanie PrestaShop1.6 z WordPress

WordPress jest najczęściej używanym w sieci CMS, i jest szansa, że używasz go już na swojej stronie lub planujesz używać go na swoim blogu lub zawartości statycznej obok PrestaShop dla części e-commerce.

PrestaShop jest w stanie obsługiwać nieograniczoną liczbę stron statycznych i stron kategorii używając funkcji CMS, ale są sytuacje kiedy blog może być konieczny, lub po prostu bardziej zaawansowane funkcje CMS PrestaShop lub jego moduły nie świadczą. To jest sytuacja kiedy bardziej kompletne narzędzie jak WordPress może być przydatne.

E-commerce i CMS: z PrestaShop i WordPress obok siebie, sprawia, że masz wszytko co najlepsze z dwóch światów- tak długo jak można je skonfigurować poprawnie.

## Scenariusz <a href="#uzywanieprestashop1.6zwordpress-scenariusz" id="uzywanieprestashop1.6zwordpress-scenariusz"></a>

Są różne scenariusze, które możesz chcieć sprawdzić, w zależności od potrzeb i preferencji:

* WordPress jest zainstalowany na root URL i PrestaShop na subdomenie/podfolderu.
* PrestaShop jest zainstalowany na root URL i WordPress na subdomenie/podfolderu.
* PrestaShop i WordPress są instalowane obok siebie.

## Powinieneś je trzymać oddzielnie <a href="#uzywanieprestashop1.6zwordpress-powinienesjetrzymacoddzielnie" id="uzywanieprestashop1.6zwordpress-powinienesjetrzymacoddzielnie"></a>

Jeśli chcesz je trzymać osobno. to integracja jest prosta: najtrudniejszą rzeczą do zrobienia będzie posiadanie spójnego motywu dla dwóch aplikacji.  Można albo przystosować domyslny motyw każdej aplikacji aby wyglądały one na jak najbardziej podobnie do siebie, lub mieć projektanta/developera który zbuduje dwie spójne kompozycje dla obydwu stron. Zauważ, że szablon API PrestaShop używa swojej własnej funkcji wywoływania PHP:

* PrestaShop 1.6 Przewodnik Projektanta: [http://doc.prestashop.com/display/PS16/Przewodnik+projektanta](http://doc.prestashop.com/display/PS16/Przewodnik+projektanta)
* Dokumentacja rozwoju szablonu WordPress: [https://developer.wordpress.org/themes/getting-started/](https://developer.wordpress.org/themes/getting-started/)

Aby zoorientować się jak może działać motyw kombi PrestaShop-WordPress, sprawdź darmowy szablon Velvet Sky: [http://www.smashingmagazine.com/2011/06/26/free-prestashop-and-wordpress-e-commerce-theme-velvet-sky/](http://www.smashingmagazine.com/2011/06/26/free-prestashop-and-wordpress-e-commerce-theme-velvet-sky/) (Uwaga: nie jest kompatybilny z PrestaShop 1.6+).

## Miksuj do woli <a href="#uzywanieprestashop1.6zwordpress-miksujdowoli" id="uzywanieprestashop1.6zwordpress-miksujdowoli"></a>

Możesz chcieć mieszać obydwa motywy. Na przykład może chcesz zobaczyć zawartość WordPress pomiędzy pełnymi kolumnami treści PrestaShop (nowe produkty, aktualny koszyk, itd). Podobnie możesz chcieć żeby twój sklep wyświetlał linki do treści WordPress. Wszystko to i więcej może być z kilku  dobrze dobranych wtyczek WordPress i modułach PrestaShop.

Dwie wtyczki WordPress mogą być pomocne:

* PrestaShop Integrator ([http://wordpress.org/plugins/prestashop-integration/](http://wordpress.org/plugins/prestashop-integration/)) dodaje 3 widżety i shortcode do instalacji WordPress:
  * Integracja PrestaShop widżet Hook: Możesz zintegrować każdy z czterech hooków PrestaShop do dowolnych motywów WordPress: Na górze stron, w bloku lewej kolumny, w bloku prawej kolumny, stopce.
  * Widżet modułu integracji PrestaShop: Możesz wstawić moduł PrestaShop w szablonie WordPress, poprzez jeden z hooks PrestaShop.
  * Integracja widżetu Produktów PrestaShop: Wyświetlić liste produktów dołączanych w post WordPress.
  * `[ps_product_list]` shortcode: Te hooks sprawiają, że możliwe jest wyświetlanie produktów z każdej kategorii PrestaShop do strony albo postu WordPress.
* Zgodność użytkownika Prestashop ([http://wordpress.org/plugins/prestashop-user-compatibility/](http://wordpress.org/plugins/prestashop-user-compatibility/)) twoi użytkownicy PrestaShop mają możliwość logowania się do WordPress.

Jako alternatywę, możesz użyć tych wtyczek WordPress:

* WordPress-PrestaShop Sprzedaż Krzyżowa ([http://wordpress.org/plugins/wordpress-prestashop-cross-sales/](http://wordpress.org/plugins/wordpress-prestashop-cross-sales/)) zawiera produkty PrestaShop na twoim post albo pasku bocznym WordPress.
* Integracja DeMomentSomTres PrestaShop ([http://wordpress.org/plugins/demomentsomtres-prestashop/](http://wordpress.org/plugins/demomentsomtres-prestashop/)) integracja treści z PrestaShop do WordPress z użyciem serwisu internetowego PrestaShop i WordPress shortcodes.

Z drugiej strony, PrestaShop ma dedykowane moduły WordPress (ale większość jest płatna):

* WordPress Sync ([http://addons.prestashop.com/pl/495-blog-forum-aktualnosci](http://addons.prestashop.com/pl/495-blog-forum-aktualnosci)) pomaga zintegrować twój blog z twoim sklepem. Możesz importować treści i trzymać je obydwie w sync.
* WordPress Cart ([http://addons.prestashop.com/pl/451-import-eksport-danych](http://addons.prestashop.com/pl/451-import-eksport-danych)) łączy twój blog WordPress z twoim sklepem PrestaShop. Wyświetla twój koszyk zakupów i linki do konta użytkownika.
* PrestaShop to WordPress ([http://addons.prestashop.com/pl/1174-prestashop-to-wordpress.html](http://addons.prestashop.com/pl/1174-prestashop-to-wordpress.html)) umożliwia na wstawienie do sześciu widżetów na swoim blogu WordPress: Koszyk, kategorie, producentów, nowe produkty, promocje i najczęściej kupowane.
