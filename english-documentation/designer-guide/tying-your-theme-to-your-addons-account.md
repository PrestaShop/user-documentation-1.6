# Tying your theme to your Addons account

In order to tie your theme to you PrestaShop Addons account, you simply need to add your Addons key to the theme's `config.xml`:

```
<?xml version="1.0" encoding="UTF-8"?>
<!-- Copyright Prestashop -->
<theme version="1.0" name="PRS040094" directory="PRS040094">
    <theme_key>ded5296cb84904fccf9dbc20f0240d6f</theme_key>
    <author name="Firstname Lastname" email="firstname@example.com" url="http://example.com"/>
    <descriptions>
        <description iso="en">HTML5 + CSS3 &amp;amp; Reponsive &amp;amp; Many More</description>
    </descriptions>

(...)
```

The `theme_key` can be found in your contributor account, in the theme upload page.
