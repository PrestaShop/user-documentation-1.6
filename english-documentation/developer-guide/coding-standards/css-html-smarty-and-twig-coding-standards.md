# CSS, HTML, Smarty & Twig Coding Standards

Regarding the CSS and HTML codebase, because we have integrated Bootstrap 4 both in the back office and front office of PrestaShop 1.7, we have decided to follow their [coding standards](http://codeguide.co), maintained by [@mdo](css-html-smarty-and-twig-coding-standards.md).

When you are writing HTML code, if your line is longer than 120 characters, we have chosen to do a line break after each attributes with an indentation. For example, it will look like this:

```
<img class="test"
  id="..."
  name="..."
  data="..."
  src="..."
  title="..."
  alt="..."
  role="..."
>
```

Some noteworthy rules:

* HTML
  * Use soft tabulations with two spaces to indent.
  * Avoid superfluous HTML markup.
  * No more self-closing tag.
* CSS
  * Use soft tabulations with two spaces to indent.
  * When grouping selectors, keep individual selectors to a single line.
  * End all declarations with a semicolon, even the last one.

```
<img class="test" src="...">
img,
a,
input[type="text"] {
  display: block;
  padding: 15px;
  margin-bottom: 15px;
  background-color: rgba(0,0,0,.5);
  box-shadow: 0 1px 2px #ccc, inset 0 1px 0 #fff;
}
```

PrestaShop 1.7 uses both the Smarty and Twig template engine. Since those are mostly used to generate HTML, we expect the Smarty/Twig code to comply with the HTML standards above – as well as the one used by SensioLabs for Twig.

Some noteworthy rules:

* Use soft tabulations with two spaces to indent.
* Use single quotes to surround strings.
* Use [snake case](https://en.wikipedia.org/wiki/Snake\_case) (underscores) to name your blocks.

```
{% raw %}
{% block my_block_name %}
   {% set foo = 'foo' %}
{% endblock %}
{% endraw %}
```

```
```
