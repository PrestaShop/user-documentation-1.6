# Ce dont vous avez besoin

**Contenu**

* [Ce dont vous avez besoin](ce-dont-vous-avez-besoin.md#Cedontvousavezbesoin-Cedontvousavezbesoin)
  * [Instructions de configuration rapides](ce-dont-vous-avez-besoin.md#Cedontvousavezbesoin-Instructionsdeconfigurationrapides)
  * [Instructions de configuration détaillées](ce-dont-vous-avez-besoin.md#Cedontvousavezbesoin-Instructionsdeconfigurationdétaillées)
    * [Enregistrer un nom de domaine](ce-dont-vous-avez-besoin.md#Cedontvousavezbesoin-Enregistrerunnomdedomaine)
    * [Trouver un hébergeur](ce-dont-vous-avez-besoin.md#Cedontvousavezbesoin-Trouverunhébergeur)
    * [Prérequis techniques](ce-dont-vous-avez-besoin.md#Cedontvousavezbesoin-Prérequistechniques)
    * [Outils](ce-dont-vous-avez-besoin.md#Cedontvousavezbesoin-Outils)
  * [Se préparer](ce-dont-vous-avez-besoin.md#Cedontvousavezbesoin-Sepréparer)

## Ce dont vous avez besoin <a href="#cedontvousavezbesoin-cedontvousavezbesoin" id="cedontvousavezbesoin-cedontvousavezbesoin"></a>

### Instructions de configuration rapides <a href="#cedontvousavezbesoin-instructionsdeconfigurationrapides" id="cedontvousavezbesoin-instructionsdeconfigurationrapides"></a>

Voici une courte de liste de ce dont vous avez besoin pour installer PrestaShop 1.6. Si vous avez besoin de plus de détails, les sections suivantes de cette page devraient répondre à toutes vos questions.

* Prérequis système :\

  * PHP 5.2 ou plus.
    * Réglages utiles (dans le fichier `php.ini`)
      * `allow_url_fopen` activé,
      * `register_globals` désactivé,
      * `magic_quotes_*` désactivé,&#x20;
      * `safe_mode` désactivé,
      * `upload_max_filesize` mis à "16M" ou plus.
    * Extensions PHP utiles (dans le fichier `php.ini`) : PDO\_MySQL, cURL, SimpleXML, mcrypt, GD, OpenSSL, DOM, SOAP.
    * Outils serveur utiles : cron/crontab, Memcached.
  * MySQL 5.0 ou plus.
  * Pour que ça fonctionne mieux :\

    * Hébergeur Unix,
    * Serveur web Apache 1.3 ou plus, ou serveur nginx.
      * Réglages Apache utiles :\

        * `mod_rewrite` activé,
        * `mod_security` désactivé,
        * `mod_auth_basic` désactivé.
    * Au moins 64 Mo de RAM. Plus il y en a, mieux c'est.
* Les codes d'accès à votre serveur FTP et votre base de données MySQL
  * Ils doivent vous être fournis par votre hébergeur si vous ne faites pas une installation locale.
* N'importe quel éditeur de texte.
* N'importe quel client FTP.
* N'importe quel navigateur web moderne (si vous utilisez Internet Explorer : au moins IE8).

Il vous faudra également connaître l'adresse web (le nom de domaine) depuis laquelle vous souhaitez vendre des produits.

Vous pouvez voir les prérequis officiels ici : [http://www.prestashop.com/fr/configuration-requise](http://www.prestashop.com/fr/configuration-requise)

Une fois votre configuration en place, vous pouvez utiliser le guide d'installation : [http://doc.prestashop.com/display/PS16/Installer+PrestaShop](http://doc.prestashop.com/display/PS16/Installer+PrestaShop)

### Instructions de configuration détaillées <a href="#cedontvousavezbesoin-instructionsdeconfigurationdetaillees" id="cedontvousavezbesoin-instructionsdeconfigurationdetaillees"></a>

PrestaShop est une application web : elle ne peut fonctionner qu'une fois installée sur un serveur web, et un nom de domaine est nécessaire pour que vos visiteurs puissent accéder à votre boutique.

#### Enregistrer un nom de domaine <a href="#cedontvousavezbesoin-enregistrerunnomdedomaine" id="cedontvousavezbesoin-enregistrerunnomdedomaine"></a>

Avant de télécharger ou d'installer quoi que ce soir, vous devez offrir un toit à votre boutique en ligne PrestaShop. Pour cela, il vous faut deux composants : un nom de domaine et un hébergement web. Le nom de domaine est l'identifiant en ligne de votre boutique, par exemple, example.fr ou example.qc.ca. C'est la face publique de votre hébergement web, et donc de votre boutique.

Vous devez acheter un nom de domaine pour votre boutique. Il se peut que vous puissiez en obtenir en même temps que vous prenez un hébergement web : de nombreux hébergeurs offrent un nom de domaine pour chaque nouveau compte. Le domaine peut être gratuit pour la première année, ou pour la durée de votre contrat d'hébergement. Le fait de proposer un paquetage complet (nom de domaine + hébergement) peut grandement vous simplifier la vie.

Un problème peut survenir avec les noms de domaine proposés par certains hébergeur : s'il se trouve qu'au bout d'un certain temps vous n'êtes pas satisfait du service de cet hébergeur, vous pourriez vouloir migrer votre boutique chez un meilleur hébergeur. Cela signifie déplacer vos fichiers, vos données, et votre nom de domaine vers cet autre hébergeur.

Les fichiers et données sont faciles à déplacer, mais en fonction de l'hébergeur, vous pourriez avoir du mal à récupérer votre domaine. Étant donné qu'ils l'ont acheté pour vous, techniquement le domaine leur appartient, et ils peuvent soit vous interdire d'héberger le domaine ailleurs, soit vous faire payer durement pour le récupérer. Et étant donné que votre nom de domaine est à la fois votre marque et votre adresse sur le web, vous devrez obéir aux règles de l'hébergeur.

C'est pour il est souvent recommandé de prendre votre nom de domaine chez un "registrar" indépendant (à lire : [http://fr.wikipedia.org/wiki/Bureau\_d%27enregistrement](http://fr.wikipedia.org/wiki/Bureau\_d'enregistrement)). Techniquement, vous n'achetez jamais un nom de domaine, on vous le loue, la plupart du temps pour une cotisation annuelle. Cela vous donne un droit d'utilisation sur ce nom de domaine, mais dès que vous cesserez de payer cette cotisation, il ne vous appartiendra plus et pourra être repris par n'importe qui d'autre. Donc vous payez pour l'enregistrement du nom de domaine en plus de votre hébergement, mais cela vous laisse libre de passer chez un nouvel hébergeur quand vous le souhaiterez, sans frais supplémentaire : changez simplement les adresse DNS du domaine, et dans les 24 heures qui suivent, le nouveau serveur se sera propagé pour le monde entier.

Si vous préférez prendre votre nom de domaine chez un registrar indépendant, en voici quelques-uns de confiance :

* Gandi : [http://www.gandi.net/](http://www.gandi.net/)
* Namecheap : [http://www.namecheap.com/](http://www.namecheap.com/)
* PairNIC: [https://www.pairnic.com/](https://www.pairnic.com/)

Il y en de nombreux autres. Demandez à vos amis !

#### Trouver un hébergeur <a href="#cedontvousavezbesoin-trouverunhebergeur" id="cedontvousavezbesoin-trouverunhebergeur"></a>

Cela signifie que les fichiers de PrestaShop doivent être placés sur un serveur web. Vous en disposez peut-être déjà d'un, mais il est plus probable que vous deviez utiliser un compte chez un hébergeur web (à lire : [http://fr.wikipedia.org/wiki/H%C3%A9bergeur\_web](http://fr.wikipedia.org/wiki/H%C3%A9bergeur\_web)), qui louer de l'espace sur leurs serveurs web au mois ou à l'année.

Avant de créer une boutique en ligne, vous devrez d'abord choisir un fournisseur d'hébergement. Presque tous les hébergeurs peuvent gérer efficacement la solution PrestaShop, mais seulement quelques hébergeurs offrent des serveurs optimisés pour PrestaShop :

*
  * 1&1 dans le monde entier : [1&1](http://www.prestashop.com/es/ecommerce-hosting/1and1)
  * InMotion Hosting dans tous les pays sauf la France et l'Espagne : [InMotion](http://www.inmotionhosting.com/prestashop-hosting)

Consultez [nos hébergeurs partenaires](http://www.prestashop.com/fr/ecommerce-hosting) !

Au moment de choisir un hébergement, retenez un prérequis absolument nécessaire : il doit proposer au moins la version 5.2 de PHP, le langage de programmation avec lequel PrestaShop est écrit, au moins la version 5 de MySQL, le système de base de données avec lequel PrestaShop stocke toutes ses données. Les autres prérequis techniques sont indiqués dans la section "Prérequis techniques" ci-dessous.

PrestaShop S.A. peut héberger votre boutique en ligne ses propres serveurs : notre service PrestaShop Cloud a été conçu afin de libérer les marchands des contraintes techniques, telles que l'installation ou la mise à jour de PrestaShop.

Ce service est complètement gratuite, pour toujours et pour n'importe quelle type de boutique. Elle est particulièrement recommandée pour les projets de boutique qui n'ont que peu d'expérience en matière de site web ou d'ordinateur.

Vous pouvez créer votre compte PrestaShop Cloud directement sur [http://www.prestashop.com](http://www.prestashop.com)!

#### Prérequis techniques <a href="#cedontvousavezbesoin-prerequistechniques" id="cedontvousavezbesoin-prerequistechniques"></a>

PrestaShop est une application qui s'installe sur un serveur web, et est écrit en PHP. Il stocke ses données dans une base de données MySQL

PHP est un langage de programmation open-source, surtout utilisé pour les applications web. Créé en 1995, il est rapidement devenu le langage de programmation le plus utilisé par les développeurs web. Il utilise une syntaxe de type C, ce qui facilite son apprentissage.

MySQL est un système open-source de gestion de base de données. Créé également en 1995, il est rapidement devenu le système de base de données le plus utilisés par les développeurs web. Il repose sur le langage SQL, le langage de base de données le plus utilisé.

Quel que soit le service d'hébergement que vous choisissez, il faut qu'il dispose des composants suivant sur ses serveurs :

* **Système** : Unix, Linux ou Windows. Nous recommandons fortement Unix.
* **Serveur web** : serveur web Apache 1.3 ou plus.
* **PHP 5.2 ou plus** : il se peut que vous dussiez activer PHP 5 sur votre serveur (renseignez-vous auprès de votre hébergeur).
* **MySQL 5.0 ou plus**.
* Au moins 64 Mo de RAM sur votre serveur, voire 128 Mo : plus il y en a, mieux c'est.

Vous trouverez plus d'information dans le guide de l'administrateur système : [http://doc.prestashop.com/pages/viewpage.action?pageId=4096124](http://doc.prestashop.com/pages/viewpage.action?pageId=4096124).

#### Outils <a href="#cedontvousavezbesoin-outils" id="cedontvousavezbesoin-outils"></a>

Il vous faudra deux outils : un éditeur de texte, afin de modifier des fichiers ; et un client FTP, afin de transférer des fichiers depuis votre machine vers votre serveur.

**Éditeur de texte**

Voici quelques éditeurs de texte réputés :

* Windows :
  * Notepad++ : [http://notepad-plus-plus.org/](http://notepad-plus-plus.org/)
  * UltraEdit : [http://www.ultraedit.com/](http://www.ultraedit.com/)
  * Crimson Editor : [http://www.crimsoneditor.com/](http://www.crimsoneditor.com/)
* OS X :
  * Textmate : [http://macromates.com/](http://macromates.com/)
  * Coda : [http://www.panic.com/coda/](http://www.panic.com/coda/)
  * Smultron : [http://www.peterborgapps.com/smultron/](http://www.peterborgapps.com/smultron/)
* Unix/Linux :
  * Vim : [http://www.vim.org/](http://www.vim.org/)
  * Emacs : [http://www.gnu.org/software/emacs/](http://www.gnu.org/software/emacs/)

N'utilisez JAMAIS un logiciel de traitement de texte lorsque vous voulez modifier les fichiers de PrestaShop, comme Microsoft Word ou OpenOffice.org Write.

**Client FTP**

FTP signifie "File Transfer Protocol", c'est à dire la méthode standard pour transférer un fichier depuis un ordinateur vers un hébergeur web, et vice-versa.

Dans ce guide, nous utilisons FileZilla, un client FTP complet et gratuit, disponible sous Windows, OS X et Linux. Vous pouvez le télécharger depuis [http://filezilla-project.org/](http://filezilla-project.org/) et lancez son installeur. A noter : ne téléchargez pas FileZilla Server, uniquement FileZilla Client !

Une fois FileZilla installé, vous devrez le configurer avec les paramètres de connexion de votre serveur web, qui ont dû vous être envoyé par votre hébergeur. Si ce n'est pas le cas, demandez-lui ces informations – ou vérifier votre dossier de courriers indésirables.

Les informations essentielles sont :

* **un nom de domaine** ou **une adresse IP** : là où se trouve le serveur FTP de votre hébergement web.
* **un nom d'utilisateur** : l'identifiant de votre compte chez votre hébergeur, qui vous est unique.
* **un mot de passe** : la nécessaire mesure de sécurité.

Lancez FileZilla, puis ouvrez son Gestionnaire de Sites. Vous pouvez le faire de trois manières différentes :

1. Faites la combinaison de touches Ctrl-S,
2. Cliquez l'icône "Ouvrir le gestionnaire de sites", en haut à gauche,
3. ouvrez le menu "Fichier", et sélectionnez l'option "Gestionnaire de sites..."

Une fenêtre s'ouvre alors.

Pour ajouter un hébergement web au gestionnaire de sites :

1. Cliquez sur le bouton "Nouveau site". Une nouvelle entrée sera créée dans la liste de site. Donnez-lui un nom clair et reconnaissable.
2. Du côté droit, dans l'onglet "Général", saisissez les paramètres que votre hébergeur vous a envoyé : hôte, identifiant, et mot de passe. Vous ne devriez pas avoir à modifier les autres paramètres par défaut, à moins que vous hébergeur vous l'ai expressément demandé.
3. Une fois que tous les champs ont été correctement remplis, cliquez sur le bouton "Connexion". Cela aura pour effet à la fois d'enregistrer votre configuration, et de vous connecter à votre compte, ce qui vous permet de vérifier que toutes les informations saisies sont correctes.

Si FileZilla ne vous convient, voici quelques autres clients FTP réputés :

* Windows :
  * CoreFTP : [http://www.coreftp.com/](http://www.coreftp.com/)
  * WinSCP : [http://winscp.net/](http://winscp.net/)
  * SmartFTP : [http://www.smartftp.com/](http://www.smartftp.com/)
* Mac OS X :
  * Cyberduck : [http://cyberduck.ch/](http://cyberduck.ch/)
  * Transmit : [http://www.panic.com/transmit/](http://www.panic.com/transmit/)
  * Fetch : [http://fetchsoftworks.com/fetch/](http://fetchsoftworks.com/fetch/)
* Unix/Linux :
  * gFTP : [http://gftp.seul.org/](http://gftp.seul.org/)
  * kasablanca : [http://kasablanca.berlios.de/](http://kasablanca.berlios.de/)
  * NcFTP : [http://www.ncftp.com/ncftp/](http://www.ncftp.com/ncftp/)

### Se préparer <a href="#cedontvousavezbesoin-sepreparer" id="cedontvousavezbesoin-sepreparer"></a>

Il vous faut savoir maintenant où vous souhaitez héberger votre boutique PrestaShop. Il y a quatre possibilités vis-à-vis de votre nom de domaine :

* à la racine du domaine : [http://www.example.com/](http://www.example.com/)
* dans un dossier: [http://www.example.com/shop/](http://www.example.com/shop/)
* dans un sous-domaine : [http://store.example.com/](http://store.example.com/)
* dans le dossier d'un sous-domaine : [http://vetemements.example.com/boutique/](http://vetemements.example.com/boutique/)

Notez que grâce à la fonctionnalité multiboutique de PrestaShop 1.5, vous pouvez avoir autant de boutique que vous le souhaitez à partir d'une seule installation de PrestaShop, chacune avec son propre nom de domaine. Vous devriez prendre cela en compte au moment de décider quelques possibilité suivre.

Quel que soit votre plan, la boutique par défaut résidera toujours là où PrestaShop est placé.
