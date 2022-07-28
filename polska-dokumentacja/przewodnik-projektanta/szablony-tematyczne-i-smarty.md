# PSzablony tematyczne i Smarty

**Spis treści**\
****

/\*\<!\[CDATA\[\*/\
div.rbtoc1597140227957 {padding: 0px;}\
div.rbtoc1597140227957 ul {list-style: disc;margin-left: 0px;}\
div.rbtoc1597140227957 li {margin-left: 0px;padding-left: 0px;}\
\
/\*]]>\*/

* [Szablony tematyczne i Smarty](szablony-tematyczne-i-smarty.md#SzablonytematyczneiSmarty-SzablonytematyczneiSmarty)
  * [Podstawowe zasady](szablony-tematyczne-i-smarty.md#SzablonytematyczneiSmarty-Podstawowezasady)
    * [Ograniczniki](szablony-tematyczne-i-smarty.md#SzablonytematyczneiSmarty-Ograniczniki)
    * [Komentarze](szablony-tematyczne-i-smarty.md#SzablonytematyczneiSmarty-Komentarze)
    * [Zmienne](szablony-tematyczne-i-smarty.md#SzablonytematyczneiSmarty-Zmienne)
    * [Tryby warunkowe](szablony-tematyczne-i-smarty.md#SzablonytematyczneiSmarty-Trybywarunkowe)
    * [Pętle](szablony-tematyczne-i-smarty.md#SzablonytematyczneiSmarty-Pętle)
    * [Włączanie pliku](szablony-tematyczne-i-smarty.md#SzablonytematyczneiSmarty-Włączaniepliku)
    * [Funkcja debugowania](szablony-tematyczne-i-smarty.md#SzablonytematyczneiSmarty-Funkcjadebugowania)
  * [Zaawansowane zastosowania](szablony-tematyczne-i-smarty.md#SzablonytematyczneiSmarty-Zaawansowanezastosowania)
    * [Zrzuty](szablony-tematyczne-i-smarty.md#SzablonytematyczneiSmarty-Zrzuty)
    * [Przypisanie zmiennych](szablony-tematyczne-i-smarty.md#SzablonytematyczneiSmarty-Przypisaniezmiennych)
    * [Zmienna $smarty](szablony-tematyczne-i-smarty.md#SzablonytematyczneiSmarty-Zmienna$smarty)
    * [Literówki](szablony-tematyczne-i-smarty.md#SzablonytematyczneiSmarty-Literówki)
    * [Funkcje](szablony-tematyczne-i-smarty.md#SzablonytematyczneiSmarty-Funkcje)
    * [Wtyczki](szablony-tematyczne-i-smarty.md#SzablonytematyczneiSmarty-Wtyczki)
    * [Smarty niemile widziane z PrestaShop](szablony-tematyczne-i-smarty.md#SzablonytematyczneiSmarty-SmartyniemilewidzianezPrestaShop)

## Szablony tematyczne i Smarty <a href="#szablonytematyczneismarty-szablonytematyczneismarty" id="szablonytematyczneismarty-szablonytematyczneismarty"></a>

Smarty jest silnikiem szablonu PHP który jest wytrzymały,szybki, łatwy w nauce i użyciu, i ma czystą i kompaktową składnie do projektowania dedykowanego. Pomaga zbudować znacznie prostszy kod HTML i działa poprzez gromadzenie, a następnie buforowania każdej strony.

Możesz się dowiedzieć więcej wchodząc na oficjalną stronę: [http://www.smarty.net/](http://www.smarty.net/)

### Podstawowe zasady <a href="#szablonytematyczneismarty-podstawowezasady" id="szablonytematyczneismarty-podstawowezasady"></a>

#### Ograniczniki <a href="#szablonytematyczneismarty-ograniczniki" id="szablonytematyczneismarty-ograniczniki"></a>

Ograniczniki umozliwiają silnikowi szablonu "rozpoznać" Smarty zwraca się wewnątrz szablonu. Ograniczniki wykorzystywane przez Smarty są w nawiasach klamrowych The delimiters used by Smarty: `{smarty_call}`

Jeśli trzeba użyć rzeczywistych nawiasów klamrowych w kodzie szablonu Smarty posiada specjalne połączenie dla Ciebie: `{redelim}` na lewej nawias klamrowy (`{`), i `{rdelim}` dla prawej nawias klamrowy (`}`).

#### Komentarze <a href="#szablonytematyczneismarty-komentarze" id="szablonytematyczneismarty-komentarze"></a>

Jak w przypadku każdego języka programowania lub skryptów, można umieścić komentarze w kodzie szablonu, a silnik szablonu nie będzie ich analizowac.&#x20;

Komentarze używają regularnych ograniczników, wraz z otwieraniem i zamykaniem \* znaków.

```
{* One-line comment. *}

{* 
Multiple
lines
comment.
*}

{* Comment for Smarty {$code} *}
```

#### Zmienne <a href="#szablonytematyczneismarty-zmienne" id="szablonytematyczneismarty-zmienne"></a>

Tak jak w PHP, zmienne są reprezentowane przez znak dolara, po którym następuje nazwa zmiennej. Umieszczenie zmiennej bezpośrednio w ograniczniku Smarty oznacza, że chcesz wyświetlić zmienną taką jaka jest.\
Na przykład, `{$foo}` Smarty jest odpowiednikiem PHP `echo $foo;`.

Można również stosować moyfikatory do zmiennych:

```
{* Displaying the content of the variable in lowercase. *}
{$foo|lower}
    
{* Displaying the content of the variable after replacing one word with another. *}
{$foo|replace:'bar':'baz'}
    
{* Example of "chaining" modifiers.	 *}
{$foo|lower|capitalize|truncate:10:'...'}
```

Możesz uzyskać pełną listę dostępnych modyfikatorów na oficjalnej stronie internetowej: [http://www.smarty.net/docs/en/language.modifiers.tpl](http://www.smarty.net/docs/en/language.modifiers.tpl)

#### Tryby warunkowe <a href="#szablonytematyczneismarty-trybywarunkowe" id="szablonytematyczneismarty-trybywarunkowe"></a>

Smarty ma warunkowy system `if` / `else` / `elseif` :

```
{if $coffee == 'good'}
  {* Happy coder *}
{elseif $coffee == 'very good'}
  {* Very happy coder *}
{else}
  {* Grumpy coder *}
{/if}
```

Możesz się dowiedzieć więcej o różnych trybach warunkowych na oficjalnej stronie: [http://www.smarty.net/docsv2/en/language.function.if.tpl](http://www.smarty.net/docsv2/en/language.function.if.tpl)

#### Pętle <a href="#szablonytematyczneismarty-petle" id="szablonytematyczneismarty-petle"></a>

Smarty obsługuje dwie pętle: `section` `i foreach`. Można użyć iteratorów, a nawet trybu warunkowego `foreachelse` :

```
<?php
  $items_list = array( 23 => array('no' => 2456, 'label' => 'Salad'), 96 => array('no' => 4889, 'label' => 'Cream') );
  $smarty->assign('items', $items_list);
?>
<ul>
{foreach from=$items key=myId item=i}
  <li><a href="item.php?id={$myId}">{$i.no}: {$i.label}</li>
{/foreach}
</ul>
```

Możesz dowiedzieć się więcej o każdej pętli na oficjalnych stronach internetowych:

* [http://www.smarty.net/docs/en/language.function.section.tpl](http://www.smarty.net/docs/en/language.function.section.tpl)
* [http://www.smarty.net/docs/en/language.function.foreach.tpl](http://www.smarty.net/docs/en/language.function.foreach.tpl)

#### Włączanie pliku <a href="#szablonytematyczneismarty-wlaczaniepliku" id="szablonytematyczneismarty-wlaczaniepliku"></a>

Można łatwo dołączyć plik szablonu do innego używając funkcji `include`, `extends` or `block`. Dzięki dziedziczeniu, włączenie pliku może mieć wpływ na wiele szablonów naraz.

Metoda przypisania używa dwóch obowiązkowych argumentów:

* `file`: Uwględnia nazwę plikiu szablonu.
* `assign`: Nazwa zmiennej wyjścia zostanie przypisana.

Oto kilka przykładów:

```
{* Including a file. *}
{include file='steps.tpl'}
   
{* Placing the included content in a variable, then display the variable.	 *}
{include file='text.tpl' assign='MyText'}
{$MyText}
```

Demonstracja dziedziczenia z  `extends` i  `block`:

```
{* Filename: parent.tpl *}
<html>
<head>
<title>{block name="title"}Default Title{/block}</title>
...
{block name="title"}New Title{/block}
</head>
</html>

{* Filename: child.tpl *}
{extends file='parent.tpl'}
{block name='title'}New Page Title{/block}
```

Ten ostatni przykład używa funkcji  `block`, który jest przeznaczony do określenia nazwy powierzchni żródła matrycy do matrycy dziedziczenia.

Można się dowiedzieć wiecej na temat dziedziczenia szablonów i każdej funkcji umieszczenia na swojej stronie na oficjalnej stronie:

* [http://www.smarty.net/docs/en/advanced.features.template.inheritance.tpl](http://www.smarty.net/docs/en/advanced.features.template.inheritance.tpl)
* [http://www.smarty.net/docs/en/language.function.include.tpl](http://www.smarty.net/docs/en/language.function.include.tpl)
* [http://www.smarty.net/docs/en/language.function.extends.tpl](http://www.smarty.net/docs/en/language.function.extends.tpl)
* [http://www.smarty.net/docs/en/plugins.block.functions.tpl](http://www.smarty.net/docs/en/plugins.block.functions.tpl)

#### Funkcja debugowania <a href="#szablonytematyczneismarty-funkcjadebugowania" id="szablonytematyczneismarty-funkcjadebugowania"></a>

Kompletny zestaw procesów wewnętrznych z szablonu Smarty mogą być wyświetlane, gdy wyświetlana jest strona.

Podczas rozwoju tematycznego, można to zrobić dla każdego ładowania strony poprzez edycje pliku `/config/smarty.config.inc.php` i edycje `$smarty->debugging` wartości:

```
$smarty->debugging = true;
```

Gdy motyw jest na stronie produkcyjnej, można włączyć funkcje debugowania poprzez dodanie dyrektywy`{DEBUG}` w pliku szablonu.

Można także zarządzać funkcją debugowania bezpośrednio z PrestaShop w menu "Paramenty Zaawansowane" na sronie "Konserwacja" zmień opcje "Konsola Debugownia" do swoich upodobań,

Możesz dowiedzieć się więcej o tej funkcji `debug` na oficjalnej stronie: [http://www.smarty.net/docs/en/language.function.debug.tpl](http://www.smarty.net/docs/en/language.function.debug.tpl)

### Zaawansowane zastosowania <a href="#szablonytematyczneismarty-zaawansowanezastosowania" id="szablonytematyczneismarty-zaawansowanezastosowania"></a>

#### Zrzuty <a href="#szablonytematyczneismarty-zrzuty" id="szablonytematyczneismarty-zrzuty"></a>

Funkcja `capture` umożliwia pobieranie danych wyjściowych szablonu bez wyświetlania go. Na przykład: `{capture name="myCapture'} ... {/capture}`\
``

W celu korzystania z takich materiałów należy przywołać `$smarty` super zmienna: `$smarty.capture.myCapture`

Nie zapomnij sprawdzić chwytu przed użyciem go:

`{if $smarty.capture.<name>}` or `{if isset($smarty.capture.<name>}`

Funkcja przechwytywania ma możliwość automatycznego przypisania zmiennej:

```
{capture name='myCapture' assign='myVar'}
   ...
{/capture}
{* Then, in order to use the content, call the $myVar variable. *}
```

Możesz dowiedzieć się więcej o funkcji `capture` na oficjalnej stronie: [http://www.smarty.net/docs/en/language.function.capture.tpl](http://www.smarty.net/docs/en/language.function.capture.tpl)

#### Przypisanie zmiennych <a href="#szablonytematyczneismarty-przypisaniezmiennych" id="szablonytematyczneismarty-przypisaniezmiennych"></a>

Możliwe jest przypisanie zmiennej do pliku szablonu (widok) używając funkcję  `assign` :

```
{assign var='myVar2' value='My value'}

{* Will display "My value". *}
{$myVar2}
```

Możesz dowiedzieć się więcej o funkcji `assign` na oficjalnej stronie: [http://www.smarty.net/docs/en/language.function.assign.tpl](http://www.smarty.net/docs/en/language.function.assign.tpl)

#### Zmienna $smarty <a href="#szablonytematyczneismarty-zmiennausdsmarty" id="szablonytematyczneismarty-zmiennausdsmarty"></a>

`$smarty` jest to tak zwana super zmienna. To sprawia, że można pobrać kilka przydatnych informacji:

* `capture` wartości: `$smarty.capture.myVariable`
* wartości GET: `{$smarty.get.<name>}`
* wartości POST: `{$smarty.post.<name>}`
* aktualny timestamp: `{$smarty.now}`, lub niestandardowego formatowania `{$smarty.now|date_format:'%d-%m-%Y %H:%M:%S'}`
* stałe PHP: `{$smarty.const.<constant name>}`

w Smarty 2, `$smarty` mogą być stosowane `foreach`:

Gdy pętla jest zdefiniowana jako: `{foreach from=$myarray key="mykey" item="myitem"}`\
...można wykonać wezwanie `$`[`smarty.foreach.name`](http://smarty.foreach.name)`.property`

Od PrestaShop 1.5 zaleca się polegać tylko na składni Smarty 3 z szablonu PrestaShop, W związku z tym `$smarty.foreach.varName.property` wezwanie call musi być zastapiony przez `$varName@property` równoważne wezwanie.

Możesz dowiedzieć więcej o zmiennej `$smarty` na oficjalnej stronie: [http://www.smarty.net/docs/en/language.variables.smarty.tpl](http://www.smarty.net/docs/en/language.variables.smarty.tpl)

#### Literówki <a href="#szablonytematyczneismarty-literowki" id="szablonytematyczneismarty-literowki"></a>

Etykieta `literal` umożliwia blokowi danych do wykorzystanie jej dosłownie, bez Smarty próbuje je interpretować:

```
{literal}
<script type="text/javascript">
  function myFonction()
  {
    ...
  }
</script>
{/literal}
```

Możesz dowiedzieć się więcej na temat funkcji dosłownej na oficjalnej stronie: [http://www.smarty.net/docs/en/language.function.literal.tpl](http://www.smarty.net/docs/en/language.function.literal.tpl)

#### Funkcje <a href="#szablonytematyczneismarty-funkcje" id="szablonytematyczneismarty-funkcje"></a>

Funkcje Smarty nie używa `$` prefix, podobnie jak zmienne: `{debug}`, `{rdelim}`, `{ldelim}`, ...

Mogą one zaakceptować argumenty: `{include file='<name of the file>'}`

Struktura wywołania funkcji jest więc: `{nameOfTheFunction arg1='...' arg2='...'}`

Nie można użyć modyfikatorów na funkcjach, na przykład `{nameOfTheFunction arg1='...' |lower}` nie będzie działać zgodnie z oczekiwaniami. .

Możesz dowiedzieć sie więcej o funkcjach Smarty na oficjalnej stronie:

* [http://www.smarty.net/docs/en/language.syntax.functions.tpl](http://www.smarty.net/docs/en/language.syntax.functions.tpl)
* [http://www.smarty.net/docs/en/language.builtin.functions.tpl](http://www.smarty.net/docs/en/language.builtin.functions.tpl)
* [http://www.smarty.net/docs/en/language.custom.functions.tpl](http://www.smarty.net/docs/en/language.custom.functions.tpl)

#### Wtyczki <a href="#szablonytematyczneismarty-wtyczki" id="szablonytematyczneismarty-wtyczki"></a>

Wtyczki Smarty umożliwia łatwe rozszerzenie standardowego zachowania. Są one zapisane w PHP. Na przykład, PrestaShop ma wtyczki Smarty, które tworzą specyficzną funkcje obsługiwania tłumaczeń: `{l}`

Po pierwsze w temacie:

```
{l s='Hello dear viewer'}
```

i w module (nawet jeśli jest nadpisany!) And in a module (even if overridden!):

```
{l s='Hello dear view' mod='myModule'}
```

Możesz dowiedzieć się więcej o wtyczkach Smarty na oficjalnej stronie: [http://www.smarty.net/docs/en/plugins.tpl](http://www.smarty.net/docs/en/plugins.tpl)

#### Smarty niemile widziane z PrestaShop <a href="#szablonytematyczneismarty-smartyniemilewidzianezprestashop" id="szablonytematyczneismarty-smartyniemilewidzianezprestashop"></a>

Kilka rzeczy które trzeba wyraźnie unikać przy użyciu Smarty:

* Nie rób stałego bezpośredniego połączenia PrestaShop. Bardziej szczegółowo nawet nie używaj `{$smarty.const._DB_PASSWD_}`, z oczywistych powodów..
* Nie zastępuj przypisanych zmiennych PrestaShop.
* Nie twórz niepotrzebnie kodu trudnego do odczytania. Na przykład powstrzymując się od jakichkolwiek zawołań  `include` od dołączonego już od wewnątrz pliku.
* Nie rób bezpośredniego połączenia PHP. Na przykład nie należy używać `{php} // PHP code {/php}`
