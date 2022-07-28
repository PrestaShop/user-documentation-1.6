# Używanie Bootstrap

## O Bootstrap <a href="#uzywaniebootstrap-obootstrap" id="uzywaniebootstrap-obootstrap"></a>

Bootstrap jest "elegancki, intuicyjny i mobilnie wydajny dla konstrukcji front-end i dla szybszego i łatwiejszego tworzenia stron " To narzędzie sprawia, że o wiele ławiej buduje się responsywne strony – to znaczy takie które adaptują się do rozmiaru ekranu, od telefonu komórkowego do dużego telewizora.&#x20;

Konstrukcja Bootstrap składa się z:

* Z konwencji kodu HTML i nazewnictwa klas CSS.
* Na bazie pliku CSS (używając formatu LESS albo Sass) zbudowany ze zbioru zmiennych.
* JavaScript dla częściej spotykanych funkcji.&#x20;

Bootstrap używa zupełnie nowego sposób pracy nad stroną internetową, która będzie naprawdę wykorzytywana w całych nadchodzący projektach – nawet tych z poza PrestaShop! Zalecamy, aby zanurzyć się w to:

* Oficjalna strona [official Bootstrap website](http://getbootstrap.com/) ma wiele punktów informacyjnych, zawiera [Getting started guide](http://getbootstrap.com/getting-started/) (w tym kompilacje kodu [overview of how it uses CSS](http://getbootstrap.com/css/), oraz wyjaśnienie [its use of JavaScript](http://getbootstrap.com/javascript/).
* Sitepoint ma kilka darmowych artykułów i tutoriali : [Understanding Twitter Bootstrap 3](http://www.sitepoint.com/understanding-twitter-bootstrap-3/), [Building Responsive Websites Using Twitter BootStrap](http://www.sitepoint.com/building-responsive-websites-using-twitter-bootstrap/), albo [Twitter Bootstrap Tutorial – Handling Complex Designs](http://www.sitepoint.com/twitter-bootstrap-tutorial-handling-complex-designs/).

## Ogólne informacje techniczne <a href="#uzywaniebootstrap-ogolneinformacjetechniczne" id="uzywaniebootstrap-ogolneinformacjetechniczne"></a>

Bootstrap wykorzystuje pewne specyficzne elementy HTML, które sprawiają, że jest to wymóg, aby korzystać z HTML5. Należy uważać, aby użyć właściwego doctype HTML5 dla wszytkich plików szablonów! \
Podobnie, CSS3 jest wykorzytsywany do wielu właściwości CSS.

```
<!DOCTYPE html>
<html lang="fr">
...
</html>
```

Bootstrap 3 jest przeznaczony do przyjaznych mobilnych stron, od początku tworzenia projektu, zamiast dodawania opcjonalnych styli mobilnych do projektu, te style są wbudowane w rdzeń projektu upewnij się, że dobrze się wyświetla na wszystkich urządzeniach.\
W celu upewnienia się, że projekt działa dobrze i że touch zoom działą zgodnie z oczekiwaniami, należy dodać `viewport` meta tag do elementu twojego szablonu `head`:

```
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

Bootstrap sprawia, że łatwiej jest zbudować projekt responsywny, i  możesz użyć małego triku żeby także twoje obrazy również były responsywne, użyj do tego klasę Boostrapa `img-responsive` w klasie obrazu.Ta klasa pozwala Twoim obrazom na użycie  `max-width: 100%;` i `height: auto;` w celu dostosowania się do elementu nadrzędnego.&#x20;

```
<img src="http://example.com/img/image.jpg" class="img-responsive" alt="Description of the image">
```

## Płynny system sieci <a href="#uzywaniebootstrap-plynnysystemsieci" id="uzywaniebootstrap-plynnysystemsieci"></a>

Bootstrap używa 12-kolumnowy system sieci, dzięki której można zbudować fluid layout. Można użyć zapytania do mediów, aby wskazać punkty krytyczne w systemie sieciowym, dzięki czemu można go skalować w górę i w dół względem liczby kolumn w zależności od rozmiaru ekranu (od 480px,szerokości małych telefonów), Więc nie jest wymagane żadne zapytanie o media. Większe rozmiary ekranu są zarządane za pomocą nastepujących pytań:

```
/* Small devices (tablets, 768px and up) */
@media (min-width: @screen-sm) { ... }

/* Medium devices (desktops, 992px and up) */
@media (min-width: @screen-md) { ... }

/* Large devices (large desktops, 1200px and up) */
@media (min-width: @screen-lg) { ... }
```

Bootstrap używa przedrostków klasy urządzeń do odróżniania ich rozmiarów ekranu:

* `.col-xs-...`: ekstremalnie mały dla telefonów (< 768px)
* `.col-sm-...`: mały, dla tabletów (≥768 px)
* `.col-md-...`: średni, dla pulpitów (≥992 px)
* `.col-lg-...`: duży, dla dużych pulpitów i telewizorów (≥1200 px)

Na przykład:

* `col-xs-3`: `3` kolumny na telefonach.
* `col-md-4`: 4 kolumny na pulpitach.

Dla każdego użądzenia, Bootstrap  również zapewnia klasy CSS, co pozwala na zmianę położenia kolumny:

* `col-`_`size`_`-push-`_`col`_: przenieść kolumnę do lewa.
* `col-`_`size`_-pull-_`col`_: przenieść kolumnę do prawa.
* `col-`_`size`_-offset-_`col`_ : kolumna pozycji według drugiej kolumny.

Na przykład:

* `col-md-push-2`: Na pulpitach, przesuń tę kolumnę przez dwie kolumny w lewo.

## Bootstrap & Sass: Używanie zmiennych i wstawek <a href="#uzywaniebootstrap-bootstrap-and-sass-uzywaniezmiennychiwstawek" id="uzywaniebootstrap-bootstrap-and-sass-uzywaniezmiennychiwstawek"></a>

### Zmienne <a href="#uzywaniebootstrap-zmienne" id="uzywaniebootstrap-zmienne"></a>

Możesz konfigurować Bootstrap poprzez edytowanie zmiennych w pliku `_variables.scss` . Na przykład:

```
@grid-columns: 12;
@grid-gutter-width: 30px;
@grid-float-breakpoint: 768px;
```

### Wstawki <a href="#uzywaniebootstrap-wstawki" id="uzywaniebootstrap-wstawki"></a>

Wstawka pozwala tworzyć grupy deklaracji CSS, które chcesz ponownie użyć na całęj swojej stronie. Na przykład:

```
@mixin border-radius($radius) {
  -webkit-border-radius: $radius;
     -moz-border-radius: $radius;
      -ms-border-radius: $radius;
          border-radius: $radius;
}

.box { @include border-radius(10px); }
```

Można zastosować zdefiniowane wstawki nowego stylu. Na przykład:

```
.wrapper {
  .make-row();
}
.content-main {
  .make-lg-column(8);
}
.content-secondary {
  .make-lg-column(3);
  .make-lg-column-offset(1);
}
```

...z następującego kodu HTML:

```
<div class="wrapper">
  <div class="content-main">...</div>
  <div class="content-secondary">...</div>
</div>
```

## Klasy Bootstrap <a href="#uzywaniebootstrap-klasybootstrap" id="uzywaniebootstrap-klasybootstrap"></a>

Bootstrap ma wiele domyślnych klas CSS, i jednocześnie PrestaShop definiuje kilka kolejnyc, które pomoga Ci zbudować spójną konstrukcje.

### Klasy Pomocnicze <a href="#uzywaniebootstrap-klasypomocnicze" id="uzywaniebootstrap-klasypomocnicze"></a>

Klasy te są używane kiedy projektuje się element który wykorzystuje jedną z PrestaShop [Klasy pomocnicze](http://doc.prestashop.com).

* `pull-left`: Dla lewego pływaka.
* `pull-right`: Dla prawego pływaka.
* `text-muted`: Dla szarego tekstu.
* `clearfix`: Aby zapobiec nadmiernej wielkości pływających bloków.
* `close`: Aby utworzyć przycisk zamykania (x).
* `caret`: Aby wskazać menu rozwijane&#x20;
* `center-block`: Aby wyśrodkować element.
* `show` i `hidden`: Aby pokazać/schować element.

### Klasy responsywne <a href="#uzywaniebootstrap-klasyresponsywne" id="uzywaniebootstrap-klasyresponsywne"></a>

Te klasy są użyteczne aby pokazać/ukryć element w zależności od urządzenia.

* `visible-xs` / `hidden-xs`
* `visible-sm` / `hidden-sm`
* `visible-md` / `hidden-md`
* `visible-lg` / `hidden-lg`
* `visible-print` / `hidden-print`

### Nawigacja, zakładki i menu <a href="#uzywaniebootstrap-nawigacja-zakladkiimenu" id="uzywaniebootstrap-nawigacja-zakladkiimenu"></a>

Główne klasy dla tego kontekstu są:

* `navbar` i `navbar-inner`: Klasa pojemnika na pasku nawigacyjnym.
* `navbar-fixed-top`: Aby przymocować pasek nawigacyjny na górze strony.
* `brand`: Dla strony tytułu/nazwy sklepu.
* `nav`, `nav-tabs` i `nav-pills`: Na kartach nawigacji.
* `btn` i `btn-navba`: Dla przycisków.
* `nav-collapse`, `collapse`, `data-toggle`, `data-target`: Do automatycznego ukrycia/pokazania zawartości.
* `icon-th-list`: Do wyświetlania ikon (tylko na małych ekranach: `th`).

Oto przykład nawigacji z menu z prawej strony:

```
<div class="navbar navbar-fixed-top">
  <div class="navbar-inner">
    <div class="container">
      <a class="btn btn-navbar" data-toggle="collapse" data-target=".nav-collapse">
        <span class="icon-th-list"></span></a>
      <a href="#" class="brand">SiteTitle</a>
      <div class="nav-collapse collapse">
        <ul class="nav pull-right">
          <li class="active"><a href="#">Home</a></li>
          <li><a href="#">About Us</a></li>
          <li><a href="#">Contact Us</a></li>
        </ul>
      </div>
    </div>
  </div>
</div>
```

Oto przykład zakładki menu:

```
<ul class="nav nav-tabs">
  <li class="active"><a href="#">Home</a></li>
  <li><a href="#">Profile</a></li>
  <li class="dropdown">
    <a href="#" data-toggle="dropdown" class="dropdown-toggle">Messages <b class="caret"></b></a>
    <ul class="dropdown-menu">
      <li><a href="#">Inbox</a></li>
      <li><a href="#">Drafts</a></li>
      <li class="divider"></li>
      <li><a class="disabled" href="#">Trash</a></li>
    </ul>
  </li>
</ul>
```

### Tabele <a href="#uzywaniebootstrap-tabele" id="uzywaniebootstrap-tabele"></a>

Główne klasy dla tabel:

* `table`, `table-responsive`: Aby utworzyć tabelę i włączyć przewijanie na mniejszych ekranach..
* `table-striped`: Aby dodać zmienne tło w wierszach.
* `table-bordered`: Aby dodać obramowanie.
* `table-hover`: Aby dodać tło do wiersza, gdy mysz go okrąża
* `table-condensed`: Aby podzielić cellpadding na dwa (sprawia, że tabela staję bardziej zwarta).
* `success`, `warning`, `danger`, etc.: Aby zmienić kolor tła wiersza lub komórki.

Przykadowe użycie::

```
<table class="table table-condensed table-hover">
<thead>
  <tr>
    <th>First Name</th>
    <th>Last Name</th>
    <th>Email</th>
  </tr>
</thead>
<tbody>
  <tr class="warning">
    <td>John</td>
    <td>Carter</td>
    <td>johncarter@mail.com</td>
  </tr>
  <tr>
    <td>Peter</td>
    <td>Parker</td>
    <td>peterparker@mail.com</td>
  </tr>
  <tr>
    <td>John</td>
    <td>Rambo</td>
    <td>johnrambo@mail.com</td>
    </tr>
  </tbody>
</table>
```

### Panele <a href="#uzywaniebootstrap-panele" id="uzywaniebootstrap-panele"></a>

Main classes for this context:

* `panel`, `panel-body`: zdefinowanie panelu.
* `panel-default`, `panel-primary`, `panel-success`, `panel-info`, `panel-warning` i `panel-danger`: W celu przystosowania układu do panelu&#x20;
* `panel-heading` i `panel-title`: W celu dodania nagłówku i tytułu w panelu.
* `panel-footer`: Aby dodać stopkę do panelu&#x20;

Przykładowe wykorzystanie:

```
<div class="panel panel-default">
  <div class="panel-heading">
    <h1 class="panel-title">Panel Title</h1>
  </div>
  <div class="panel-body">
      This is the content of the panel.
  </div>
  <div class="panel-footer clearfix">
    <div class="pull-right">
      <a href="#" class="btn btn-default">Go Back</a>
    </div>
  </div>
</div>
```

### Obrazy <a href="#uzywaniebootstrap-obrazy" id="uzywaniebootstrap-obrazy"></a>

* `img-rounded`: Do wyświetlania obrazu z zaokrąglonymi granicami.
* `img-circle`: Aby wyświetlić obraz w okręgu .
* `img-thumbnail`: Aby poradzić sobie z miniaturami

Przykadowe użycie:

```
<div class="container">
  <div class="row">
    <div class="col-xs-6">
      <div class="thumbnail">
        <img src="avatar.jpg" alt="Sample Image">
        <div class="caption">
          <h3>label</h3><p>description...</p>
        </div>
      </div>
    </div>
    <div class="col-xs-6">
      <div class="thumbnail">
        <img src="avatar.jpg" alt="Sample Image">
          <div class="caption">
            <h3>label</h3><p>description...</p>
          </div>
      </div>
    </div>
  </div>
</div>
```

### Listy <a href="#uzywaniebootstrap-listy" id="uzywaniebootstrap-listy"></a>

Gówne klasy:

* `list-unstyled`: Lista bez listy-stylu a teraz z lewym marginesem.
* `list-inline`: Lista pozioma
* `breadcrumb`: Lista pozioma dla ścieżki nawigacji.
* `dl-horizontal`: Lista z dwóch wyrównanych elementów.
* `list-group`: Panel-lista jak wyświetlacz.

Przykład Breadcrumb:

```
<ul class="breadcrumb">
  <li><a href="#">Home</a></li>
  <li><a href="#">Products</a></li>
  <li class="active">Accessories</li>
</ul>
```

Przykład nagówka i paragrafu:

```
<div class="list-group">
  <a href="#" class="list-group-item">
    <h4 class="list-group-item-heading">What is HTML?</h4>
    <p class="list-group-item-text">HTML stands for HyperText Markup Language. 
      HTML is the main markup     language for describing the structure of Web pages.</p>
  </a>
  <a href="#" class="list-group-item active">
    <h4 class="list-group-item-heading">What is Twitter Bootstrap?</h4>
    <p class="list-group-item-text">Twitter Bootstrap is a powerful front-end framework for faster 
    and easier web development. It is a collection of HTML and CSS based design template.</p>
  </a>
  <a href="#" class="list-group-item">
    <h4 class="list-group-item-heading">What is CSS?</h4>
    <p class="list-group-item-text">CSS stands for Cascading Style Sheet. CSS allows you to specify 
    various style properties for a given HTML element such as colors, backgrounds, fonts etc.</p>
  </a>
</div>
```

### Formy <a href="#uzywaniebootstrap-formy" id="uzywaniebootstrap-formy"></a>

Główna klasa:

* `form-inline` i `form-horizontal` w elemencie `form`.
* `form-group` na div który grupuje `label` i `textarea`. Umożliwia automatyczną regulacje rozstawu.
* `form-control` w `input`, `textarea` i `select` elementy - które normalnie mają szerokosć 100%.

Pojemnik który ma `form-group` klasa zawsze potrzebuje etykiety. Żeby dodać etykietę i wyświetlać ją, musisz użyć klasę `sr-only` .Na przykład:

```
<div class="form-group">
  <label class="sr-only" for="exampleInput">Email address, label not visible</label>
  <input type="email" class="form-control" id="exampleInput" placeholder="Enter email">
</div>
```

Klasy które zmieniają wygląd w zależności od stref zawartości walidacji:

* `has-warning`
* `has-error`
* `has-success`

Klasy, które umożliwiają wyświetlanie ikony w polu tekstowym:

* `glyphicon et form-control-feedback`
* `glyphicon-ok`
* `glyphicon-warning-sign`
* `glyphicon-remove`

Na przykład:

```
<div class="form-group has-warning">
  <label class="control-label" for="input1">Label with warning</label>
  <input type="text" class="form-control" id="input1">
  <span class="glyphicon glyphicon-warning-sign form-control-feedback"></span>
</div>
```

### Przyciski i linki <a href="#uzywaniebootstrap-przyciskiilinki" id="uzywaniebootstrap-przyciskiilinki"></a>

Główne klasy:

* `btn`: Klasa bazowa dla przycisków
* `btn-default`, `btn-primary`, `btn-success`, `btn-info`, `btn-warning`, `btn-danger`, `btn-link`: Aby zmienić wygląd przycisku.
* `btn-lg`, `btn-sm` and `btn-xs`: Aby zmienić rozmiar przycisku.
* `btn-block`: Aby zmienić rozmiar elementu nadrzędnego .
* `active` i `disabled`: zmianę dostępności przycisku&#x20;

```
<span class="button ajax_add_to_cart_button btn btn-default disabled">
  <span>{l s='Add to cart'}</span>
</span>
<a itemprop="url" class="button lnk_view btn btn-default" 
    href="{$product.link|escape:'html':'UTF-8'}" title="{l s='View'}">
  <span>{l s='More'}</span>
</a>
<button type="submit" name="submitMessage" id="submitMessage" 
    class="button btn btn-default button-medium">
  <span>{l s='Send'}<i class="icon-chevron-right right"></i></span>
</button>
```
