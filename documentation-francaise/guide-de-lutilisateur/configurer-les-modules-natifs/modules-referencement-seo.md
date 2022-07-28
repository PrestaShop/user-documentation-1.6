# Modules Référencement - SEO

## Google sitemap <a href="#modulesreferencement-seo-googlesitemap" id="modulesreferencement-seo-googlesitemap"></a>

Ce module vous permet de créer un sitemap pour votre magasin, et de le garder à jour.

Afin d'optimiser votre référencement, il est essentiel d'avoir un fichier sitemap, qui est un fichier XML répertoriant tous les produits et les pages de votre boutique. Ce fichier permettra aux moteurs de recherche d'indexer toutes les pages facilement et efficacement. Vos produits apparaissent alors parfaitement dans les moteurs de recherche quand un visiteur effectue une recherche. Vous pouvez créer un sitemap pour PrestaShop, et être indexé par tous les moteurs de recherche qui prennent en charge le format de fichier (Google, Yahoo, Bing, ...), en utilisant des outils tels que Webmaster Tools de Google. Une fois installé, cliquez sur le lien "Configurer".

La page de configuration a peu d'options :

* **Le sitemap inclut également les produits des catégories inactives**. Vous devez décider s'il faut ou non afficher les produits que vous n'avez pas activés dans votre boutique. Si vous souhaitez utiliser tous les produits, cochez la case "Le sitemap inclut également les produits des catégories inactives". Les produits inactifs seront ensuite indexés par Google afin que vous puissiez les rendre visibles dès que vous les remettez en ligne.
* **Le sitemap inclut également les pages CMS qui ne sont pas dans un bloc de CMS**. De même, vous voudrez peut-être que le plan du site contienne également les pages CMS qui ne sont pas directement disponibles

Une fois que vous avez fini de configurer le module, cliquez sur "Mettre à jour fichier sitemap". Vous avez alors l'adresse du sitemap (par exemple, [myprestashop.com/sitemap.xml](http://myprestashop.com/sitemap.xml)). Copiez cette URL pour l'enregistrer dans votre compte Google Webmaster Tools. Le module affichera alors la taille du fichier et le nombre de pages indexées. N'oubliez pas de le mettre à jour régulièrement afin que les moteurs de recherche indexent parfaitement votre contenu.

La dernière section de la page de configuration donne un lien cron. Un bon sitemap doit être régulièrement mis à jour, et à moins d'être prêts à cliquer sur le bouton "Mettre à jour fichier sitemap" à chaque fois qu'il y a un changement sur votre boutique, vous pouvez faire en sorte que votre serveur fasse le travail pour vous. Créez une tâche cron avec l'URL donnée, et vous n'aurez plus jamais à vous faire du souci à ce sujet.\
&#x20;Si vous ne savez pas ce qu'est une tâche cron, demandez à votre hébergeur.
