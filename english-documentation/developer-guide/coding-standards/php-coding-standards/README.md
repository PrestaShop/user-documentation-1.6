# PHP Coding Standards

**Table of contents**

* PHP Coding Standards
  * [Introduction](./#PHPCodingStandards-Introduction)
  * [PSR-1 - Basic Coding Standard](./#PHPCodingStandards-PSR-1-BasicCodingStandard)
  * [PSR-2 - Coding Style Guide](./#PHPCodingStandards-PSR-2-CodingStyleGuide)

The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD", "SHOULD NOT", "RECOMMENDED", "MAY", and "OPTIONAL" in this document are to be interpreted as described in [RFC 2119](http://www.ietf.org/rfc/rfc2119.txt).

## Introduction <a href="#phpcodingstandards-introduction" id="phpcodingstandards-introduction"></a>

As you already know if you have read [this article](http://build.prestashop.com/news/prestashop-1-7-and-symfony/), we chose to integrate the Symfony framework into PrestaShop. So, what’s more natural than to follow their coding standards? It comes as a complement of the PSR standards ([PSR-0](http://www.php-fig.org/psr/psr-0/), [PSR-1](http://www.php-fig.org/psr/psr-1/), [PSR-2](http://www.php-fig.org/psr/psr-2/) and [PSR-4](http://www.php-fig.org/psr/psr-4/)).

Some noteworthy rules:

* Use camelCase, not\_underscores, for variable names, function names, method names, and arguments names.
* ![](http://build.prestashop.com/assets/images/2016/05/yoda.gif)[Yoda conditions](https://en.wikipedia.org/wiki/Yoda\_conditions) you should use.
* Add a comma after each array item in a multi-line array, even after the last one.

```
$defaultOptions = array(
    'some_default' => 'values',
    'another_default' => 'more values',
);

if (true === isset($defaultOptions['some_default'])) {
    return;
}
```

More details and a complete example can be found on [Symfony documentation](http://symfony.com/doc/current/contributing/code/standards.html).

## PSR-1 - Basic Coding Standard <a href="#phpcodingstandards-psr-1-basiccodingstandard" id="phpcodingstandards-psr-1-basiccodingstandard"></a>

### 1. Overview <a href="#phpcodingstandards-1.overview" id="phpcodingstandards-1.overview"></a>

* Files MUST use only `<?php` and `<?=` tags.
* Files MUST use only UTF-8 without BOM for PHP code.
* Files SHOULD _either_ declare symbols (classes, functions, constants, etc.) _or_ cause side-effects (e.g. generate output, change .ini settings, etc.) but SHOULD NOT do both.
* Namespaces and classes MUST follow an "autoloading" PSR: \[[PSR-0](https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-0.md), [PSR-4](https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-4-autoloader.md)].
* Class names MUST be declared in `StudlyCaps`.
* Class constants MUST be declared in all upper case with underscore separators.
* Method names MUST be declared in `camelCase`.

### 2. Files <a href="#phpcodingstandards-2.files" id="phpcodingstandards-2.files"></a>

#### 2.1. PHP Tags <a href="#phpcodingstandards-2.1.phptags" id="phpcodingstandards-2.1.phptags"></a>

PHP code MUST use the long `<?php ?>` tags or the short-echo `<?= ?>` tags; it MUST NOT use the other tag variations.

#### 2.2. Character Encoding <a href="#phpcodingstandards-2.2.characterencoding" id="phpcodingstandards-2.2.characterencoding"></a>

PHP code MUST use only UTF-8 without BOM.

#### 2.3. Side Effects <a href="#phpcodingstandards-2.3.sideeffects" id="phpcodingstandards-2.3.sideeffects"></a>

A file SHOULD declare new symbols (classes, functions, constants, etc.) and cause no other side effects, or it SHOULD execute logic with side effects, but SHOULD NOT do both.

The phrase "side effects" means execution of logic not directly related to declaring classes, functions, constants, etc., _merely from including the file_.

"Side effects" include but are not limited to: generating output, explicit use of `require` or `include`, connecting to external services, modifying ini settings, emitting errors or exceptions, modifying global or static variables, reading from or writing to a file, and so on.

The following is an example of a file with both declarations and side effects; i.e, an example of what to avoid:

```
<?php 
// side effect: change ini settings
ini_set('error_reporting', E_ALL);
 
// side effect: loads a file
include "file.php";
 
// side effect: generates output
echo "<html>\n";
 
// declaration
function foo()
{
    // function body
}
```

The following example is of a file that contains declarations without side effects; i.e., an example of what to emulate:

```
<?php 
// declaration
function foo()
{
    // function body
}
 
// conditional declaration is *not* a side effect
if (! function_exists('bar')) {
    function bar()
    {
        // function body
    }
}
```

### 3. Namespace and Class Names <a href="#phpcodingstandards-3.namespaceandclassnames" id="phpcodingstandards-3.namespaceandclassnames"></a>

Namespaces and classes MUST follow an "autoloading" PSR: \[[PSR-0](https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-0.md), [PSR-4](https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-4-autoloader.md)].

This means each class is in a file by itself, and is in a namespace of at least one level: a top-level vendor name.

Class names MUST be declared in `StudlyCaps`.

Code written for PHP 5.3 and after MUST use formal namespaces.

For example:

```
<?php 
// PHP 5.3 and later:
namespace Vendor\Model;
 
class Foo
{
}
```

Code written for 5.2.x and before SHOULD use the pseudo-namespacing convention of `Vendor_` prefixes on class names.

```
<?php 
// PHP 5.2.x and earlier:
class Vendor_Model_Foo
{
}
```

### 4. Class Constants, Properties, and Methods <a href="#phpcodingstandards-4.classconstants-properties-andmethods" id="phpcodingstandards-4.classconstants-properties-andmethods"></a>

The term "class" refers to all classes, interfaces, and traits.

#### 4.1. Constants <a href="#phpcodingstandards-4.1.constants" id="phpcodingstandards-4.1.constants"></a>

Class constants MUST be declared in all upper case with underscore separators. For example:

```
<?php 
namespace Vendor\Model;
 
class Foo
{
    const VERSION = '1.0';
    const DATE_APPROVED = '2012-06-01';
}
```

#### 4.2. Properties <a href="#phpcodingstandards-4.2.properties" id="phpcodingstandards-4.2.properties"></a>

This guide intentionally avoids any recommendation regarding the use of `$StudlyCaps`, `$camelCase`, or `$under_score` property names.

Whatever naming convention is used SHOULD be applied consistently within a reasonable scope. That scope may be vendor-level, package-level, class-level, or method-level.

#### 4.3. Methods <a href="#phpcodingstandards-4.3.methods" id="phpcodingstandards-4.3.methods"></a>

Method names MUST be declared in `camelCase()`.

## PSR-2 - Coding Style Guide <a href="#phpcodingstandards-psr-2-codingstyleguide" id="phpcodingstandards-psr-2-codingstyleguide"></a>

### 1. Overview <a href="#phpcodingstandards-1.overview.1" id="phpcodingstandards-1.overview.1"></a>

* Code MUST follow a "coding style guide" PSR \[[PSR-1](https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-1-basic-coding-standard.md)].
* Code MUST use 4 spaces for indenting, not tabs.
* There MUST NOT be a hard limit on line length; the soft limit MUST be 120 characters; lines SHOULD be 80 characters or less.
* There MUST be one blank line after the `namespace` declaration, and there MUST be one blank line after the block of `use` declarations.
* Opening braces for classes MUST go on the next line, and closing braces MUST go on the next line after the body.
* Opening braces for methods MUST go on the next line, and closing braces MUST go on the next line after the body.
* Visibility MUST be declared on all properties and methods; `abstract` and `final` MUST be declared before the visibility; `static` MUST be declared after the visibility.
* Control structure keywords MUST have one space after them; method and function calls MUST NOT.
* Opening braces for control structures MUST go on the same line, and closing braces MUST go on the next line after the body.
* Opening parentheses for control structures MUST NOT have a space after them, and closing parentheses for control structures MUST NOT have a space before.

#### 1.1. Example <a href="#phpcodingstandards-1.1.example" id="phpcodingstandards-1.1.example"></a>

This example encompasses some of the rules below as a quick overview:

```
<?php 
namespace Vendor\Package;
 
use FooInterface;
use BarClass as Bar;
use OtherVendor\OtherPackage\BazClass;
 
class Foo extends Bar implements FooInterface
{
    public function sampleFunction($a, $b = null)
    {
        if ($a === $b) {
            bar();
        } elseif ($a > $b) {
            $foo->bar($arg1);
        } else {
            BazClass::bar($arg2, $arg3);
        }
    }
 
    final public static function bar()
    {
        // method body
    }
}
```

### 2. General <a href="#phpcodingstandards-2.general" id="phpcodingstandards-2.general"></a>

#### 2.1 Basic Coding Standard <a href="#phpcodingstandards-2.1basiccodingstandard" id="phpcodingstandards-2.1basiccodingstandard"></a>

Code MUST follow all rules outlined in [PSR-1](https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-1-basic-coding-standard.md).

#### 2.2 Files <a href="#phpcodingstandards-2.2files" id="phpcodingstandards-2.2files"></a>

All PHP files MUST use the Unix LF (linefeed) line ending.

All PHP files MUST end with a single blank line.

The closing `?>` tag MUST be omitted from files containing only PHP.

#### 2.3. Lines <a href="#phpcodingstandards-2.3.lines" id="phpcodingstandards-2.3.lines"></a>

There MUST NOT be a hard limit on line length.

The soft limit on line length MUST be 120 characters; automated style checkers MUST warn but MUST NOT error at the soft limit.

Lines SHOULD NOT be longer than 80 characters; lines longer than that SHOULD be split into multiple subsequent lines of no more than 80 characters each.

There MUST NOT be trailing whitespace at the end of non-blank lines.

Blank lines MAY be added to improve readability and to indicate related blocks of code.

There MUST NOT be more than one statement per line.

#### 2.4. Indenting <a href="#phpcodingstandards-2.4.indenting" id="phpcodingstandards-2.4.indenting"></a>

Code MUST use an indent of 4 spaces, and MUST NOT use tabs for indenting.

Using only spaces, and not mixing spaces with tabs, helps to avoid problems with diffs, patches, history, and annotations. The use of spaces also makes it easy to insert fine-grained sub-indentation for inter-line alignment.

#### 2.5. Keywords and True/False/Null <a href="#phpcodingstandards-2.5.keywordsandtrue-false-null" id="phpcodingstandards-2.5.keywordsandtrue-false-null"></a>

PHP [keywords](http://php.net/manual/en/reserved.keywords.php) MUST be in lower case.

The PHP constants `true`, `false`, and `null` MUST be in lower case.

### 3. Namespace and Use Declarations <a href="#phpcodingstandards-3.namespaceandusedeclarations" id="phpcodingstandards-3.namespaceandusedeclarations"></a>

When present, there MUST be one blank line after the `namespace` declaration.

When present, all `use` declarations MUST go after the `namespace` declaration.

There MUST be one `use` keyword per declaration.

There MUST be one blank line after the `use` block.

For example:  \


```
<?php 
namespace Vendor\Package;
 
use FooClass;
use BarClass as Bar;
use OtherVendor\OtherPackage\BazClass;
 
// ... additional PHP code ...
```

### 4. Classes, Properties, and Methods <a href="#phpcodingstandards-4.classes-properties-andmethods" id="phpcodingstandards-4.classes-properties-andmethods"></a>

The term "class" refers to all classes, interfaces, and traits.

#### 4.1. Extends and Implements <a href="#phpcodingstandards-4.1.extendsandimplements" id="phpcodingstandards-4.1.extendsandimplements"></a>

The `extends` and `implements` keywords MUST be declared on the same line as the class name.

The opening brace for the class MUST go on its own line; the closing brace for the class MUST go on the next line after the body.

```
<?php 
namespace Vendor\Package;
 
use FooClass;
use BarClass as Bar;
use OtherVendor\OtherPackage\BazClass;
 
class ClassName extends ParentClass implements \ArrayAccess, \Countable
{
    // constants, properties, methods
}
```

Lists of `implements` MAY be split across multiple lines, where each subsequent line is indented once. When doing so, the first item in the list MUST be on the next line, and there MUST be only one interface per line.

```
<?php 
namespace Vendor\Package;
 
use FooClass;
use BarClass as Bar;
use OtherVendor\OtherPackage\BazClass;
 
class ClassName extends ParentClass implements
    \ArrayAccess,
    \Countable,
    \Serializable
{
    // constants, properties, methods
}
```

#### 4.2. Properties <a href="#phpcodingstandards-4.2.properties.1" id="phpcodingstandards-4.2.properties.1"></a>

Visibility MUST be declared on all properties.

The `var` keyword MUST NOT be used to declare a property.

There MUST NOT be more than one property declared per statement.

Property names SHOULD NOT be prefixed with a single underscore to indicate protected or private visibility.

A property declaration looks like the following.

```
<?php 
namespace Vendor\Package;
 
class ClassName
{
    public $foo = null;
}
```

#### 4.3. Methods <a href="#phpcodingstandards-4.3.methods.1" id="phpcodingstandards-4.3.methods.1"></a>

Visibility MUST be declared on all methods.

Method names SHOULD NOT be prefixed with a single underscore to indicate protected or private visibility.

Method names MUST NOT be declared with a space after the method name. The opening brace MUST go on its own line, and the closing brace MUST go on the next line following the body. There MUST NOT be a space after the opening parenthesis, and there MUST NOT be a space before the closing parenthesis.

A method declaration looks like the following. Note the placement of parentheses, commas, spaces, and braces:

```
<?php 
namespace Vendor\Package;
 
class ClassName
{
    public function fooBarBaz($arg1, &$arg2, $arg3 = [])
    {
        // method body
    }
}
```

#### 4.4. Method Arguments <a href="#phpcodingstandards-4.4.methodarguments" id="phpcodingstandards-4.4.methodarguments"></a>

In the argument list, there MUST NOT be a space before each comma, and there MUST be one space after each comma.

Method arguments with default values MUST go at the end of the argument list.

```
<?php 
namespace Vendor\Package;
 
class ClassName
{
    public function foo($arg1, &$arg2, $arg3 = [])
    {
        // method body
    }
}
```

Argument lists MAY be split across multiple lines, where each subsequent line is indented once. When doing so, the first item in the list MUST be on the next line, and there MUST be only one argument per line.

When the argument list is split across multiple lines, the closing parenthesis and opening brace MUST be placed together on their own line with one space between them.

```
<?php 
namespace Vendor\Package;
 
class ClassName
{
    public function aVeryLongMethodName(
        ClassTypeHint $arg1,
        &$arg2,
        array $arg3 = []
    ) {
        // method body
    }
}
```

#### 4.5. `abstract`, `final`, and `static` <a href="#phpcodingstandards-4.5.abstract-final-andstatic" id="phpcodingstandards-4.5.abstract-final-andstatic"></a>

When present, the `abstract` and `final` declarations MUST precede the visibility declaration.

When present, the `static` declaration MUST come after the visibility declaration.

```
<?php 
namespace Vendor\Package;
 
abstract class ClassName
{
    protected static $foo;
 
    abstract protected function zim();
 
    final public static function bar()
    {
        // method body
    }
}
```

#### 4.6. Method and Function Calls <a href="#phpcodingstandards-4.6.methodandfunctioncalls" id="phpcodingstandards-4.6.methodandfunctioncalls"></a>

When making a method or function call, there MUST NOT be a space between the method or function name and the opening parenthesis, there MUST NOT be a space after the opening parenthesis, and there MUST NOT be a space before the closing parenthesis. In the argument list, there MUST NOT be a space before each comma, and there MUST be one space after each comma.

```
<?php 
bar();
$foo->bar($arg1);
Foo::bar($arg2, $arg3);
```

Argument lists MAY be split across multiple lines, where each subsequent line is indented once. When doing so, the first item in the list MUST be on the next line, and there MUST be only one argument per line.

```
<?php 
$foo->bar(
    $longArgument,
    $longerArgument,
    $muchLongerArgument
);
```

### 5. Control Structures <a href="#phpcodingstandards-5.controlstructures" id="phpcodingstandards-5.controlstructures"></a>

The general style rules for control structures are as follows:

* There MUST be one space after the control structure keyword
* There MUST NOT be a space after the opening parenthesis
* There MUST NOT be a space before the closing parenthesis
* There MUST be one space between the closing parenthesis and the opening brace
* The structure body MUST be indented once
* The closing brace MUST be on the next line after the body

The body of each structure MUST be enclosed by braces. This standardizes how the structures look, and reduces the likelihood of introducing errors as new lines get added to the body.

#### 5.1. `if`, `elseif`, `else` <a href="#phpcodingstandards-5.1.if-elseif-else" id="phpcodingstandards-5.1.if-elseif-else"></a>

An `if` structure looks like the following. Note the placement of parentheses, spaces, and braces; and that `else` and `elseif` are on the same line as the closing brace from the earlier body.

```
<?php 
if ($expr1) {
    // if body
} elseif ($expr2) {
    // elseif body
} else {
    // else body;
}
```

The keyword `elseif` SHOULD be used instead of `else if` so that all control keywords look like single words.

#### 5.2. `switch`, `case` <a href="#phpcodingstandards-5.2.switch-case" id="phpcodingstandards-5.2.switch-case"></a>

A `switch` structure looks like the following. Note the placement of parentheses, spaces, and braces. The `case` statement MUST be indented once from `switch`, and the `break` keyword (or other terminating keyword) MUST be indented at the same level as the `case` body. There MUST be a comment such as `// no break` when fall-through is intentional in a non-empty `case` body.

```
<?php 
switch ($expr) {
    case 0:
        echo 'First case, with a break';
    	break;
    case 1:
        echo 'Second case, which falls through';
        	// no break
    case 2:
    case 3:
    case 4:
        echo 'Third case, return instead of break';
        return;
    default:
        echo 'Default case';
        	break;
}
```

#### 5.3. `while`, `do while` <a href="#phpcodingstandards-5.3.while-dowhile" id="phpcodingstandards-5.3.while-dowhile"></a>

A `while` statement looks like the following. Note the placement of parentheses, spaces, and braces.

```
<?php 
while ($expr) {
    // structure body
}
```

Similarly, a `do while` statement looks like the following. Note the placement of parentheses, spaces, and braces.

```
<?php 
do {
    // structure body;
} while ($expr);
```

#### 5.4. `for` <a href="#phpcodingstandards-5.4.for" id="phpcodingstandards-5.4.for"></a>

A `for` statement looks like the following. Note the placement of parentheses, spaces, and braces.

```
<?php 
for ($i = 0; $i < 10; $i++) {
    // for body
}
```

#### 5.5. `foreach` <a href="#phpcodingstandards-5.5.foreach" id="phpcodingstandards-5.5.foreach"></a>

A `foreach` statement looks like the following. Note the placement of parentheses, spaces, and braces.

```
<?php 
foreach ($iterable as $key => $value) {
    // foreach body
}
```

#### 5.6. `try`, `catch` <a href="#phpcodingstandards-5.6.try-catch" id="phpcodingstandards-5.6.try-catch"></a>

A `try catch` block looks like the following. Note the placement of parentheses, spaces, and braces.

```
<?php 
try {
    // try body
} catch (FirstExceptionType $e) {
    // catch body
} catch (OtherExceptionType $e) {
    // catch body
}
```

### 6. Closures <a href="#phpcodingstandards-6.closures" id="phpcodingstandards-6.closures"></a>

Closures MUST be declared with a space after the `function` keyword, and a space before and after the `use` keyword.

The opening brace MUST go on the same line, and the closing brace MUST go on the next line following the body.

There MUST NOT be a space after the opening parenthesis of the argument list or variable list, and there MUST NOT be a space before the closing parenthesis of the argument list or variable list.

In the argument list and variable list, there MUST NOT be a space before each comma, and there MUST be one space after each comma.

Closure arguments with default values MUST go at the end of the argument list.

A closure declaration looks like the following. Note the placement of parentheses, commas, spaces, and braces:

```
<?php 
$closureWithArgs = function ($arg1, $arg2) {
    // body
};
 
$closureWithArgsAndVars = function ($arg1, $arg2) use ($var1, $var2) {
    // body
};
```

Argument lists and variable lists MAY be split across multiple lines, where each subsequent line is indented once. When doing so, the first item in the list MUST be on the next line, and there MUST be only one argument or variable per line.

When the ending list (whether or arguments or variables) is split across multiple lines, the closing parenthesis and opening brace MUST be placed together on their own line with one space between them.

The following are examples of closures with and without argument lists and variable lists split across multiple lines.

```
<?php 
$longArgs_noVars = function (
    $longArgument,
    $longerArgument,
    $muchLongerArgument
) {
    // body
};
 
$noArgs_longVars = function () use (
    $longVar1,
    $longerVar2,
    $muchLongerVar3
) {
    // body
};
 
$longArgs_longVars = function (
    $longArgument,
    $longerArgument,
    $muchLongerArgument
) use (
    $longVar1,
    $longerVar2,
    $muchLongerVar3
) {
    	// body
};
 
$longArgs_shortVars = function (
    $longArgument,
    $longerArgument,
    $muchLongerArgument
) use ($var1) {
    // body
};
 
$shortArgs_longVars = function ($arg) use (
    $longVar1,
    $longerVar2,
    $muchLongerVar3
) {
    // body
};
```

Note that the formatting rules also apply when the closure is used directly in a function or method call as an argument.

```
<?php 
$foo->bar(
    $arg1,
    function ($arg2) use ($var1) {
        // body
    },
    $arg3
);
```
