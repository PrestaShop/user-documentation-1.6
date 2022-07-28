# Korzystanie z jQuery i Ajax

**Spis treści**\
****

/\*\<!\[CDATA\[\*/\
div.rbtoc1597140227994 {padding: 0px;}\
div.rbtoc1597140227994 ul {list-style: disc;margin-left: 0px;}\
div.rbtoc1597140227994 li {margin-left: 0px;padding-left: 0px;}\
\
/\*]]>\*/

* [Korzystanie jQuery and Ajax](korzystanie-z-jquery-i-ajax.md#KorzystaniezjQueryiAjax-KorzystaniejQueryandAjax)
  * [O jQuery](korzystanie-z-jquery-i-ajax.md#KorzystaniezjQueryiAjax-OjQuery)
    * [jQuery $](korzystanie-z-jquery-i-ajax.md#KorzystaniezjQueryiAjax-jQuery$)
    * [Funkcje w jQuery](korzystanie-z-jquery-i-ajax.md#KorzystaniezjQueryiAjax-FunkcjewjQuery)
    * [Selektory](korzystanie-z-jquery-i-ajax.md#KorzystaniezjQueryiAjax-Selektory)
    * [Metody i wywołania zwrotne](korzystanie-z-jquery-i-ajax.md#KorzystaniezjQueryiAjax-Metodyiwywołaniazwrotne)
    * [Dostępne wtyczki w PrestaShop ](korzystanie-z-jquery-i-ajax.md#KorzystaniezjQueryiAjax-DostępnewtyczkiwPrestaShop)
    * [Kilka innych narzędzi](korzystanie-z-jquery-i-ajax.md#KorzystaniezjQueryiAjax-Kilkainnychnarzędzi)
  * [Wykonywanie połączeń Ajax z jQuery](korzystanie-z-jquery-i-ajax.md#KorzystaniezjQueryiAjax-WykonywaniepołączeńAjaxzjQuery)
    * [O Ajax](korzystanie-z-jquery-i-ajax.md#KorzystaniezjQueryiAjax-OAjax)
    * [Metody jQuery's Ajax ](korzystanie-z-jquery-i-ajax.md#KorzystaniezjQueryiAjax-MetodyjQuery%27sAjax)

## Korzystanie jQuery and Ajax <a href="#korzystaniezjqueryiajax-korzystaniejqueryandajax" id="korzystaniezjqueryiajax-korzystaniejqueryandajax"></a>

### O jQuery <a href="#korzystaniezjqueryiajax-ojquery" id="korzystaniezjqueryiajax-ojquery"></a>

jQuery jest solidną biblioteką JavaScript. Wśród wielu zalet:

* Działa zgodnie z oczekiwaniami wielu przeglądarek internetowych.
* Jasna, zwięzła i intuicyjna architektura
* Wiele dostępnych wtyczek.

Możesz się dowiedzieć więcej o jQuery na oficjalnej stronie: [http://jquery.com/](http://jquery.com/)

#### jQuery $ <a href="#korzystaniezjqueryiajax-jqueryusd" id="korzystaniezjqueryiajax-jqueryusd"></a>

jQuery posiada funkcje `$()`, nazw, który zawierają wszystkie inne funkcje.

Funkcja `$()` może być użyta na wiele sposobów:

* Przy zastosowaniu funkcji jako parametr, `$()` będzie wykonywał funkcje gdy strony w DOM są w pełni załadowane.\
  Na przykład: `$(function(){ /* do something */ });`
* Po przejściu ciągu zawierającego selektor CSS `$()`zwróci wszystkie węzły HTML, które odpowiadają selektorowi.\
  Na przykład: `$('ul#nav');`
* Ten zestaw węzłów może być przypisany do każdej z metod jQuery. Na przykład. Jeśli chcesz ukryć elementy nawigacji zwracane przez powyższy selektor.\
  Na przykład: `$('ul#nav').slideUp('fast');`
* Przy użyciu czystego kodu HTML jako jego parametru `$()` stworzy węzeł (element DOM). Ten węzeł może znowu być stosowany z dowolną metodą jQuery\
  Na przykład: `$("<li>Sign Off</li>").appendTo("ul#nav");`

`$()`jest jedynie skrótem specyficznej biblioteki funkcji `jQuery()`. Istnieje w celu przyspieszenia kodowania. Wiele innych bibliotek JavaScript używa `$()` ich skrótów.

W związku z tym te dwie linie są równoważne:

```
$('ul#nav').slideUp('fast'); 
jQuery('ul#nav').slideUp('fast');
```

Jeśli mieszasz biblioteki JavaScript w swoim temacie, może będzie lepiej powiedzieć jQuery żeby uwolnić `$()`. Prosty zwrot `$.noConflict()`, i od tej pory każde wywołanie `jQuery()`będzie wymagać korzystania z `$()`.

Możesz dowiedzieć się więcej na temat `jQuery()` i `$()` na oficjalnej stronie: [http://api.jquery.com/jQuery/](http://api.jquery.com/jQuery/)

#### Funkcje w jQuery <a href="#korzystaniezjqueryiajax-funkcjewjquery" id="korzystaniezjqueryiajax-funkcjewjquery"></a>

jQuery's namespace `$` zawiera wszystkie funkcje, które nie są dołączane do konkretnego węzła.

Wśród nich znajduje się kilka funkcji Ajax I funkcji użytkowych. Na przykład:

```
$.post('/handler.php', {'action': 'purchase', 'product': 434}, function(data){/* do something */} );
```

Można dołaczyć zdarzenia do zbioru skróconych węzłów zwróconych przez `$()`. Jedną z zalet korzystania z jQuery, po raz kolejny jest to, że podczas obsługi zdarzenia, pomaga on poprzez harmonizacje, tak, że nie trzeba uzględniać specyfiki każdej przeglądarki.

Aby przypisać funkcje click event, jest prosty dodatek `.click(function)`.\
W celu wygenerowania click event, można również użyć `.click()` z każdym parametrem. Na przykład: `$('#button').click(function(){/* do something */});`

Możesz się dowiedzieć więcej na temat jQuery's Ajax i funkcji użytkowych na oficjalnej stronie:

* [http://api.jquery.com/category/ajax/](http://api.jquery.com/category/ajax/) (na przykład, [http://api.jquery.com/jQuery.post/](http://api.jquery.com/jQuery.post/))
* [http://api.jquery.com/category/utilities/](http://api.jquery.com/category/utilities/)

#### Selektory <a href="#korzystaniezjqueryiajax-selektory" id="korzystaniezjqueryiajax-selektory"></a>

jQuery oferuje dwa spososby, aby wybrać elementy strony:

* Połącz selektory CSS i XPath w ciągu znaków, które są używane z funkcją `$()`. Na przykład: `$("div > ul a")`
* Użyj jednej z kilku metod, które są już dostępne w `jQuery` namespace.

Oba te spososby mogą być łączone

```
var my_jQuery_object = $("#my_image");
var my_jQuery_object = $("#menu a");
var my_jQuery_object = $("#id > .classe, #id td:last-child"); 
    
/* returns the 'td' elements within the odd 'tr'. */
var my_jQuery_object = $('tr:odd td');
    
/* returns the fourth paragraph. */
var my_jQuery_object = $("p:eq(4)");
    
/* returns the 7 first paragraphs. */
var my_jQuery_object = $("p:lt(8)");
```

Możesz dowiedzieć się więcej na temat selektorów jQuery's na oficjalnej stronie: [http://api.jquery.com/category/selectors/](http://api.jquery.com/category/selectors/)

#### Metody i wywołania zwrotne <a href="#korzystaniezjqueryiajax-metodyiwywolaniazwrotne" id="korzystaniezjqueryiajax-metodyiwywolaniazwrotne"></a>

Cały zestaw metod dostępny w standardowym API to: manipulacja DOM, manipulacja CSS, event managment, efekty wizualne, etc.

Na przykład jeśli chcesz, aby znikneły powoli wszystkie akapity na stronie, użyj tego:

```
$("p").fadeOut();
```

Niektóre metody (takie jak `fadeOut()`) przyjmują inną metodę jako parametr. Taki sposób wykonany raz jest już zrobiony. To nazywamy wywołaniem zwrotnym&#x20;

Na przykład:

```
$(".test").fadeOut("slow",function(){ 
  $(this).fadeIn("slow"); 
});
```

Wszystkie metody powrotu przedmiotu  `jQuery` . To sprawia, że metody łańcucha są bez ograniczeń. Można nawet napisać swój kod, tak, że jest on czytany jak blok funkcyjny.

Na przykład, ten kod działa doskonale i łatwy do odczytu i aktualizacji:

```
$(".emptyContent").append("This is a test")
  .css("border", "1px solid red")
  .addClass("fullContent")
  .removeClass("emptyContent");
```

#### Dostępne wtyczki w PrestaShop  <a href="#korzystaniezjqueryiajax-dostepnewtyczkiwprestashop" id="korzystaniezjqueryiajax-dostepnewtyczkiwprestashop"></a>

To jest lista wtyczek jQuery które są dostępne w domyślnej instalacji PrestaShop:

| Nazwa wtyczki              | Opis wtyczki                                                                                          |
| -------------------------- | ----------------------------------------------------------------------------------------------------- |
| jquery.colorpicker         | Selektor stylu kolorów PrestaShop.                                                                    |
| jquery.cookie-plugin       | Odczytuje, zapisuje i usuwa pliki cookie.                                                             |
| jquery.dimensions          | Zarządza elementami wymiarów.                                                                         |
| jquery.easing              | Zarządza prędkością elementów.                                                                        |
| jquery.excanvas            | Zmienia obszar elementu roboczego (zaokrąglone narożniki/gradienty/krycia/rysowanie lini, łuku itp.). |
| jquery.fieldselection      | Wykorzystuje i zastępuje tekst w wybranej strefie.                                                    |
| jquery.flip                | Odwraca element.                                                                                      |
| jquery.flot                | Tworzy wykres prezentacji danych, takich jak krzywe, bary, itp.                                       |
| jquery.highlight           | Dodaje składnie koloryzacji.                                                                          |
| jquery.hoverIntent         | Dodaje efekt przewidywania na JavaScript hover event.                                                 |
| jquery.idTabs              | Zarządza kartami.                                                                                     |
| jquery.ifxtransfer         | Animuje elementem podczas przenoszenia z jednego pojemnika do drugiego.                               |
| jquery.jqminmax            | Dodaje min-width, max-width, min-height i max-height na wszystkich przeglądarkach.                    |
| jquery.pngFix              | Zarządza przejrzystością w IE 5.5 i IE 6.                                                             |
| jquery.scrollTo            | Dodaje strony lub przewijanie elementu do określonej pozycji.                                         |
| jquery.serialScroll        | Wprowadza szereg.elementów przewijania do określonej pozycji.                                         |
| jquery.tablednd            | Przeciąga i upuszcza wiersze tabeli.                                                                  |
| jquery.typewatch           | Wykonuje funkcje kiedy użytkownik wpisał jakiś tekst w strefie i przestał pisać po pewnym czasie.     |
| jquery.validate-creditcard | Weryfikuje numer karty kredytowej w zależności od jego typu.                                          |

#### Kilka innych narzędzi <a href="#korzystaniezjqueryiajax-kilkainnychnarzedzi" id="korzystaniezjqueryiajax-kilkainnychnarzedzi"></a>

jQuery's API jest bardzo kompletne, i spędzisz godziny na poszukiwaniu nowych możliwości.

Oto kilka funkcji, które mogą być niezwykle użyteczne podczas tworzenia tematu.&#x20;

Po pierwsze, `each()`, co umożliwia petli przejście przez liste elementów:

```
$("img").each(function(){ console.log($(this).attr("src")); });
```

Po drugie, `browser`, jest obiektem, który pozwala dowiedzieć się, która przeglądarka pracuje z:

```
if($.browser.msie) {
  if($.browser.version == 6) {
    // Your IE6 specific code.
  } else {
    // Code for any other IE browser.
  }
}
```

### Wykonywanie połączeń Ajax z jQuery <a href="#korzystaniezjqueryiajax-wykonywaniepolaczenajaxzjquery" id="korzystaniezjqueryiajax-wykonywaniepolaczenajaxzjquery"></a>

#### O Ajax <a href="#korzystaniezjqueryiajax-oajax" id="korzystaniezjqueryiajax-oajax"></a>

Termin "Ajax" jest naprawdę skrótem od Asynchronous JavaScript i XML. Opisuje użycie JavaScript  do załadowania nowej zawartości do bieżącej strony bez konieczności przeładowania całęj. Proces ten nazywany jest ansynchronicznym, ponieważ gdy żadanie Ajax zostało wysłane do serwera webowego, przeglądarka nie musi czekać na odpowiedź w celu wykonania innych zadań. Przesyłana treść nie musi być sformatowana w XML, można użyć JSON, HTML, lub zwykły tekst.

W efekcie użycie Ajax sprawia, że mozliwe jest zbudowanie bardzo dynamicznych stron internetowych&#x20;

Możesz się dowiedzieć więcej na temat techniki Ajax na nastepującej stronie:&#x20;

* Wikipedia: [https://pl.wikipedia.org/wiki/AJAX](https://pl.wikipedia.org/wiki/AJAX)
* Mozilla Developer Network: [https://developer.mozilla.org/en/docs/AJAX](https://developer.mozilla.org/en/docs/AJAX)

About JSON

&#x20;JavaScript Object Notation jest najczęściej stosowanym formatem podczas przesyłania danych przy użyciu techniki Ajax, z dwóch głównych powodów, uważa sie, że jest lżejszy niż XML, a to może być bardzo ątwe wykorzystane przez JavaScript gdyż przypomina podzbiór tego języka. Możesz dowiedzieć się więcej o JSON na następujących stronach.

* [http://json.org/](http://json.org/json-fr.html)
* [https://pl.wikipedia.org/wiki/JSON](https://pl.wikipedia.org/wiki/JSON)
* [https://developer.mozilla.org/en-US/docs/JSON](https://developer.mozilla.org/en-US/docs/JSON).

**Jak użyć Ajax w PrestaShop**&#x20;

Domyśłne kontrolery PrestaShop uzywają standardowej pełnej strony- procesu przeładowania.

Jeśli PrestaShop wykryje parametr "ajax" w GET albo POST zapytania, kontroler `ajax` obiektu jest przełączony na true: `$this->ajax = true;`.

Na przykład, Jeśli kod wyzwala URL, takie jak : `http://...`**`&ajax`**`&action=updatelist`\
...regulator następnie wykona `displayAjaxUpdateList()` jeśli metoda istnieje. Jeśli nie istnieje, to wykona  `displayAjax()` metodą (domyślną).

Dlatego on musi zawierać kod który weźmie pod uwagę wezwanie Ajax. Oto jak można napisać prostą kwerendę za pomocą Ajax jQuery:

```
var query = $.ajax({
  type: 'POST',
  url: baseDir + 'modules/mymodule/ajax.php',
  data: 'method=myMethod&id_data=' + $('#id_data').val(),
  dataType: 'json',
  success: function(json) {
    // ....
  }
});
```

Oto jak skrypt  `ajax.php` będzie działać:

```
// Located in /modules/mymodule/ajax.php
require_once(dirname(__FILE__).'../../../config/config.inc.php');
require_once(dirname(__FILE__).'../../../init.php');
switch (Tools::getValue('method')) {
  case 'myMethod' :
    die( Tools::jsonEncode( array('result'=>'my_value'));
    break;
  default:
    exit;
}
exit;
```

Jak widzisz w przykładzie powyższy kod, PrestaShop  `Tools` zawiera obiekt  `jsonEncode()`, to metoda, która sprawia, że łatwo przekształcić tablicę PHP do obiektu JSON:

```
public function displayAjax() {
  $return = array(
    'hasError' => true,
    'errors' => 'Ceci est le message'
  );
  die(Tools::jsonEncode($return));
}
```

#### Metody jQuery's Ajax  <a href="#korzystaniezjqueryiajax-metodyjquerysajax" id="korzystaniezjqueryiajax-metodyjquerysajax"></a>

**jQuery.ajax(url \[, ustawienia ] )**

Parametry:

* url: URL do której należy wysłać zapytanie
* ustwienia: opcje i funkcje

Niektóre opcje:

`async` (boolean): domyslną jest true

* `type`: domyślnym jest 'GET'
* `cache` (logiczna): domyślną jest true
* `data`: GET tablica wysyłana do serwera
* `dataType`: zarówno `xml`, `json`, `script` albo `html`

Niektóre funkcje:

* `beforeSend`: wyzwalane przed wywołaniem Ajax
* `error`: w przypadku błędu
* `success`: w przypadku powodzenia
* `timeout`: w przypadku przekroczenia czasu&#x20;
* `complete`: wyzwalane po sukcesie zawołania, bez względu na wynik.

Możesz się dowiedzieć więcej o  `ajax()`tutaj: [http://api.jquery.com/jQuery.ajax/](http://api.jquery.com/jQuery.ajax/)

**Alternatywny: jQuery.load(url \[, data ] \[, complete(responseText, textStatus, XMLHttpRequest) ] )**

Metoda ta stosowana jest do bezpośredniego załadowania wyniku HTML do wywołania Ajax, w obrębie elemenetu na bieżącej stronie.&#x20;

Na przykład :

```
$('#result').load('ajax/test.html', function() {
  alert('Load was performed.');
});
```

**Alternatywny: jQuery.get( url \[, data ] \[, success(data, textStatus, jqXHR) ] \[, dataType ] )**

Metoda ta pozwala na połączenie się z zapytaniem Ajax ze skryptem HTTP GET. Jest to równoznaczne z następującym połączeniem Ajax: &#x20;

```
$.ajax({
  url: url,
  data: data,
  success: success,
  dataType: dataType
});
```

**Wartości zwracane na wywołanie Ajax jQuery**&#x20;

Wszystkie te metody jQuery zwracają obiekt  `jqHXR,` który jest przedłużeniem obiektu  `XMLHTTPRequest.` Obiekt ten umożliwia wywołanie różnych funkcji w zależności od wyniku połączenia:

* Powodzenie: `jqXHR.done(function(data, textStatus, jqXHR) {});`
* Błąd: `jqXHR.fail(function(jqXHR, textStatus, errorThrown) {});`
* Powodzenie albo Błąd: `jqXHR.always(function(data|jqXHR, textStatus, jqXHR|errorThrown){ });`
* Powodzenie i Błąd: `jqXHR.then(function(data, textStatus, jqXHR) {}, function(jqXHR, textStatus, errorThrown) {});`

Oto przykład z połaczenia funkcji w zależności od wyniku kwerendy:

```
// Assign handlers immediately after making the request,
// and remember the jqxhr object for this request
var jqxhr = $.get("example.php", function() {
  alert("success");
})
.done(function() { alert("second success"); })
.fail(function() { alert("error"); })
.always(function() { alert("finished"); });

// perform other work here ...
// Set another completion function for the request above
jqxhr.always(function(){ alert("second finished"); });
```
