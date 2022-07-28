# Theme templates and Smarty

**Table of contents**

* [Theme templates and Smarty](theme-templates-and-smarty.md#ThemetemplatesandSmarty-ThemetemplatesandSmarty)
  * [Basic principles](theme-templates-and-smarty.md#ThemetemplatesandSmarty-Basicprinciples)
    * [Delimiters](theme-templates-and-smarty.md#ThemetemplatesandSmarty-Delimiters)
    * [Comments](theme-templates-and-smarty.md#ThemetemplatesandSmarty-Comments)
    * [Variables](theme-templates-and-smarty.md#ThemetemplatesandSmarty-Variables)
    * [Conditionals](theme-templates-and-smarty.md#ThemetemplatesandSmarty-Conditionals)
    * [Loops](theme-templates-and-smarty.md#ThemetemplatesandSmarty-Loops)
    * [File inclusion](theme-templates-and-smarty.md#ThemetemplatesandSmarty-Fileinclusion)
    * [Debug function](theme-templates-and-smarty.md#ThemetemplatesandSmarty-Debugfunction)
  * [Advanced uses](theme-templates-and-smarty.md#ThemetemplatesandSmarty-Advanceduses)
    * [Captures](theme-templates-and-smarty.md#ThemetemplatesandSmarty-Captures)
    * [Assigning variables](theme-templates-and-smarty.md#ThemetemplatesandSmarty-Assigningvariables)
    * [The $smarty variable](theme-templates-and-smarty.md#ThemetemplatesandSmarty-The$smartyvariable)
    * [Literals](theme-templates-and-smarty.md#ThemetemplatesandSmarty-Literals)
    * [Functions](theme-templates-and-smarty.md#ThemetemplatesandSmarty-Functions)
    * [Plugins](theme-templates-and-smarty.md#ThemetemplatesandSmarty-Plugins)
    * [Smarty Don'ts with PrestaShop](theme-templates-and-smarty.md#smarty-donts-with-prestashop)

## Theme templates and Smarty <a href="#themetemplatesandsmarty-themetemplatesandsmarty" id="themetemplatesandsmarty-themetemplatesandsmarty"></a>

Smarty is a PHP template engine that is sturdy, fast, easy to learn and use, and has a clean and compact design-dedicated syntax. It helps building a much simpler HTML code, and works by compiling then caching each page.

You can learn more by going to its official website: [http://www.smarty.net/](http://www.smarty.net/)

### Basic principles <a href="#themetemplatesandsmarty-basicprinciples" id="themetemplatesandsmarty-basicprinciples"></a>

#### Delimiters <a href="#themetemplatesandsmarty-delimiters" id="themetemplatesandsmarty-delimiters"></a>

Delimiters make it possible for the template engine to "recognize" Smarty calls within a template. The delimiters used by Smarty are curly braces: `{smarty_call}`

If you need to use actual curly braces within your template code, Smarty has special calls for you: `{redelim}` for a left curly brace (`{`), and `{rdelim}` for a right curly brace (`}`).

#### Comments <a href="#themetemplatesandsmarty-comments" id="themetemplatesandsmarty-comments"></a>

As with any scripting or programming language, you can put comments within your template code, and the template engine will not parse them.

Comments use regular delimiters, along with opening and closing `*` characters:

```
{* One-line comment. *}

{* 
Multiple
lines
comment.
*}

{* Comment for Smarty {$code} *}
```

#### Variables <a href="#themetemplatesandsmarty-variables" id="themetemplatesandsmarty-variables"></a>

Just as in PHP, variable are represented by a dollar sign followed by the name of the variable. Putting a variable directly within a Smarty delimiter means that you want to display the variable as-is.\
For instance, `{$foo}` is the Smarty equivalent of PHP's `echo $foo;`.

You can also apply modifiers to your variables:

```
{* Displaying the content of the variable in lowercase. *}
{$foo|lower}
    
{* Displaying the content of the variable after replacing one word with another. *}
{$foo|replace:'bar':'baz'}
    
{* Example of "chaining" modifiers.	 *}
{$foo|lower|capitalize|truncate:10:'...'}
```

You can get a complete list of the available modifiers on the official website: [http://www.smarty.net/docs/en/language.modifiers.tpl](http://www.smarty.net/docs/en/language.modifiers.tpl)

#### Conditionals <a href="#themetemplatesandsmarty-conditionals" id="themetemplatesandsmarty-conditionals"></a>

Smarty has a conditional `if` / `else` / `elseif` system:

```
{if $coffee == 'good'}
  {* Happy coder *}
{elseif $coffee == 'very good'}
  {* Very happy coder *}
{else}
  {* Grumpy coder *}
{/if}
```

You can learn more about the various conditionals on the official website: [http://www.smarty.net/docsv2/en/language.function.if.tpl](http://www.smarty.net/docsv2/en/language.function.if.tpl)

#### Loops <a href="#themetemplatesandsmarty-loops" id="themetemplatesandsmarty-loops"></a>

Smarty supports two loops: `section` and `foreach`. You can use iterators, and even the `foreachelse` conditional:

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

You can learn more on each loop on their respective pages on the official website:

* [http://www.smarty.net/docs/en/language.function.section.tpl](http://www.smarty.net/docs/en/language.function.section.tpl)
* [http://www.smarty.net/docs/en/language.function.foreach.tpl](http://www.smarty.net/docs/en/language.function.foreach.tpl)

#### File inclusion <a href="#themetemplatesandsmarty-fileinclusion" id="themetemplatesandsmarty-fileinclusion"></a>

You can easily include a template file into another using the `include`, `extends` or `block` functions. Thanks to inheritance, file inclusion can impact many templates at a time.

The assignation method takes two mandatory arguments:

* `file`: the name of the template file to include.
* `assign`: the name of the variable that the output of include will be assigned to.

Here are a couple examples:

```
{* Including a file. *}
{include file='steps.tpl'}
   
{* Placing the included content in a variable, then display the variable.	 *}
{include file='text.tpl' assign='MyText'}
{$MyText}
```

Demonstration of inheritance with `extends` and `block`:

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

That last example uses the `block` function, which is designed to define a named area of template source for template inheritance.

You can learn more about template inheritance and each inclusion function on their respective pages on the official website:

* [http://www.smarty.net/docs/en/advanced.features.template.inheritance.tpl](http://www.smarty.net/docs/en/advanced.features.template.inheritance.tpl)
* [http://www.smarty.net/docs/en/language.function.include.tpl](http://www.smarty.net/docs/en/language.function.include.tpl)
* [http://www.smarty.net/docs/en/language.function.extends.tpl](http://www.smarty.net/docs/en/language.function.extends.tpl)
* [http://www.smarty.net/docs/en/plugins.block.functions.tpl](http://www.smarty.net/docs/en/plugins.block.functions.tpl)

#### Debug function <a href="#themetemplatesandsmarty-debugfunction" id="themetemplatesandsmarty-debugfunction"></a>

The complete set of internal processes from a Smarty template can be displayed when the page is displayed.

During theme development, this can be done for each page load by editing the `/config/smarty.config.inc.php` file and editing the `$smarty->debugging` value:

```
$smarty->debugging = true;
```

Once the theme is on a production site, you can enable the debug function by adding the `{DEBUG}` directive in the template file.

You can also manage the debug function directly from PrestaShop: in the "Advanced Parameters" menu, in the "Maintenance" page, change the "Debug console" option to your liking.

You can learn more about the `debug` function on the official website: [http://www.smarty.net/docs/en/language.function.debug.tpl](http://www.smarty.net/docs/en/language.function.debug.tpl)

### Advanced uses <a href="#themetemplatesandsmarty-advanceduses" id="themetemplatesandsmarty-advanceduses"></a>

#### Captures <a href="#themetemplatesandsmarty-captures" id="themetemplatesandsmarty-captures"></a>

The `capture` function makes it possible to retrieve the output of a template without displaying it. For instance: `{capture name="myCapture'} ... {/capture}`\
``

In order to use the content, you must call the `$smarty` super-variable: `$smarty.capture.myCapture`

Do not forget to test for the capture's existence before using it:

`{if $smarty.capture.<name>}` or `{if isset($smarty.capture.<name>}`

The capture function is also able to auto-assign a variable:

```
{capture name='myCapture' assign='myVar'}
   ...
{/capture}
{* Then, in order to use the content, call the $myVar variable. *}
```

You can learn more about the `capture` function on the official website: [http://www.smarty.net/docs/en/language.function.capture.tpl](http://www.smarty.net/docs/en/language.function.capture.tpl)

#### Assigning variables <a href="#themetemplatesandsmarty-assigningvariables" id="themetemplatesandsmarty-assigningvariables"></a>

It is possible to assign a variable into a template file (view), using the `assign` function:

```
{assign var='myVar2' value='My value'}

{* Will display "My value". *}
{$myVar2}
```

You can learn more about the `assign` function on the official website: [http://www.smarty.net/docs/en/language.function.assign.tpl](http://www.smarty.net/docs/en/language.function.assign.tpl)

#### The $smarty variable <a href="#themetemplatesandsmarty-theusdsmartyvariable" id="themetemplatesandsmarty-theusdsmartyvariable"></a>

`$smarty` is a so-called super-variable. It makes it possible to retrieve some useful information:

* `capture` values: `$smarty.capture.myVariable`
* GET values: `{$smarty.get.<name>}`
* POST values: `{$smarty.post.<name>}`
* Current timestamp: `{$smarty.now}`, or with customized formatting `{$smarty.now|date_format:'%d-%m-%Y %H:%M:%S'}`
* PHP constants: `{$smarty.const.<constant name>}`

In Smarty 2, `$smarty` could be used with `foreach`:

When the loop is defined as: `{foreach from=$myarray key="mykey" item="myitem"}`\
...you can perform a `$`[`smarty.foreach.name`](http://smarty.foreach.name)`.property` call

Since PrestaShop 1.5, it is recommended to only rely on the Smarty 3 syntax from PrestaShop themes. Therefore, a `$smarty.foreach.varName.property` call must be replaced by the `$varName@property` equivalent call.

You can learn more about the `$smarty` variable on the official website: [http://www.smarty.net/docs/en/language.variables.smarty.tpl](http://www.smarty.net/docs/en/language.variables.smarty.tpl)

#### Literals <a href="#themetemplatesandsmarty-literals" id="themetemplatesandsmarty-literals"></a>

The `literal` tag makes it possible for a data block to be used as-is, literally, without Smarty trying to interpret it:

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

You can learn more about the literal function on the official website: [http://www.smarty.net/docs/en/language.function.literal.tpl](http://www.smarty.net/docs/en/language.function.literal.tpl)

#### Functions <a href="#themetemplatesandsmarty-functions" id="themetemplatesandsmarty-functions"></a>

Smarty functions do not use the `$` prefix, as do variables: `{debug}`, `{rdelim}`, `{ldelim}`, ...

They can accept arguments: `{include file='<name of the file>'}`

The structure of a function call is thus: `{nameOfTheFunction arg1='...' arg2='...'}`

You cannot use modifiers on functions. For instance, `{nameOfTheFunction arg1='...' |lower}` will not work as expected.

You can learn more about Smarty functions on the official website:

* [http://www.smarty.net/docs/en/language.syntax.functions.tpl](http://www.smarty.net/docs/en/language.syntax.functions.tpl)
* [http://www.smarty.net/docs/en/language.builtin.functions.tpl](http://www.smarty.net/docs/en/language.builtin.functions.tpl)
* [http://www.smarty.net/docs/en/language.custom.functions.tpl](http://www.smarty.net/docs/en/language.custom.functions.tpl)

#### Plugins <a href="#themetemplatesandsmarty-plugins" id="themetemplatesandsmarty-plugins"></a>

Smarty plugins makes it possible to easily extend the standard behavior. They are written in PHP.

For instance, PrestaShop has a Smarty plugin that creates a specific function to handle translatable strings: `{l}`

First, in a theme:

```
{l s='Hello dear viewer'}
```

And in a module (even if overridden!):

```
{l s='Hello dear view' mod='myModule'}
```

You can learn more about Smarty plugins on the official website: [http://www.smarty.net/docs/en/plugins.tpl](http://www.smarty.net/docs/en/plugins.tpl)

#### Smarty Don'ts with PrestaShop

A few things that you should expressly avoid when using Smarty:

* Do not make direct call PrestaShop's constants. Most particularly, do not even use `{$smarty.const._DB_PASSWD_}`, for obvious reasons.
* Do not override PrestaShop's assigned variables.
* Do not make the code needlessly hard to read. For instance, refrain from making `include` calls from within an already included file.
* Do not make direct PHP calls. For instance, do not use `{php} // PHP code {/php}`
