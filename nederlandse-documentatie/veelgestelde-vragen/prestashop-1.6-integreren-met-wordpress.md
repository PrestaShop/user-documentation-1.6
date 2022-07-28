# PrestaShop 1.6 integreren met WordPress

WordPress is de meest gebruikte CMS op het web en de kans is groot dat u het al gebruikt voor uw website of deze graag wilt gebruiken als blog of voor statische content samen met PrestaShop voor het e-commercegedeelte.

PrestaShop kan een onbeperkt aantal statische pagina's en paginacategoriën aan met zijn CMS-features, maar er zijn situaties waar een blog beter is of een andere CMS-feature dat PrestaShop niet kan bieden. Dit is waar complexere software als WordPress aan te pas komt.

E-commerce en CMS: met PrestaShop en WordPress naast elkaar, krijgt u het beste van beide werelden – zolang u alles goed hebt geconfigureerd.

## Scenario's <a href="#prestashop1.6integrerenmetwordpress-scenarios" id="prestashop1.6integrerenmetwordpress-scenarios"></a>

Er zijn verschillende scenario's mogelijk die u wellicht wilt onderzoeken, afhankelijk van uw wensen en benodigdheden:

* WordPress is de hoofd-URL en PrestaShop is geïnstalleerd in een subdomein/submap.
* PrestaShop is geïnstalleerd in de hoofd-URL en WordPress in een subdomein/submap.
* PrestaShop en WordPress zijn naast elkaar geïnstalleerd.

## U wilt ze gescheiden houden <a href="#prestashop1.6integrerenmetwordpress-uwiltzegescheidenhouden" id="prestashop1.6integrerenmetwordpress-uwiltzegescheidenhouden"></a>

Als u beide gescheiden wilt houden, dan is de integratie simpel: het moeilijkste dat u moet doen is een consistent thema maken voor beide applicaties. U kunt de standaardthema's aanpassen om ervoor te zorgen dat ze veel op elkaar lijken of een designer/developer twee consistente thema's laten ontwikkelen. Houd rekening met het feit dat PrestaShop Smarty gebruikt, terwijl WordPress zijn eigen function calls gebruikt voor het thema:

* PrestaShop 1.6 Designer Guide: [http://doc.prestashop.com/display/PS16/Designer+guide](http://doc.prestashop.com/display/PS16/Designer+guide)
* WordPress theme development documentation: [https://developer.wordpress.org/themes/getting-started/](https://developer.wordpress.org/themes/getting-started/)

Om een idee te krijgen of een PrestaShop-WordPress themacombinatie kan werken, bekijkt u het gratis Velvet Sky theme: [http://www.smashingmagazine.com/2011/06/26/free-prestashop-and-wordpress-e-commerce-theme-velvet-sky/](http://www.smashingmagazine.com/2011/06/26/free-prestashop-and-wordpress-e-commerce-theme-velvet-sky/) (Let op: niet compatibel met 1.6+).

## Door elkaar mengen <a href="#prestashop1.6integrerenmetwordpress-doorelkaarmengen" id="prestashop1.6integrerenmetwordpress-doorelkaarmengen"></a>

Maar u wilt wellicht beide mengen. U wilt bijvoorbeeld dat de content van WordPress tussen kolommen van PrestaShop kan verschijnen (nieuwe producten, huidige winkelwagen, etc.). Op dezelfde manier wilt u wellicht dat uw online winkel links toont naar uw WordPress-content. Al dit en meer kan bereikt worden met WordPress plugins en PrestaShop-modules.

Twee WordPress plugins kunnen u helpen:

* PrestaShop Integration ([http://wordpress.org/plugins/prestashop-integration/](http://wordpress.org/plugins/prestashop-integration/)) voegt 3 widgets toe en een shortcode voor uw WordPress:
  * PrestaShop Integration Hook widget: u kunt de content van vier PrestaShop haken weergeven in een WordPress-thema. Bovenkant van pagina's, linkerkolom, rechterkolom en de onderkant.
  * PrestaShop Integration Module widget: u kunt een PrestaShop module toevoegen aan uw WordPress-thema, via één van PrestaShops haken.
  * PrestaShop Integration Products widget: toont de productlijn in een WordPress-post.
  * `[ps_product_list]` shortcode: deze haak maakt het mogelijk om producten vanuit elke PrestaShop-categorie te tonen op een WordPress-pagina of -post.
* Prestashop User Compatibility ([http://wordpress.org/plugins/prestashop-user-compatibility/](http://wordpress.org/plugins/prestashop-user-compatibility/)) maakt het mogelijk voor uw PrestaShop-gebruikers om in te loggen op WordPress.

Als een alternatief kunt u ook deze WordPress-plugins gebruiken:

* WordPress-PrestaShop Cross Sales ([http://wordpress.org/plugins/wordpress-prestashop-cross-sales/](http://wordpress.org/plugins/wordpress-prestashop-cross-sales/)) voeg PrestaShop-producten toe aan uw WordPress-post of zijbalk.
* DeMomentSomTres PrestaShop Integration ([http://wordpress.org/plugins/demomentsomtres-prestashop/](http://wordpress.org/plugins/demomentsomtres-prestashop/)) integreert content van PrestaShop in WordPress door gebruik te maken van PrestaShop's webservice en WordPress shortcodes.

Aan de andere kant heeft PrestaShop ook modules, geschikt om WordPress te koppelen (wel tegen betaling):

* WordPress Sync ([http://addons.prestashop.com/en/content-management/3052-wordpress-sync.html](http://addons.prestashop.com/en/content-management/3052-wordpress-sync.html)) helpt u met het integreren van uw blog in uw winkel. U kunt content importeren en synchroniseren.
* WordPress Cart ([http://addons.prestashop.com/en/export-modules/6419-wordpress-cart.html](http://addons.prestashop.com/en/export-modules/6419-wordpress-cart.html)) verbindt uw WordPress blog met uw PrestaShop-winkel. Toont uw winkelwagen en links naar het gebruikersaccount.
* PrestaShop to WordPress ([http://addons.prestashop.com/en/export-modules/1174-prestashop-to-wordpress.html](http://addons.prestashop.com/en/export-modules/1174-prestashop-to-wordpress.html)) maakt het mogelijk om zes widgets op uw WordPress-blog te tonen: winkelwagen, categorieën, fabrikanten, nieuwe producten, aanbiedingen en best verkochte producten.
