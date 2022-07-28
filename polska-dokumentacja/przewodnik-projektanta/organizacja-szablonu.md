# Organizacja szablonu

Zanurzmy się w organizacje szablonu: foldery, pliki, do których należą i jak je poprawnie obsługiwać.

/\*\<!\[CDATA\[\*/\
div.rbtoc1597140227833 {padding: 0px;}\
div.rbtoc1597140227833 ul {list-style: disc;margin-left: 0px;}\
div.rbtoc1597140227833 li {margin-left: 0px;padding-left: 0px;}\
\
/\*]]>\*/

* [Organizacja szablonu](organizacja-szablonu.md#Organizacjaszablonu-Organizacjaszablonu)
  * [Foldery](organizacja-szablonu.md#Organizacjaszablonu-Foldery)
    * [Pliki miniatur](organizacja-szablonu.md#Organizacjaszablonu-Plikiminiatur)
    * [CSS i Sass](organizacja-szablonu.md#Organizacjaszablonu-CSSiSass)
      * [CSS](organizacja-szablonu.md#Organizacjaszablonu-CSS)
      * [Sass / Compass](organizacja-szablonu.md#Organizacjaszablonu-Sass/Compass)
    * [Trzcionka](organizacja-szablonu.md#Organizacjaszablonu-Trzcionka)
    * [Obraz](organizacja-szablonu.md#Organizacjaszablonu-Obraz)
    * [JavaScript](organizacja-szablonu.md#Organizacjaszablonu-JavaScript)
    * [Język](organizacja-szablonu.md#Organizacjaszablonu-Język)
    * [Szablon mobilny](organizacja-szablonu.md#Organizacjaszablonu-Szablonmobilny)
  * [Pliki](organizacja-szablonu.md#Organizacjaszablonu-Pliki)
    * [Pliki Szablonów](organizacja-szablonu.md#Organizacjaszablonu-PlikiSzablonów)
    * [Arkusze stylów](organizacja-szablonu.md#Organizacjaszablonu-Arkuszestylów)
    * [Pliki obrazów](organizacja-szablonu.md#Organizacjaszablonu-Plikiobrazów)
    * [Narzędzia](organizacja-szablonu.md#Organizacjaszablonu-Narzędzia)

## Foldery <a href="#organizacjaszablonu-foldery" id="organizacjaszablonu-foldery"></a>

To są główne foldery motywu PrestaShp:

* Folder`/cache` zawiera wszystkie pliki tymczasowe, które są generowane i ponownie wykorzystane w celu zmniejszenia obciążena serwera. Folder jest domyslnie pusty.
* Folder `/css` zawiera wszystkie pliki CSS.\

  * Folder `/sass` zawiera wszystkie pliki żródłowe Sass `.scss`, za nim zostaną one skompilowane plikach CSS.
* Folder`/font` zawiera niezbędne pliki trzcionek.
* Folder `/img` zawiera wszystkie obrazy.
* Folder`/js` zawiera wszystkie pliki JavaScript.
* Folder`/lang` zawiera wszystkie tematy tłumaczeń. Jego prawa dostepu powinny być ustawione na CHMOD 666 (na przykład), tak że narzędzie do tłumaczenia w panelu administracyjnym może odczytywać i zapisywać do niego.

Nastepujące foldery nie są bezpośrednio związane tematycznie, ale mają pomóc upewnić się, że cała funkcja PrestaShop ma konstrukcje któa jest zgodna z szablonem:

* Folder`/mails` zawiera szablony które wysyła PrestaShop (potwierdzenie zamówienia, żądanie chasła, powiadomienia wysyłki itp.).
* Folder`/mobile` zawiera mobilną wersje motywu,
* Folder`/modules` zawiera pliki szablonu dla wielu modułów.
* Folder`/pdf` zawiera pliki szablonu dla plików PDF, które PrestaShop generuje ( folder contains the template files for the PDF files that PrestaShop generates (faktury, potweirdzenie dostawy, zamówienia dostawy, itd.).

Folder root zawiera tylko pliki TPL, a także pliki miniatur `preview.jpg` .

### Pliki miniatur <a href="#organizacjaszablonu-plikiminiatur" id="organizacjaszablonu-plikiminiatur"></a>

Plik  `preview.jpg`  w katologu głównym w folderze szablonu jest miniaturą która jest używana przez selektor motywów w panelu administracyjnym PrestaShop.

Służy ona jako wizualne przypomienie tego co jest tematem, a zatem należy zrobić zrzut ekranu zamiast loga firmy.

To może mieć dowolny rozmiar - domyślny motyw ma 180'445 pikseli.

Musi to być plik JPEG.

### CSS i Sass <a href="#organizacjaszablonu-cssisass" id="organizacjaszablonu-cssisass"></a>

#### CSS <a href="#organizacjaszablonu-css" id="organizacjaszablonu-css"></a>

Pliki szablonu CSS są zlokalizowane w folderze `/css`.

Zaleca się, aby mieć wspólny arkusz stylów dla globalnych reguł CSS: `global.css`.\
Następnie każdy regulator powinien mieć własny plik CSS na przykład, `product.css` dla strony produktu.

#### Sass / Compass <a href="#organizacjaszablonu-sass-compass" id="organizacjaszablonu-sass-compass"></a>

Pliki Sass i Compass są opcjonalne: Nie trzeba używać tych narzędzi to tworzenia plików CSS dla motywu panelu administracyjnego.

Jeśli używasz Sass i Compass radzimy umieścić pliki żródłowe`.scss` w temacie `/sass`, aby inni programiści mogli mieć dostep do motywu i łatwiej mogli go przerobić.

Stamtąd możesz generować pliki CSS w folderach`/css` z plikami Sass w folderze `/sass` !

### Trzcionka <a href="#organizacjaszablonu-trzcionka" id="organizacjaszablonu-trzcionka"></a>

Folder`/font` jest opcjonalny: Zawiera trzcionki które używa się do tworzenia motywu.

Na przykład domyslny motyw PrestaShop używa trzcionkę Font Awesome ([http://fortawesome.github.io/Font-Awesome/](http://fortawesome.github.io/Font-Awesome/)) dla responsywnych ikon i w związku z tym ma następujące pliki z folderu `/font`:

* `fontawesome-webfont.eot`
* `fontawesome-webfont.svg`
* `fontawesome-webfont.ttf`
* `fontawesome-webfont.woff`

Jeśli nie tworzysz swojego szablonu z konkretnej trzcionki, lub zestawu ikon możesz pominąć ten folder.

### Obraz <a href="#organizacjaszablonu-obraz" id="organizacjaszablonu-obraz"></a>

Obrazy związane tematycznie powinny być przechowywane w folderze `/img`.

Można utworzyć podfolder dla lepszej organizacji. Na przykład, domyślny motyw ma następujące podfoldery:

* `/icon` dla prostych ikon (na przykład, nie są dostępne z wybranym wymiarem czcionek).
* `/jquery` dla specyficznych obrazów jQuery. .

Można stworzyć więcej jeśli jest taka potrzeba.

### JavaScript <a href="#organizacjaszablonu-javascript" id="organizacjaszablonu-javascript"></a>

Pliki JavaScript mają być przechowywane w folderze `/js` .

W przeciwieństwie do plików CSS, zalecamy, aby nie mieć współnego pliku/globalnego JavaScript, ani nie powinień być pojedynczy plik za kontrolera.

### Język <a href="#organizacjaszablonu-jezyk" id="organizacjaszablonu-jezyk"></a>

Wszystkie pliki z tłumaczeniami powinny być przechowywane w folderze `/lang`.

Pliki powinny się nazywać po ich ISO 3166-1 alpha-2 kod z małej litery na przykład, `fr.php`.

Pliki te pownny być generowane przez zintegrowane narzędzie do tłumaczenia PrestaShop (znajduje się w menu Lokalizacja/Tłumaczenia).

### Szablon mobilny <a href="#organizacjaszablonu-szablonmobilny" id="organizacjaszablonu-szablonmobilny"></a>

Domyślny motyw PrestaShop 1.6 ijest w pełni responsywny, co oznacza, że dostosowuje się do każdego rodzaju ekranu. .

Twój własny motyw graficzny powinien być także responsywny! Jeśli nie jest, to powinieneś stworzyć alternatywny szablon ukierunkowany na mniejsze ekrany - albo użyj/dostosować jeden z dostepnych domyślnych szablonów PrestaShop 1.5.

PrestaShop posiada w panelu adminstracyjnym opcje szablonu mobilnego: Na stronie Preferencje/Motywy, "Mobilne" w zakładce "Twój aktualny szablon" sekcja daje Tobie następujące możliwości: Wyłącz opcje, lub włącz ją dla smarfonów, tabletów lub obydwu z nich.

Gdy ta opcja jest włączona, to szablon który jest wyświetlany na telefonie użytkownika nie jest domyślnym szablonem pulpitu, ale alternatywnym szablonem znajdującym się w folderze`/mobile`: To lepiej nadaje się do niewielkich rozmiarów ekranu, a zatem klienci docenią różnice.

W istocie zawartość folderu`/mobile` to kolejny kompletny szablon PrestaShop: Ma taką samą ogólną strukturę pliku z własnym `/css`, `/img` i folderami `/js`, a także z własnymi plikami szablonów.

## Pliki <a href="#organizacjaszablonu-pliki" id="organizacjaszablonu-pliki"></a>

### Pliki Szablonów <a href="#organizacjaszablonu-plikiszablonow" id="organizacjaszablonu-plikiszablonow"></a>

PrestaShop używa silnika szablonu Smarty dla swojego systemu szablonów. Smarty umożliwia oddzielenie treści (informacje są prezentowane) od prezentacji (sposób w jaki informacje są wyświetlane). Plik szablonu łączy obydwa w pełny utworzony plik HTML.

Plik szablonu jest zbudowany z dwóch rodzajów bloków kodu:

* Kod który nie zmienia się w trakcie całego procesu renderowania HTML: Przede wszytkim zaprojektowane sekcje i niektóre niezmienne treści (logo, menu, linki, itd.)
* Kod który ulega zmianie w zależności od kontekstu renderowanej strony: Zmienne w kodzie są zastępowane przez rzeczywiste zawartości, który jest oczekiwany przez użytkownika w tym kontekście.

Zauważ, że można generować więcej niż tylko strony HTML ze Smarty: Pliki XML, pliki tekstu, pliki email, itd.

Zobacz na przykład stałe i zmienne bloki w 404.tpl, kiedy wyświetlany plik szablonu PrestaShop musi wysłać komunikat o błędzie 404 Nie znaleziono strony:

```
<div>
 <div>
 <img src="{$img_dir}/img-404.jpg" alt="{l s='Page not found'}" />
 </div>
 
 <h1>{l s='This page is not available'}</h1>
 <p>
 {l s='We\'re sorry, but the Web address you\'ve entered is no longer available.'}
 </p>
 
 <h3>{l s='To find a product, please type its name in the field below.'}</h3>
 <form action="{$link->getPageLink('search')}" method="post">
 <div>
 <label for="search_query">{l s='Search our product catalog:'}</label>
 <input id="search_query" name="search_query" type="text" />
 <button type="submit" name="Submit" value="OK">{l s='Ok'}</button>
 </div>
 </form>
 
 <div>
 <a href="{$base_dir}" title="{l s='Home'}">{l s='Home page'}</a>
 </div>
</div>

```

_(to jest uprostrzona wersja szblonu pliku, którą możesz znaleźć tutaj:_ [_https://github.com/PrestaShop/PrestaShop/blob/1.6/themes/default-bootstrap/404.tpl_](https://github.com/PrestaShop/PrestaShop/blob/1.6/themes/default-bootstrap/404.tpl)_)_

Osoby zaznajomione z HTML(które powinny być jeśli zamierzają zbudować szablon PrestaShop) natychmiast zauważą pewne`{$tag_name}` tagi w zwykłej zawartości HTML. Są to zmienne PrestaShop Smarty.

Istnieje tutaj już kilka interesujących zmiennych:

* `{$img_dir}`zwraca bezwględną ścieżkę pliiku w folderze`/img`.
* `{l s='My text'}` jest specjalna metoda ciągów, które muszą być przetłumaczone. Każdy ciąg powinien być zamknięty w sposób `{l s='...'}`.
* `{$link->getPageLink('search')}`zwraca bezwględną ścieżkę pliku do innego pliku szablonu, w tym przypadku do pliku `search.tpl` .
* `{$base_dir}` zwraca bezwględną ścieżkę pliku do katogu głównego folderu PrestaShop  – a zatem do strony głównej.

PrestaShop używa silnik Smarty 3. Możesz się dowiedzieć więcej o Smarty i jego składni tutaj: [http://www.smarty.net/docs/en/smarty.for.designers.tpl](http://www.smarty.net/docs/en/smarty.for.designers.tpl).

### Arkusze stylów <a href="#organizacjaszablonu-arkuszestylow" id="organizacjaszablonu-arkuszestylow"></a>

Pliku szablonów renderują do plików HTML, bez stylizacji (z wyjątkiem stylów inline, jeśli w ogóle), co oznacza, że bloki treści są wyświetlane jak są szkielety, jeden blok po drugim. To gdzie arkusze stylów (pliki CSS) są użyteczne: Są tutaj po to aby przedefinowac sposób w jaki bloki zawartości się wyświetlają, czasami nawet całe rozmieszczenie części strony, aby wyglądała lepiej. Czcionki, margines, kolumny i wiele innych aspektów projektowania można komponować za pomocą CSS.

Można tworzyć i edytować pliki CSS w dowolny sposób, upewniając się, że są przechowywane w folderze `/css`.\
Zaleca się aby mieć wspólny arkusz stylów dla globalnych reguł CSS: `global.css`.\
Nastepnie każdy z kontrolerów powinen mieć swój własny plik CSS: na przykład. `product.css` dla strony produktu.

Jeśli zaczynasz z plików arkuszy stylów domyślnego motywu, Powinieneś raczej zmodyfikować odpowiednie pliki w folderze Sass `/sass`, nastepnie wygenerować nowe pliki CSS i przechowywać go folderze`/css`. Zapewnia to spójność plików CSS i Sass.

Oto przykład pliku Sass:**Filename: /sass/product.scss**

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

...która zostanie wygenrowana w tych liniach CSS:**Filename: /css/product.css**

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

Jak widzisz zmienna `$top-line-color`  w pliku Sass przemienia się w wartość `#c4c4c4` w renderowanym pliku CSS. Zmienne Sass w domyślnym szablonie PrestaShop 1.6 są przechowywane w pliku `_theme_variables.scss`.

### Pliki obrazów <a href="#organizacjaszablonu-plikiobrazow" id="organizacjaszablonu-plikiobrazow"></a>

Obrazy używane przez szablon powinny być przechowywane w folderze `/img` (i podfolderze dla szczególnych przypadków, na przykład `/img/icon` dla ikon Gif `/img/jquery` dla szczególnych obrazów jQuery).\
Możesz korzystać z prawie każdego rodzaju obrazu jaki chcesz podczas tworzenia projektu.

Pod względem ikon PrestaShop używa zestawu czcionek Font Awesome przechowywanym w folderze `/font`. Używanie czcionki dla ikon ma wiele zalet:

* Pojedynczy plik dla wielu różnych ikon.
* Wiele możliwych wariantów: rozmiar, kolor, cienie, obracanie itd.
* Wyświetlanie równie dobrze na wszystkich rozmiarach i rozdzielczościach; PC, ekranch telewizorów, Retina, itd.

### Narzędzia <a href="#organizacjaszablonu-narzedzia" id="organizacjaszablonu-narzedzia"></a>

Tak na marginesie trzeba mieć solidne IDE (i jego dobrą znajomość) w celu szybkiego znalezienia poszukiwanego pliku takim narzędziem jak grep.

Należy również zapoznać się z narzędziami pre-kompilacji, aby ułatwić sobie życie.
