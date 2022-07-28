# Best practices

**Table of contents**

* [Best practices](best-practices.md#Bestpractices-Bestpractices)
  * [Thinking ahead](best-practices.md#Bestpractices-Thinkingahead)
  * [Designing in Photoshop](best-practices.md#Bestpractices-DesigninginPhotoshop)
  * [Usability](best-practices.md#Bestpractices-Usability)
  * [Optimizing images](best-practices.md#Bestpractices-Optimizingimages)
  * [Key SEO tips](best-practices.md#Bestpractices-KeySEOtips)

## Best practices <a href="#bestpractices-bestpractices" id="bestpractices-bestpractices"></a>

There are a few steps you can take, from designing your theme in Photoshop to optimizing you code for search engines, which have been established as being the must-do for theme development. Following these best practices will help you build a better theme.

### Thinking ahead <a href="#bestpractices-thinkingahead" id="bestpractices-thinkingahead"></a>

Before opening Photoshop, GIMP or any other graphic editor, you should sit at a desk with a pen and a sheet paper, and think of the map/hierarchy for your shop, making it as flexible as possible (not all shops have the same amount of categories, or of products per category).

A complete PrestaShop theme requires at least 30 pages or page sections:

* Home page
* Category page
* Product page
* Product comparison page
* Search results page
* "My Account" and its inner pages:
  * My vouchers
  * Orders history
  * Personal information
* "My Cart"
* Authentication page
* Account creation
* Checkout pages:
  * Addresses list
  * Shipping costs
  * Payment choice (check, bank transfer)
  * One page checkout
* Address creation
* Delivery page
* Maintenance page
* Manufacturers list and single manufacturer page
* Suppliers list and single supplier page
* The 404 page ("Page not found")
* "Best sales" page
* "New products" page
* "Current promotions" page
* "Forgotten password" page
* Legal notice
* Sitemap
* Stores page
* Contact form

Please do take all these into account, so as to not forget any. Failing to take some page into account may result in an incomplete theme, and thus a bad experience for your users.

In truth, these 30 files just make sure you scratch the surface. To get a better sense of the pages you should take into account, dive into the default theme, located in the `/themes/default` folder. It has no less than 60 template files, not mentioning the CSS, JavaScript and image files, along with the mobile version (in the `/themes/default/mobile` folder) which has its own set of 58 template files, along with its own CSS, JavaScript and image files.

Once you feel good about your shop's hierarchy and mandatory template files, make a few sketches of the interface, in order to get a feel of where the various elements will be placed: new products, promotions, pictures, text, etc.). Also, include the important details, such as the various mentions on the product's page: on sale, promotion, new product, stricken price...).

Of course, these are just general tips; some professional might prefer to do it all directly in Photoshop, and then jump right into PHP/Smarty, HTML and CSS.

### Designing in Photoshop <a href="#bestpractices-designinginphotoshop" id="bestpractices-designinginphotoshop"></a>

You are seldom alone when creating a theme: whether a colleague or a client, there are many occasions when you will have to share your design with other people. You should therefore make it easy for them to work with it out-of-the-box.

One of the first thing to do is to provide a work in the RGB color space, in 72 dpi, and to always provide the non-flattened file (unless it is for the final client, in which case you should provide the flattened one, unless he paid for the non-flattened version explicitly).\
In general, you should never flatten a design, unless you are certain you are never going to want to edit it again.

When building a PrestaShop theme, you should work with a 980px width and, depending on your uses, with:

* One Photoshop folder for all text layers, so that web developers can easily access the design.
* One Photoshop folder per design block (new products, best sales, etc.).

#### Color space <a href="#bestpractices-colorspace" id="bestpractices-colorspace"></a>

Always rely on RGB. Do not ever use CMYK, which is made for print.

#### Units <a href="#bestpractices-units" id="bestpractices-units"></a>

When designing for the Web, the base unit is the pixel. Do not measure in picas, points or centimeters.

#### Font <a href="#bestpractices-font" id="bestpractices-font"></a>

Do not use atypical fonts! Keep it readable at all times!

Standard text (title, sub-title, regular text) should be limited to the following fonts, in order to insure that all visitors can see the same thing:

* Arial
* Verdana
* Helvetica
* Georgia
* Tahoma

Keep the number of fonts to the bare minimum, for fear of making your website confusing and unreadable.

Of course, you can use any font you like when designing a graphic, such as the header image or a slide-show picture.

#### Font size <a href="#bestpractices-fontsize" id="bestpractices-fontsize"></a>

Never forget that the user has the final say on the text size, since modern browsers can increase or decrease it at the touch of a keyboard key.\
As a matter of fact, you should test your website with various browser variations, see how easy it is break your design... and therefore rework your design in order to avoid such easy breakage.

You may start off with a handful of basic text sizes:

* Titles: 18px.
* Smaller titles: 14px.
* Regular text: 10 to 12px.

#### Transparency <a href="#bestpractices-transparency" id="bestpractices-transparency"></a>

Transparent images do not work well with older browsers, particularly with Internet Explorer, so you should stay away from 24-bits PNG images. As for GIF images with transparency, use the over a plain background to ensure they work properly. Avoid 50% opacity by using the same matte color as the website's background color.

#### Miscellaneous <a href="#bestpractices-miscellaneous" id="bestpractices-miscellaneous"></a>

* Test your theme with all of PrestaShop's options activated, so as to see how the theme reacts.
* Edit a product in order to see how the various options influence your design (promotion, new product, etc. …)... if it does at all.
* Make sure to have a homogeneous style for your shop.

### Usability <a href="#bestpractices-usability" id="bestpractices-usability"></a>

We won't delve into complex human–computer interaction theories here, but rather try to make sure that your shop is accessible to as many potential customers as possible. Your ultimate goal should be to have visitors trust your shop enough so that they start buying.

Every time a visitor stumbles upon a usability problem, your site loses their trust. Ultimately, if the trust reaches a low point, frustration comes and the visitor leaves your site, without buying anything of course. Such is the importance of usability in the e-commerce world.

When designing your shop's theme, keep in mind that its mission (in addition to selling goods, of course) is to show your visitors that your website is managed by serious and competent people.

#### The home page <a href="#bestpractices-thehomepage" id="bestpractices-thehomepage"></a>

This is **the** most important page of your shop, the one where it is "hit or miss". This is the page where the visitor will get a general opinion of your shop, and decide if she should trust you with her money.

You should make sure to make your shop easily recognizable, and have your catalog be the first thing people see.

The website's header is where you will be able to put the most recognizable details: logo, name, unique image... It should be not be higher than 250px, so that your visitors can reach your catalog without resorting to scrolling down the page. In other words, your main content should never be below the fold (to learn more about the Fold, read this Wikipedia page: [http://en.wikipedia.org/wiki/Above\_the\_fold](http://en.wikipedia.org/wiki/Above\_the\_fold)).

The visual aspect of your website is of course very important (hence our "Thinking ahead" section above): you must find way to put your products forward with overloading the page. Moreover, you should use homogeneous colors and layout within a page and between pages. For instance, if a button has an interaction effect on one page, make sure to apply that effect to all other pages on the site.

The search engine must be easy to find. Visitors often know what they came for, and don't want to browse through categories and sub-categories in search for it.

Still, when building your website's content, think of the user who browse categories, and make them simple and intuitive.

You can reinforce the perceived trust by displaying logos or mentions of your partners (banks, carriers), and your rating from a known e-commerce institution, such as FIA-NET in France.

Do display your contact details, such as phone number or chat system, if available. It will show you are real, and that can make a huge difference.\
&#x20;Of course, do not use your personal phone number: they need to feel they are calling a company's support team, not disturbing you while you cook.

Clearly display your Return Merchandise conditions, your general T\&C and other applicable laws that you respect.

#### The product page <a href="#bestpractices-theproductpage" id="bestpractices-theproductpage"></a>

A visitor only comes to the product page if she's interested by said product, and wants more details. There should therefore be aplenty of those.

Make the "Add to Cart" button clear and visible. It must distinguish itself from the rest of the layout, by both its size and color – but do keep a homogeneous design: if the button is too far off from the general design, the visitor can just as easily not see it, in the same way people have trained themselves not to see ads on the Internet.

Make sure to display all the relevant labels: "New product", "Promotion", "Voucher", etc. Also, do not forget to add the delivery delays.

#### The conversion funnel: "My Account" and related pages <a href="#bestpractices-theconversionfunnel-myaccount-andrelatedpages" id="bestpractices-theconversionfunnel-myaccount-andrelatedpages"></a>

The conversion funnel is where your visitors become client (hence the use of "conversion", or sometimes "transformation"). If these pages are badly designed or structured, this can mean the loss of many potential clients, and therefore all the order they would have made on your site. To learn more about the conversion funnel, read this Wikipedia page: [http://en.wikipedia.org/wiki/Conversion\_funnel](http://en.wikipedia.org/wiki/Conversion\_funnel).

**Account creation / "My Account"**

The default PrestaShop theme comes with an account form that gives a very good transformation percentage. But it might still not suit your own site's needs. Hence, here are a few tips to follow if you intend to update the form.

* Be basic, keep the essential only. The visitor must concentrate on the account creation, and the purchase. See how Amazon does it.
* Reduce the number of steps. The user must know how many steps she still has to go through before she can actually finalize her purchase.
* Clearly display any mistake the user makes, right next to form field. Errors should be displayed in a distinct color (red is a favorite), and mandatory fields should indicated (with an asterisk \*, for instance).

**Payment**

The visitor has created her client account, great! But it's still not over yet, she must now go through the purchase itself.

Same as for the account creation form:

* Reduce the number of steps (delivery address, payment page).
* Display the errors in a distinct color.
* Payment page:
  * If the visitor uses a credit card, warn them that they will be redirected to your bank's secure server. For instance, add a little padlock icon, with an explanation.
  * If she chooses to pay by check (or any other offline payment method), clearly mention what to do next: amount, address, etc.

All these usability tips are just part of the whole story, but they can bring you a solid ground on which building your theme, in order to improve your shop.

### Optimizing images <a href="#bestpractices-optimizingimages" id="bestpractices-optimizingimages"></a>

One important thing to keep in mind is that images slow a shop down, especially if the images are not optimized. This section shows you how to optimize images, but at the end of the end, the optimization is to only keep the important images, and let go of the others.\
There are just a few important images on a shop theme: the products images/thumbnails, the shop's logo or header, and maybe the homepage's slideshow. Most of the rest can be easily replaced by clever use of CSS and HTML, especially if it belongs to the shop's design. Keep the number of images on any page to a minimum: the faster a shop will be, the longer a potential customer will be willing to browser its page.

Image optimization means two things:

* Lowering image size in order to improve loading time.
* Making sure they are properly indexed by search engines.

Dealing with image size should be done directly in Photoshop: do not ever use a bigger image than it is displayed within the browser. Use the necessary size, no more, no less.\
Photoshop also has a special "Save for the web" tool, which helps you perform compression and format comparison, and will remove much of the data cruft.

There are also online tools which can help you optimize your pictures with loss of quality, by performing safe automatic tasks:

* Yahoo! [Smush.it](http://smush.it) is the most well-know: [http://www.smushit.com/ysmush.it/](http://www.smushit.com/ysmush.it/)
* Kraken is another which at times can give better results, and has Firefox and Chrome extensions: [http://kraken.io/](http://kraken.io/)
* Image Optimizer enables you to also change the size of the file: [http://www.imageoptimizer.net/](http://www.imageoptimizer.net/)

If you are at ease with command line tools, you can use these:

* Pngnq: converts 24-bit PNG files into 6 to 8-bit ones, by only keeping the needed colors.\
  Download: [http://pngnq.sourceforge.net/](http://pngnq.sourceforge.net/)\
  Sample command line: `pngnq -vf -s1 image.png`
* OptiPNG: tests several compression methods on a PNG file in order to find the best one.\
  Download: [http://optipng.sourceforge.net/](http://optipng.sourceforge.net/)\
  Sample command line: `optipng -o7 image-nq8.png`
* pngcrush: another PNG optimization tool.\
  Download: [http://pmt.sourceforge.net/pngcrush/](http://pmt.sourceforge.net/pngcrush/)\
  Sample command line: `pngcrush image.png -rem all -reduce -brute result.png`
* jpegtran: performs lossless operations on JPEG images.\
  Download: [http://jpegclub.org/jpegtran/](http://jpegclub.org/jpegtran/)\
  Sample command line: `jpegtran -copy none -optimize -perfect src.jpg dest.jpg`

### Key SEO tips <a href="#bestpractices-keyseotips" id="bestpractices-keyseotips"></a>

Improving your site ranking is key to getting new clients. While we will not dive into SEO in this section, there is a handful of tips you should strive for:

* Improve your URL's, title and other meta tags: make sure to fill all the textfields in the back office, both for products and for categories. Use short and concise descriptions; fill the title with the most important details in order to have these details appear in the URL, etc.
* Improve your image display: use proper captions and titles.
* Do not hesitate to use HTML lists when naming the various components/features of a product.
* Use important words multiple times in the product description.
* Put important text forward using \<strong> and \<em>.
* Optimize page display: make sure they load quickly, either by minimizing image size or by using a better web-host.

See also PrestaShop free guide on SEO: [http://www.prestashop.com/en/white-paper-seo](http://www.prestashop.com/en/white-paper-seo)
