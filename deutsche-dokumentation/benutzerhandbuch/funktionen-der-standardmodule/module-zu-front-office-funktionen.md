# Module zu Front-Office-Funktionen

Many of these are installed by default. Therefore, if some of PrestaShop's functionalities are not useful to you, you can disable them here.

## Banner block <a href="#modulezufront-office-funktionen-bannerblock" id="modulezufront-office-funktionen-bannerblock"></a>

Displays a banner at the top of your store's home page (depending on your store's settings).

Make the banner very wide while keeping the content centered, so that the banner can adapt to all device sizes.

## Cart block <a href="#modulezufront-office-funktionen-cartblock" id="modulezufront-office-funktionen-cartblock"></a>

Displays the products that your customers added to their carts; on all the pages. Visitors can then see their choices while shopping, change the quantity of product they are ordering, and delete or add a coupon. By clicking on "Shopping Cart", they see the "Shopping cart summary" of all products added to their cart, and their quantity.

You can configure the cart to use Ajax, which means that any change that the uses makes to his shopping list will apply immediately instead of reloading the page. The Ajax setting is not compatible with all themes, be sure to test it thoroughly with your own theme.

You can also set the maximum number of products that your cart should display.

## Categories block <a href="#modulezufront-office-funktionen-categoriesblock" id="modulezufront-office-funktionen-categoriesblock"></a>

Displays a list of your product categories on your shop.

You have a few configuration possibilities:

* **Maximum depth**. If you have a great number of categories, or with long names, you might prefer to not break your design and limit the number of sub-levels that should be displayed.
* **Dynamic**. When enabled, sub-categories are hidden by default, and the customer can choose to display them. This is great for preserving space and avoiding clutter: if disabled, this module displays all categories and all their sub-categories.
* **Sort**. Most of the time, you should keep the category sort to alphabetical, for easier perusing. But the "By position" sort enables you to choose which categories should be at the top, and thus promote these.
* **How many footer columns would you like?**. Enables you to choose the number of columns in the "Category" block of your footer.

## CMS Block <a href="#modulezufront-office-funktionen-cmsblock" id="modulezufront-office-funktionen-cmsblock"></a>

Adds a block with several CMS links.

The first section, "CMS Block configuration", has one option:

* **CMS blocks**. You can have your CMS content be displayed either in the left column of your shop, or the right column. You can edit the content of the existing page by clicking on the 'edit' icon on the right of its name, or add new blocks of content on either side by clicking on the "Add new" button.

The second section, "Footer's various links configuration", has four options:

* **Display various links and information in the Footer**. You can choose to not display any CMS page in the footer, simply by unchecking this setting.
* **Footer links**. The CMS pages linked from this section appear at the bottom of the site. This is where shop owners tend to place informational pages: legal notice, terms & conditions, etc.
* **Footer text**. You can add one line or paragraph of text below the list of CMS pages in the footer. Write it in as many languages as needed.
* **Display "Powered by PrestaShop"**. Adds a line with a link to [prestashop.com](http://prestashop.com). Note that this line is located between the links and the footer text.

When you delete the footer text, PrestaShop might give you this error: "Please provide footer text for the default language".

This is because when you first enter a footer text, PrestaShop replicates it in all the available languages. When you delete the text, you must therefore delete it from all the available languages: first delete the text from the default language, then click on the language selector next to the text field, choose another language, and delete the content of the field again. Do this for every language. You can then save your changes, and PrestaShop will not display the error anymore.

## Contact block <a href="#modulezufront-office-funktionen-contactblock" id="modulezufront-office-funktionen-contactblock"></a>

Allows you to display extra information about customer service:

* **Phone number**. This should be a dedicated customer service/support number, not a way to contact the sales section or the partnership program (if any). If you do not provide customer service by phone, leave this field empty.
* **E-mail**. Again, this should be a dedicated customer service/support e-mail address.

This information appears in the footer by default.

## Contact information block <a href="#modulezufront-office-funktionen-contactinformationblock" id="modulezufront-office-funktionen-contactinformationblock"></a>

Adds a block to add some information about contacting the shop:

* **Company name**. Your company's name might be different from your shop's name. Indicating the full name brings trust to your brand.
* **Address**. Your headquarters' address, or if it applies, your main shop address. Do not give your own personal address, as you certainly do not want customers to come knock at your door. If you do not want people visiting or sending your letters, leave this field empty.
* **Phone number**. Your business phone line. Again, do not give your personal number here. If you do not have a dedicated business line, leave the field empty.
* **Email**. Your business e-mail address, where you want to receive any correspondence (often including support requests).

This information appears in the footer by default.

## Cross-Selling <a href="#modulezufront-office-funktionen-cross-selling" id="modulezufront-office-funktionen-cross-selling"></a>

Displays a "Customers who bought this product also bought..." block on each product page. You can set the number of products to be displayed (default is 10).

## Currency block <a href="#modulezufront-office-funktionen-currencyblock" id="modulezufront-office-funktionen-currencyblock"></a>

Adds a little interface feature where customers can choose which currency will be used to display prices, as well as how the customers will pay for their orders. The block appears in the header (top part) of your shop, and only displays the installed currencies. To add a currency or configure the existing ones, go to the "Currencies" page, under the "Localization" menu.

## Custom CMS information block <a href="#modulezufront-office-funktionen-customcmsinformationblock" id="modulezufront-office-funktionen-customcmsinformationblock"></a>

Adds a block containing information for your customer, retrieved from your CMS pages.

You have two custom blocks by default, each with an edit button. Click that button will give you access to and a text editor, where you can enter the basic information for your home page. That editor features an "HTML" button, which makes it possible to enter specific HTML tags, and using custom classes and such, which you can then style with CSS.

## Customer data privacy block <a href="#modulezufront-office-funktionen-customerdataprivacyblock" id="modulezufront-office-funktionen-customerdataprivacyblock"></a>

Adds a block to display a message about customer data privacy. The configuration screen simply presents you with a big text area. It is up to you to fill it up with your data privacy policy.

This is an important text, as people online are more and more worried about privacy. Providing a clear policy of how you handle their private information brings trust to your brand – and also ties you legally to respect it. You should never copy/paste a policy from another site, but write your own, based on your country's privacy laws.

## Customer reassurance block <a href="#modulezufront-office-funktionen-customerreassuranceblock" id="modulezufront-office-funktionen-customerreassuranceblock"></a>

Adds a block to display more information to reassure your customers. This block appears in the footer of the default theme. It was previously called "Bloc reinsurance".

The default sample pages are:

* **Money back guarantee**. Says Wikipedia, "A money-back guarantee is essentially a simple guarantee that, if a buyer is not satisfied with a product or service, a refund will be made."
* **In-store exchange**. The text should explain that the customer can bring any unwanted product to your physical store in order to make an exchange with another model, or get a refund. If you do not have a store, you certainly should delete this page.
* **Payment upon shipment**. The customer only pays for the order once it has been shipped. It is not recommended for smaller shops.
* **Free shipping**. This is where you indicate your shipping policy. All shipping can be free, or you can choose to have it be free starting with a certain amount, for instance.
* **100% secured payment processing**. Typically, because you rely on third-party payment services such as PayPal or Moneybookers, you trust them with your money exchanges, and so should your customers. You can paste information about each payment service in this page.

These are only sample pages: they do not have any content by default. It is therefore up to you (and your legal team) to fill it with the proper text. If some of the sample policies do reflect your business, you should delete them.\
Click on the 'edit' icon at the right in order to add text that fits your shop's trust features. You can remove or add pages as you see fit.

## Facebook Like Box block <a href="#modulezufront-office-funktionen-facebooklikeboxblock" id="modulezufront-office-funktionen-facebooklikeboxblock"></a>

Displays a new block on your home page with a link to your store's Facebook page, a Like button, and photos of people who liked your page.

## Facebook sharing block <a href="#modulezufront-office-funktionen-facebooksharingblock" id="modulezufront-office-funktionen-facebooksharingblock"></a>

Adds a block to display a link "Share on Facebook" on product pages. Clicking the link directs the customer to his or her Facebook page, with a pre-filled link to the product.

## Favorite Products <a href="#modulezufront-office-funktionen-favoriteproducts" id="modulezufront-office-funktionen-favoriteproducts"></a>

Adds an "Add this product to my favorites" link on each product page, only visible to logged-in customers. They can then access their list of favorite products by going to their account page and clicking the "My favorite products" link.

## Featured Products on the homepage <a href="#modulezufront-office-funktionen-featuredproductsonthehomepage" id="modulezufront-office-funktionen-featuredproductsonthehomepage"></a>

With this module, you can choose which products to highlight by placing them on your homepage.

In the configuration page, you can set the number of products you want to show. Once this value is saved, go into the configuration page of a product of your choice ("Catalog" menu). Select "Home" as the category into which the product appears, in addition to its current categories (do not remove its original category). Save your change, and you product will appear on your shop's home page.\
Repeat for all of the products that you want to place on the home page.

## FIA-NET Sceau de Confiance <a href="#modulezufront-office-funktionen-fia-netsceaudeconfiance" id="modulezufront-office-funktionen-fia-netsceaudeconfiance"></a>

**France only**.

Turn your visitors into buyers by promoting trust in your site.

FIA-NET is a French third-party e-commerce trust partner: it protects both customers and online shops against credit card frauds and other malevolent activities.

You have to be a FIA-NET partner in order to use the module. Ask for more information here: [http://www.fia-net-group.com/form\_partenaires\_fianet.php?p=185](http://www.fia-net-group.com/form\_partenaires\_fianet.php?p=185). Once you have your account details, you can configure the module with them, and the FIA-NET logo will be displayed on your front page. This logo is well known in France, and lets visitors know that your shop is trustworthy.

When configuring the module, you can choose to use the Test mode or the Production mode. The Test mode enables you to perform some test purchases and see how the FIA-NET system reacts.

## Home Editorial <a href="#modulezufront-office-funktionen-homeeditorial" id="modulezufront-office-funktionen-homeeditorial"></a>

Adds a block to the central column of your homepage, with an image above a text, both of which you can edit by configuring the module.

You can move the block around in your design using the Live Edit tool.

The homepage is the first thing your visitors experience when they discover your shop. Therefore, be sure to make it pleasant and efficient, and to update it regularly. Make sure to translate the text in as many languages as your shop supports.

## Image slider for your homepage <a href="#modulezufront-office-funktionen-imagesliderforyourhomepage" id="modulezufront-office-funktionen-imagesliderforyourhomepage"></a>

Adds a slider block on your homepage's central column, where you can define a set of images that will be displayed one after the other, with a sliding motion.

The module's configuration screen presents you with two sections:

* **Settings**. You can set the size of the block, the time to wait between two images, and whether the slide should loop or not.
* **Slides list**. You can visually arrange the images' order by drag-and-dropping their individual blocks.\
  Three icons at the right of each block enables you to enable/disable the image, edit its settings, or remove it from the set altogether.

### Adding/editing an image <a href="#modulezufront-office-funktionen-adding-editinganimage" id="modulezufront-office-funktionen-adding-editinganimage"></a>

Make sure that all the images have the exact same size, and that this size is reflected in the block's own size (in the "Slider configuration" section).

Clicking the "Add Slide" link brings you to a new screen.

* **Select a file**. Note that you can have text on the image, and indicate the language of that text using the language selector.\
  Additionally, this means you can have a different image for each language. But be aware they these images will be tied: same position, inability to delete one without deleting the others, etc.
* **Title**. The title appears in the "Slides configuration" section, and helps you sort the images.
* **URL**. You can choose to send the customer to a given page of your shop when he or she clicks the image. This is useful when the image promotes a certain product, category or manufacturer.
* **Caption**. The alternate text to be used if somehow the image cannot be loaded. This is essential for accessibility.
* **Description**. The text appears when the mouse pointer hovers over the image.
* **Active**. You can disable an image whenever needed, for instance when the discount it promotes ends.

## Language block <a href="#modulezufront-office-funktionen-languageblock" id="modulezufront-office-funktionen-languageblock"></a>

Displays a block of the available languages at the top of the homepage. This block enables the customer to choose the language in which he or she wants the shop to appear. If you do not want the customers to be able to change the shop's languages, then uninstall this block.

## Layered navigation block <a href="#modulezufront-office-funktionen-layerednavigationblock" id="modulezufront-office-funktionen-layerednavigationblock"></a>

Displays a block with layered navigation filters. Layered navigation enables the customer to define cumulative criteria to filter category products, little by little providing more details in order to reduce the number of displayed products. This is a great tool for customers who know the details of what they want (color, condition, price range...), but are unsure how to find it.

When configuring the module, you are presented with 4 sections:

* **Indexes and caches**. This module heavily relies on database index and its own content cache.
* **Existing filter templates**. A filter template is the kind of navigation to which the customer has access to.
* **Build your own filter template**. You can build various templates, which will serve as the basis for what the customer sees.
* **Configuration**. You can further detail the way this module operates.

### Indexes and caches <a href="#modulezufront-office-funktionen-indexesandcaches" id="modulezufront-office-funktionen-indexesandcaches"></a>

In order to work properly, layered navigation needs to be kept up-to-date with your latest products, product attributes and product prices – unless these never change. You should therefore regularly re-index the data, using the buttons provided here. They each have specific actions:

* **Index all missing prices**. Only adds to the index the prices that were not indexed before. Much faster than the next button.
* **Rebuild entire price index**. Adds to the index all the prices, whether they were already indexed before or not. Much slower than the previous button when you have many products.
* **Build attribute index**. Adds to the index all the product attributes.
* **Build url index**. Adds to the index the URLs for all the products.

You should update your indexes every time your products' data changes. As this can prove pretty painstaking or even boring, PrestaShop enables you to trigger the indexing automatically, using cron tasks. Add the provided URLs to your crontab, and you will not have to handle this yourself anymore. If you do not know about cron and crontab, ask your webhost about it.

### Existing filters templates <a href="#modulezufront-office-funktionen-existingfilterstemplates" id="modulezufront-office-funktionen-existingfilterstemplates"></a>

Layered navigation is based on templates, or groups of criteria. There is one by default, named "My template", which makes use of all the available filters. You should create templates more adapted to your content or needs.

You can have as many templates as needed. This section enables you to edit and delete them when necessary.

### Build your own filters template <a href="#modulezufront-office-funktionen-buildyourownfilterstemplate" id="modulezufront-office-funktionen-buildyourownfilterstemplate"></a>

The template builder enables you to specify what kind of filters your customers should have access to.

Creating a new template requires only three easy steps:

1. **Select categories**. You can either create filter for the whole site, or on a per-category basis.\
   You could for instance have the whole site display the price filter, while some categories can have additional filters.\
   When choosing "Specific categories", a small window opens where you can choose in which categories this filter should be available.\
   Note that filters do not automatically apply to sub-categories of the selected category: if there is no product on your "Home" category, then the layered navigation will not appear there.
2. **Selected filters**. The number of available filters depends on the content of your shop. Six default filters will appear here: price, weight, condition, manufacturer, available stock and sub-categories. Along with these are the attribute groups for all products in the selected categories (with the number of products). Check a filter's box to move if from the "Available" section to the "Selected" one. You can move the filters up and down with your mouse cursor, which will influence their display in the front-page.\
   Each filter has a two drop-down menu included:
   * **Type of display**. You can choose how the filter is displayed to the customer. The visualization depends on the type of the filter.
     * Numerical (price & weight): check-box, radio button, drop-down list. Note that only the check-box setting allows for multiple selection.
     * Alphabetical (all others): slider, inputs area, list of values.
   * **Limit**. If some of your categories have too many choices for a given filters, you can limit the number of displayed items using this selector.
3. **Name your template**. Customers will not see the name, but it will prove very useful to you when you have to edit one template among the dozen or hundred you may create in the lifespan of your shop.

Note that saving the filter will not save the whole configuration: you have to save the filter first, then click on "Save configuration".

### Configuration <a href="#modulezufront-office-funktionen-configuration" id="modulezufront-office-funktionen-configuration"></a>

Two options are available:

* **Hide filter values with no product is matching**. If disabled, you will still see filters, even if they are useless because of the lack of matching product (which can make the layered navigation over-crowded with options).
* **Show the number of matching products**. Displays the number after the name of the filter, between brackets. If there is no matching product, it will display "(0)".
* **Show products from subcategories**. The filter applies to more than just the current category.
* **Category filter depth (0 for no limits, 1 by default)**. If the above option is enabled, you risk having too many products taken into account, and lose the interest of layered navigation. The depth is of 1 by default, but you can use even deeper sub-categories.
* **Use tax to filter price**.
* **Allow indexing robots (google, yahoo, bing, ...) to use condition/availability/manufacturer filter**. These four filters help you define whether search bots should be able to browse your navigation and index it. This can prove beneficial for SEO (search engine optimization).

These options apply to all templates and filters.

## Link block <a href="#modulezufront-office-funktionen-linkblock" id="modulezufront-office-funktionen-linkblock"></a>

With this module, you can add links to the sites you want, or to pages of your shop.

The configuration page is divided in three sections:

* **Add a new link**. Enables you to specify the link's name and URL, and whether it should open in a new page or not.\
  When adding a link, do not forget the "`http://`" part. For instance, [**http://**www.myprestashop.com](http://www.myprestashop.com/).\
  Note that it is often said that opening a link in a new page is bad practice. At the very least, you should keep your shop's own page in the same window.
* **Block title**. Enables you to rename the link block itself, and even link to a page from the block's title.
* **Settings**. Enables you to sort the links. By default the links are ordered by most recently added link. If you want to invert this setting, select instead "by oldest links" from the drop-down list.

At the bottom of the page, you will find all of the links that you have entered. If you would like to modify the links, click the edit icon. To delete a link, click the trashcan icon.

## Manufacturers block <a href="#modulezufront-office-funktionen-manufacturersblock" id="modulezufront-office-funktionen-manufacturersblock"></a>

Displays a block of manufacturers/brands.

The block's content can be displayed in two ways: either as a list of links, or as a drop-down list. It can even display both, with the text links being limited in number, whereas the drop-down list gives access to all the manufacturers.\
Manufacturers are displayed alphabetically.

## My Account block <a href="#modulezufront-office-funktionen-myaccountblock" id="modulezufront-office-funktionen-myaccountblock"></a>

Displays a block containing links to the logged customer's various account pages: previous orders, package tracking, product returns, registered addresses, available coupons, etc. Once the client is connected, this block is displayed.

## My Account block for your website's footer <a href="#modulezufront-office-funktionen-myaccountblockforyourwebsitesfooter" id="modulezufront-office-funktionen-myaccountblockforyourwebsitesfooter"></a>

This is the equivalent to the "My Account block" module (see above), but specifically designed to be used in the theme's footer.

## New products block <a href="#modulezufront-office-funktionen-newproductsblock" id="modulezufront-office-funktionen-newproductsblock"></a>

Displays a block presenting the recently added products, in order to make them more visible. With this block, you can drive more traffic to your new products. You can set the number of visible links by configuring this module.

By default, a product is considered as new if it has been added to the shop's catalog in the last 20 days. You can change that setting in the "Products" page under the "Preferences" menu.\
If you do not have recent product, displaying this block will hint that you do not renew your catalog much. Therefore, it is not recommended to enable the "Always display block" option for this module.

## Newsletter block <a href="#modulezufront-office-funktionen-newsletterblock" id="modulezufront-office-funktionen-newsletterblock"></a>

Displays a block which invites your shop's visitors to subscribe to your newsletter.

In the configuration screen, you can set several options:

* **Would you like to send a verification email after subscription?**. This is important, as it prevents unsuspecting people to be subscribed without their knowledge.
* **Would you like to send a confirmation email after subscription?**. Likewise, a customer should always confirm they he or she chose to be subscribed to your newsletter. This way they cannot say you are sending them spam without their consent.
* **Welcome voucher code**. You can thank new subscribers with a voucher code. For instance, you can offer them 10% off their next order.\
  To create a new voucher code, go to the "Cart rules" page under the "Price rules" menu. See how to create a voucher in the "Creating Price Rules and Vouchers" chapter.

## Payment logos block <a href="#modulezufront-office-funktionen-paymentlogosblock" id="modulezufront-office-funktionen-paymentlogosblock"></a>

Adds a block to display all payment logos.

The module's configuration page enables you to choose where to display these logos. Therefore, you should first create a CMS page where you would put the payment logos and descriptions for all the payment services you support, then link to that page from the module's configuration page.

## Permanent links block <a href="#modulezufront-office-funktionen-permanentlinksblock" id="modulezufront-office-funktionen-permanentlinksblock"></a>

Adds a block on the front-end which displays permanent links to your CMS pages, such as sitemap, contact, etc.

## Product Comments <a href="#modulezufront-office-funktionen-productcomments" id="modulezufront-office-funktionen-productcomments"></a>

Enables logged-in customers or visitors to leave a message on your product page. Comments will appear in a new tab right on the product page, next to the "More info" section. They can also rate your products, between 0 and 5 stars.\
You can also manage comments from this module, such as moderate them or delete them.

Logged-in customers can also report spam or useless comments to you: when a comment is displayed on a product page, it has two options:

* "Was this comment useful to you?" If the customer clicks "No", other visitors will see this.
* "Report abuse". If the customer clicks this button, the comment goes to the "Reported comments" queue.

The configuration screen gives you access to several sections:

* **Configuration**.
  * **All comments must be validated by an employee**. This makes sure that no spam or insult ever appears on your live site, which could ruin your content. Note that in some countries, validating content is akin to publishing them yourself, and therefore can make you responsible for their content.
  * **Allow guest comments**. You can allow non-logged visitors to publish comments too. Be careful, as this can greatly increase spam comments.
  * **Minimum time between 2 comments from the same user**. This prevents spam bot to fill your inbox with comments – or at least limits the impact.
* **Moderate Comments**. If you chose to have comments validated by your staff before they are public, they will be displayed in this section, and can choose to put them offline if you feel they are detrimental.
* **Reported Comments**. Customers can click a "Report abuse" link on any comment, which will bring it to your attention here. You can choose to dismiss the report and accept the comment, or remove the comment altogether.
* **Add a new comment criterion**. You can motive your customers to leave comments by providing them with criteria, or "themes": text fields with a title indicating what the comment should be about, such as "scent", "taste", "robustness". This helps your customers come up with ideas for their comment.
  * **Name**. The name is visible to your customers, so choose a short and specific one.
  * **Apply to**. You can choose to have the chosen criterion field appear on all products ("Valid for the entire catalog"), or on a set of products.\
    If you choose to restrict the criterion to a subset of your catalog (either some categories or some products), a new section will appear after saving your criterion: "Manage criterions scope". See below.
  * **Active**. You can disable a criterion at any time.
* **Manage criterions scope**. This section only appears when you have at least one criterion that is restricted to a subset of your catalog.\
  In the drop-down list, choose the criterion for which you want to set the scope. The page will reload with a table of all your categories or products (depending on the scope choice). Check the boxes for all the items that apply, and validate.
* **Manage Comments**. This is where all the public comments appear. You can choose to delete them by clicking on the Delete icon, either one by one or in batch.

## Product Payment logos block <a href="#modulezufront-office-funktionen-productpaymentlogosblock" id="modulezufront-office-funktionen-productpaymentlogosblock"></a>

Displays payment logos right on the product page. The configuration page makes you choose an image – which you have to build yourself by combining the logos of the payment methods you accept.

## Products category <a href="#modulezufront-office-funktionen-productscategory" id="modulezufront-office-funktionen-productscategory"></a>

On each product page, displays suggestions of other products that are in the same category. This module is particularly useful for discovering what your shop has to offer.

In the configuration page, you can choose whether to display the other products' prices or not.

## Product tooltips <a href="#modulezufront-office-funktionen-producttooltips" id="modulezufront-office-funktionen-producttooltips"></a>

Displays live notifications on your shop. This module helps the visitors know what is happening on your shop in real time. Whenever a visitor visits a product's page, three kinds of notification can be displayed over the content at the top right of the page:

* The number of people who are currently also watching this page. In effect, it displays the number of people who have been on this page in the last 30 minutes, 30 being the default value, which you can change using the "Lifetime" option.
* The last time this product has been bought.
* The last time this product has been added to a cart.

The first option is always a nice thing to have. The other two are a bit trickier: on a successful product, it can be nice to see it has been recently bought; on the other hand, less-successful products will be seen as failures if they have not been bought for a long period of time.\
This is why the "Do not display events older than" option is important: make sure not to change it to double-digit number, or you will without doubt make fewer sales of already-disappointing products.

## RSS Feed (RSS products feed) <a href="#modulezufront-office-funktionen-rssfeed-rssproductsfeed" id="modulezufront-office-funktionen-rssfeed-rssproductsfeed"></a>

Enables you to generate a RSS Product feed for your shop's catalog. A RSS feed is a website content syndication format, which enables anyone to display the latest content from a website on another. \
With this module, loyal customers will be able to get regular updates about products added to your catalog, by adding this feed to their own feed reader, without the need to subscribe to your newsletter. Also, other websites will be able to display your new products on their page. Finally, search engines may use it to discover your new content.

In case of a multistore installation, you can display the new products from one shop, right in the sidebar of another of your shop using its RSS Feed Block module.

If you would rather not have your content be available to anyone online, disable this module.

## RSS feed block <a href="#modulezufront-office-funktionen-rssfeedblock" id="modulezufront-office-funktionen-rssfeedblock"></a>

Adds a block displaying an RSS feed. A RSS feed is a website content syndication format, which enables anyone to display the latest content from a website on another. \
With this module, your visitors can stay informed about news from a site that you specify in the field provided in the module configuration. The RSS feed will then appear on the front of your shop in a block. Visitors can sign up for the RSS feed in this block.

This module has three configuration options:

* **Block title**. Give the block a comprehensible name: you might not want your visitors to think that the content displayed is from your own website.
* **Add a feed URL**. Do not put your shop's address in this field, as it could create an error.
* **Number of threads displayed**. Usually, a RSS feed contains 10 to 20 of the latest articles from the source website. You could limit that to 5 or fewer, in order to not clutter your homepage with content other than your products.

## Send to a Friend module <a href="#modulezufront-office-funktionen-sendtoafriendmodule" id="modulezufront-office-funktionen-sendtoafriendmodule"></a>

Displays a "Send to a friend" link at the bottom of every product pages. Clicking it opens a window where the customer can enter the name and e-mail of the person who he wants to tell about this product. The e-mail sent contains a simple link to the product's page.

This module can be important, because as a shop owner, you want to give your customers the opportunity to spread knowledge of your products and your shop.

## Social networking block <a href="#modulezufront-office-funktionen-socialnetworkingblock" id="modulezufront-office-funktionen-socialnetworkingblock"></a>

Allows you to add extra information about social networks where your customers can find you. Specifically, you can indicate your account URLs for:

* **Facebook**. Avoid using your own userpage! Try to create a page for your shop/company instead.
* **Twitter**. Likewise, use your company's user account, not your CEO's.
* **Your RSS feed**. A RSS feed is a special file that is generated automatically by your shop, and can be used by RSS readers tools (such as Google Reader) to send your latest news to your customers. While it is not a social network, it is an important aspect of sending regular news out there. Note: you must have the "RSS products feed" module installed in order for this to work.

## Store locator block <a href="#modulezufront-office-funktionen-storelocatorblock" id="modulezufront-office-funktionen-storelocatorblock"></a>

Displays a block with a link to the store locator. If you do not have any physical location where customers can buy or at least retrieve products, then be sure to disable this module.

Your list of physical stores is available in the "Store Contacts" page, under the "Preferences" menu. By default, there are a handful of sample stores lists, which you should delete in order to replace them with your own.

The configuration page simply enables you to choose a picture to display as the link to the store locator.

## Suppliers block <a href="#modulezufront-office-funktionen-suppliersblock" id="modulezufront-office-funktionen-suppliersblock"></a>

Displays a block of suppliers.

The block can display two types of content: either as a list of links, or as a drop-down list. It can even display both, with the text links being limited in number, whereas the drop-down list gives access to all the suppliers.\
Suppliers are displayed alphabetically.

## Tags block <a href="#modulezufront-office-funktionen-tagsblock" id="modulezufront-office-funktionen-tagsblock"></a>

Each of your products can have tags added to its description page. Basically, they help create on-the-fly categories of products which have the same tags, but this module makes tags even more useful by adding a block in one of the theme's columns, where the most popular tags are displayed in order of importance, with the most prominent ones using a bigger font.

In the configuration page, indicate how many keywords should appear.

## Theme configurator <a href="#modulezufront-office-funktionen-themeconfigurator" id="modulezufront-office-funktionen-themeconfigurator"></a>

Helps you configure some aspects of your theme.

The configuration page for this module serves two purposes.

First, it gives you direct links to the most usual front-office settings: from this module, you can enable and disable a dozen of features, such displaying social buttons or the Facebook block. You can also access the Live Configurator (Live Edit) from here.

Second, the Theme Configurator itself makes it possible for you to easily attach images with links on specific home page hooks: home, top, left, right, footer. Each available language has its own tab with its own hooks that you can edit from here.

## Top-sellers block <a href="#modulezufront-office-funktionen-top-sellersblock" id="modulezufront-office-funktionen-top-sellersblock"></a>

Adds a block displaying the shop's top selling products.

The configuration page enables you to set if the block should be displayed even when there is no product or even no product sale yet.

The block is not present in the default theme at first. You will have to hook it to a location, for instance the right column.

To hook the module to the right column, go to the module's configuration page, then:

1. Click the "Manage hooks" link at the top. You are taken to the "Positions" page.
2. As you can see in the "Positions" page, the module does not appear in any hook. Click the "Transplant a module" button at the top right to hook the module.
3. In the hooking tool, select "Right column blocks" from the "Hook into" drop-down list.
4. Save your change, then reload the homepage to see the module's block appear. You can then change the module's location by using the Live Edit tool.

## Top horizontal menu <a href="#modulezufront-office-funktionen-tophorizontalmenu" id="modulezufront-office-funktionen-tophorizontalmenu"></a>

Adds a new horizontal menu to the top of your store.

This is an important module: it adds a whole new block at the bottom of the header, where you can display links to the various categories and pages of your shop.\
This is very useful, as it helps your customer quickly find their way through your shop. You can have simple links or menus with sub-menus, thus enabling customers to have a good bird's eye view of your content.

The "Menu top links" section of this module helps you build your menu with links to a selection of pages, categories or to individual products.

## User info block <a href="#modulezufront-office-funktionen-userinfoblock" id="modulezufront-office-funktionen-userinfoblock"></a>

Adds a block that displays information about the customer:

* Link to his or her cart, with a quick view of its content.
* Link to the customer's account.
* Link to log out of the shop.

## Viewed products block <a href="#modulezufront-office-funktionen-viewedproductsblock" id="modulezufront-office-funktionen-viewedproductsblock"></a>

Displays the latest products that a customer has recently consulted. You can set the number of products shown using the "Products to display" field.

## Wishlist block <a href="#modulezufront-office-funktionen-wishlistblock" id="modulezufront-office-funktionen-wishlistblock"></a>

Adds an "Add to my wishlist" link on all product pages. Logged-in customers can then build a wishlist of products from your shop, and send it as a link to their friends. A customer can have many wishlists.

The module also adds a "Wishlist" block on every pages of the shop, which only the customer can see. The block is there so that the customer knows exactly what is in it, and can review it regularly. The block features a "My wishlists" link to access the wishlists management tool.

The module's configuration page enables you to view your customers' lists: simply select a customer in the drop-down list to have the page reload with the chosen customer's lists, then choose a list to display.
