# Using jQuery and jQueryUI -

## About Controller::addJquery() <a href="#usingjqueryandjqueryui-aboutcontroller-addjquery" id="usingjqueryandjqueryui-aboutcontroller-addjquery"></a>

When this method is called with a parameter, it includes the current version of jQuery, as available in the PrestaShop installation.

For instance, this method can be called from the `setMedia()` method in the `AdminController`:

```
public function setMedia()
{
    $this->addJquery();
}
```

If you wish to use a newer or older version of jQuery, you just have to pass the version number as first parameter:

```
Controller::addJquery('1.3.1');
```

If the file is not available on your server, PrestaShop will try downloading it from the Google servers.

Including a version of jQuery that differs from PrestaShop's default one, means that the `noConflict` flag is automatically called, so that both version can work seamlessly.

Making noConflict work

Version 1.3.1 of jQuery is not available through `$`, but rather using the `$j131` variable.

Hence, you can call `$j131('body').hide();`.

If you wish to use 1.3.1's `$`, you simply have to use this:

```
<script type="text/javascript">
var tmp = $;     // jQuery's current version becomes temporary variable.
$ = $j131;
$('body').hide(); // Now using 1.3.1's hide().
$ = tmp;          // IMPORTANT: always restore the default version of jQuery!
</script>
```

If the file is on your server, you can give its path as a second argument:

```
Controller::addJquery('1.3.1', '/local/path/to/jquery');
```

## About Controller::addJqueryUI() <a href="#usingjqueryandjqueryui-aboutcontroller-addjqueryui" id="usingjqueryandjqueryui-aboutcontroller-addjqueryui"></a>

This method enables you the include the necessary JavaScript files for UI work.

For instance, if you need to use jQuery's slider:

```
public function setMedia()
{
    $this->addJqueryUI('ui.slider');
}
```

This code will automatically include the following dependencies:

```
<script type="text/javascript" src="/trunk/js/jquery/ui/ui.core.min.js"></script>
<script type="text/javascript" src="/trunk/js/jquery/ui/ui.widget.min.js"></script>
<script type="text/javascript" src="/trunk/js/jquery/ui/ui.mouse.min.js"></script>
<script type="text/javascript" src="/trunk/js/jquery/ui/ui.slider.min.js"></script>
```

## About Controller::addJqueryPlugin('plugin\_name') <a href="#usingjqueryandjqueryui-aboutcontroller-addjqueryplugin-plugin_name" id="usingjqueryandjqueryui-aboutcontroller-addjqueryplugin-plugin_name"></a>

This method enables you to include the JavaScript and CSS files for the plugin found in the local `/js/jquery/plugin` folder, or in the folder passed as second parameter.

If you wish to add a specific jQuery plugin to PrestaShop, you must follow this process:

* **If your plugin has only one file**. Put it in the JavaScript plugin folder, as such: `/js/plugins/jquery.plugin_name.js`.
* **If your plugin has other files (CSS, images, etc.)**. Put it in the JavaScript plugin folder, as such: `/js/plugins/plugin_name/jquery.plugin_name.js`.
