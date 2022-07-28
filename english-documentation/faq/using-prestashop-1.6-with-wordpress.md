# Using PrestaShop 1.6 with WordPress

WordPress is the most-used CMS on the Web, and chance is that you are already using it for your site, or plan on using it for your blog or static content alongside PrestaShop for the e-commerce part.

PrestaShop is able to handle an unlimited number of static pages and page categories using its CMS feature, but there are situations when a blog might be necessary, or simply more advanced CMS features that PrestaShop or its modules do not provide. This is where a more complex tool such as WordPress might be useful.

E-commerce and CMS: with PrestaShop and WordPress side by side, you get the best of both worlds – as long as you can configure it all correctly.

## Scenarios <a href="#usingprestashop1.6withwordpress-scenarios" id="usingprestashop1.6withwordpress-scenarios"></a>

There are different scenarios that you might want to explore, depending on your needs and preferences:

* WordPress on the root URL and PrestaShop installed on a subdomain/subfolder.
* PrestaShop installed on the root URL and WordPress on a subdomain/subfolder.
* PrestaShop and WordPress installed side by side.

## You gotta keep'em separated <a href="#usingprestashop1.6withwordpress-yougottakeepemseparated" id="usingprestashop1.6withwordpress-yougottakeepemseparated"></a>

If you want to keep each separate, the integration is easy: the hardest thing to do will be to have a consistent theme for both applications. You can either adapt each application's default theme in order to have them look as similar as possible, or have a designer/developer build two consistent theme for both. Note that the PrestaShop theme API uses Smarty, while the WordPress theme API uses its own PHP function calls:

* PrestaShop 1.6 Designer Guide: [http://doc.prestashop.com/display/PS16/Designer+guide](http://doc.prestashop.com/display/PS16/Designer+guide)
* WordPress theme development documentation: [https://developer.wordpress.org/themes/getting-started/](https://developer.wordpress.org/themes/getting-started/)

In order to get an idea of how a PrestaShop-WordPress theme combo can work, check out the free Velvet Sky theme: [http://www.smashingmagazine.com/2011/06/26/free-prestashop-and-wordpress-e-commerce-theme-velvet-sky/](http://www.smashingmagazine.com/2011/06/26/free-prestashop-and-wordpress-e-commerce-theme-velvet-sky/) (Note: not compatible with PrestaShop 1.6+).

## Mix-A-Lot <a href="#usingprestashop1.6withwordpress-mix-a-lot" id="usingprestashop1.6withwordpress-mix-a-lot"></a>

But you might want to mix both of them. For instance, you might want to display the WordPress content in-between columns full of PrestaShop content (new products, current cart, etc.). Likewise, you might want to have your online store display links to your WordPress content. All this and more can be with a few well chosen WordPress plugins and PrestaShop modules.

Two WordPress plugins can help you:

* PrestaShop Integration ([http://wordpress.org/plugins/prestashop-integration/](http://wordpress.org/plugins/prestashop-integration/)) adds 3 widgets and a shortcode to your WordPress installation:
  * PrestaShop Integration Hook widget: you can integrate the content of any of four PrestaShop hooks into any WordPress theme: Top of pages, Left column block, Right column block, Footer.
  * PrestaShop Integration Module widget: you can insert a PrestaShop module in your WordPress theme, via one of PrestaShop's hooks.
  * PrestaShop Integration Products widget: display the product list attached to a WordPress post.
  * `[ps_product_list]` shortcode: this hooks makes it possible to display products from any PrestaShop category into a WordPress page or post.
* Prestashop User Compatibility ([http://wordpress.org/plugins/prestashop-user-compatibility/](http://wordpress.org/plugins/prestashop-user-compatibility/)) makes it possible for your PrestaShop users to log in WordPress.

As an alternative, you can use these WordPress plugins:

* WordPress-PrestaShop Cross Sales ([http://wordpress.org/plugins/wordpress-prestashop-cross-sales/](http://wordpress.org/plugins/wordpress-prestashop-cross-sales/)) includes PrestaShop products on your WordPress post or sidebar.
* DeMomentSomTres PrestaShop Integration ([http://wordpress.org/plugins/demomentsomtres-prestashop/](http://wordpress.org/plugins/demomentsomtres-prestashop/)) integrate content from PrestaShop into WordPress using PrestaShop's webservice and WordPress shortcodes.

On the other side, PrestaShop has WordPress-dedicated modules (but most are for pay):

* WordPress Sync ([http://addons.prestashop.com/en/content-management/3052-wordpress-sync.html](http://addons.prestashop.com/en/content-management/3052-wordpress-sync.html)) helps you integrate your blog into your store. You can import content and keep both in sync.
* WordPress Cart ([http://addons.prestashop.com/en/export-modules/6419-wordpress-cart.html](http://addons.prestashop.com/en/export-modules/6419-wordpress-cart.html)) connects your WordPress blog with your PrestaShop store. Displays your shopping cart and links to the user account.
* PrestaShop to WordPress ([http://addons.prestashop.com/en/export-modules/1174-prestashop-to-wordpress.html](http://addons.prestashop.com/en/export-modules/1174-prestashop-to-wordpress.html)) enables you to insert up to six widgets on your WordPress blog: cart, categories, manufacturers, new products, specials and top sellers
