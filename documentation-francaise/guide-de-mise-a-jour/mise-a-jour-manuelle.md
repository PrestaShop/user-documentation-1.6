# Mise à jour manuelle

**Contenu**

* [Mise à jour manuelle](mise-a-jour-manuelle.md#Miseàjourmanuelle-Miseàjourmanuelle)
  * [L'essentiel](mise-a-jour-manuelle.md#Miseàjourmanuelle-L%27essentiel)
  * [Première étape – Enregistrer et sauvegarder la boutique actuellement en ligne](mise-a-jour-manuelle.md#Miseàjourmanuelle-Premièreétape–Enregistreretsauvegarderlaboutiqueactuellementenligne)
  * [Deuxième étape – Se préparer pour la nouvelle version](mise-a-jour-manuelle.md#Miseàjourmanuelle-Deuxièmeétape–Sepréparerpourlanouvelleversion)
  * [Troisième étape – Lancer la mise à jour locale](mise-a-jour-manuelle.md#Miseàjourmanuelle-Troisièmeétape–Lancerlamiseàjourlocale)
  * [Quatrième étape – tests et assurance qualité](mise-a-jour-manuelle.md#Miseàjourmanuelle-Quatrièmeétape–testsetassurancequalité)
  * [Cinquième étape – Lancer la mise à jour sur votre hébergement web](mise-a-jour-manuelle.md#Miseàjourmanuelle-Cinquièmeétape–Lancerlamiseàjoursurvotrehébergementweb)
  * [Sixième étape – tests et assurance qualité](mise-a-jour-manuelle.md#Miseàjourmanuelle-Sixièmeétape–testsetassurancequalité)
  * [Septième étape – Relancer votre boutique mise à jour](mise-a-jour-manuelle.md#Miseàjourmanuelle-Septièmeétape–Relancervotreboutiquemiseàjour)

**CETTE MÉTHODE EST DÉSORMAIS DÉCONSEILLÉE.**\
**VEUILLEZ UTILISER LE MODULE GRATUIT** [**1-CLICK UPGRADE**](http://addons.prestashop.com/fr/outils-administration-modules-prestashop/5496-1-click-upgrade-autoupgrade.html)**.**

Lisez la [documentation sur la mise à jour automatique](http://doc.prestashop.com/pages/viewpage.action?pageId=11272345), la seule méthode officiellement conseillée.

## Mise à jour manuelle <a href="#miseajourmanuelle-miseajourmanuelle" id="miseajourmanuelle-miseajourmanuelle"></a>

La mise à jour manuelle est un processus long et détaillé, auquel vous ne devriez faire appel qu'en cas de nécessité – notamment si vous ne pouvez pas faire de mise à jour automatique.

De fait, les mises à jour manuelles sont à réserver aux experts, ceux qui connaissent les outils de développement web comme WAMP, phpMyAdmin, etc. Si ce n'est pas votre cas, demandez à un ami ou payez un développeur pour vous assister. Prévoyez une ou deux heures, peut-être plus : prenez le temps de bien faire.

Le principe de la mise à jour manuelle est simple : plutôt que de prendre le risque de mettre directement à jour votre boutique en ligne, tout le travail se déroule sur votre ordinateur, grâce à un serveur PHP/MySQL local comme WAMP ou XAMPP. Une fois la mise à jour locale réussie, il faut refaire ce processus en ligne.

Toute la durée du processus, votre boutique en ligne sera désactivée (en mode "maintenance") afin de s'assurer que vos clients ne perdront pas leurs paniers et achats lors de la mise en jour. Dans les faits, cela signifie que votre boutique sera fermée et inaccessible pendant l'intégralité du processus (une à deux heures).

### L'essentiel <a href="#miseajourmanuelle-lessentiel" id="miseajourmanuelle-lessentiel"></a>

Cette courte section est réservée à ceux qui sont déjà habitués à l'installation d'applications PHP-MySQL sur un serveur. Si le manque de détail vous gêne, vous trouverez des instructions détaillées dans les sections qui suivent.

Une grande partie du processus se déroule au sein d'un serveur web installé sur votre ordinateur. Avant de vous lancer, téléchargez et installez le serveur local de votre choix : WAMP, XAMPP, EasyPHP, MAMP, ou autre. Si vous n'avez jamais installé de serveur local, lisez le chapitre "Ce dont vous avez besoin" du Guide de Démarrage, section "Installer PrestaShop sur votre propre ordinateur" : [http://doc.prestashop.com/display/PS15/Ce+dont+vous+avez+besoin#Cedontvousavezbesoin-InstallerPrestaShopsurvotrepropreordinateur](http://doc.prestashop.com/display/PS15/Ce+dont+vous+avez+besoin#Cedontvousavezbesoin-InstallerPrestaShopsurvotrepropreordinateur) .

Les étapes de la mise à jour de PrestaShop :

1. Enregistrer et sauvegarder la boutique actuellement en ligne :
   * Désactivez votre boutique (page "Maintenance" du menu "Préférences").
   * Sauvegardez vos fichiers sur votre PC, en utilisant votre client FTP, dans un dossier "prestashop-prod". C'est une copie fidèle de votre site en production
   * Sauvegardez votre base de données (page "Paramètres avancés / Sauvegarde BDD", ou en passant par phpMyAdmin).
   * Sauvegardez votre traduction sur mesure ("Export d'une langue" dans la page "Localisation / Traductions").
2. Se préparer pour la nouvelle version :
   * Téléchargez la dernière version de PrestaShop ([http://www.prestashop.com/fr/telechargement](http://www.prestashop.com/fr/telechargement)), et décompressez-la vers le dossier "prestashop-prep".
   * Copiez vos fichiers personnels (images, logos, photos, traductions, modules, etc.) depuis "prestashop-prod" vers le dossier "prestashop-prep" de votre ordinateur. Une liste détaillée se trouve plus loin dans ce guide.
   * Copiez le dossier "prestashop-prep" dans le dossier web de votre serveur local (`/htdocs`, `/www` ou un autre nom en fonction du serveur utilisé). C'est dans ce dossier que se fera la mise à jour, laissant intacts votre sauvegarde principale (prestashop-prod) et vos fichiers préparés (prestashop-prep).
   * Recréez la base de données de production sur votre serveur local : à l'aide phpMyAdmin, créez une base de données, dans laquelle vous mettrez les données de votre boutique de production, à partir des fichiers SQL sauvegardés au début du processus.
3. Lancer la mise à jour localement :
   * Lancez le script de mise à jour sur votre serveur local, en y accédant avec votre navigateur. Dans la version 1.6, le script est situé à l'adresse `/install/upgrade/upgrade.php`.
   * Vérifiez tous les paramètres avant la mise à jour : suivez les instructions à l'écran et assurez-vous que votre serveur est conforme aux exigences techniques de la nouvelle version.
   * Fin de la mise à jour : une fois la mise à jour terminée, supprimez le dossier `/install` et rendez-vous sur votre front-office et votre back-office pour vous assurer que tout fonctionne.
4. Tests et assurance qualité :
   * Importez vos traductions (section "Importez un pack de langue manuellement" dans la page "Traduction", dans le menu "Localisation").
   * Vérifiez que votre thème fonctionne toujours comme prévu. Si ce n'est pas le cas, vous devrez modifier ses fichiers.
   * Testez votre boutique en détail : créez des comptes, achetez des produits, annulez des commandes, vérifiez les factures, etc.
5. Lancer la mise à jour sur votre hébergement web :
   * À l'aide de votre client FTP, remplacez les fichiers de votre boutique en ligne par ceux de votre dossier "prestashop-prep".
   * Lancez le script de mise à jour sur votre boutique en production, en y accédant avec votre navigateur. Dans la version 1.6, le script est situé à l'adresse `/install/upgrade/upgrade.php`.
   * Vérifiez tous les paramètres avant la mise à jour : suivez les instructions à l'écran et assurez-vous que votre serveur est conforme aux exigences techniques de la nouvelle version.
   * Fin de la mise à jour : une fois la mise à jour terminée, supprimez le dossier `/install` et rendez-vous sur votre front-office et votre back-office pour vous assurer que tout fonctionne.
6. Tests et assurance qualité :
   * Importez vos traductions (section "Importez un pack de langue manuellement" dans la page "Traduction", dans le menu "Localisation").
   * Vérifiez que le nom de domaine principal est correct (page "Préférences / SEO & URLs", section "URL de la boutique").
   * Régénérez votre fichier robots.txt (page "Préférences / SEO & URLs", section "Génération du fichier robots.txt").
   * Vérifiez que votre thème fonctionne toujours comme prévu. Si ce n'est pas le cas, vous devrez modifier ses fichiers.
   * Testez votre boutique en détail : créez des comptes, achetez des produits, annulez des commandes, vérifiez les factures, etc.
7. Lancez votre boutique mise à jour :
   * Activez votre boutique (page "Maintenance" du menu "Préférences").

C'est fait ! Découvrez toutes les nouvelles fonctionnalités de cette mise à jour !

### Première étape – Enregistrer et sauvegarder la boutique actuellement en ligne <a href="#miseajourmanuelle-premiereetape-enregistreretsauvegarderlaboutiqueactuellementenligne" id="miseajourmanuelle-premiereetape-enregistreretsauvegarderlaboutiqueactuellementenligne"></a>

Attention

Ne pas sauvegarder votre boutique vous fait prendre un risque très important si vous rencontrez des difficultés avec la mise à jour. Vous pourriez perdre vos données et ne jamais les récupérer

**Ne jamais sauter cette étape**. Ne passez pas à l'étape 2 sans être absolument certain que vos sauvegardes ont été effectuées avec succès, et sont entièrement fonctionnelles. Faites autant de tests et vérifications que possible.

#### Désactiver votre boutique <a href="#miseajourmanuelle-desactivervotreboutique" id="miseajourmanuelle-desactivervotreboutique"></a>

Il est **très important** de désactiver votre boutique.\
&#x20;En la désactivant, vous vous assurez qu'il n'y a pas d'activité sur votre boutique tandis que vous la mettez à jour. Par conséquent, si jamais vous avez à revenir à annuler la mise à jour en revenant une sauvegarde, même très récente, vous n'aurez pas perdu de commandes ou de paniers en cours de remplissage.

Allez dans le back-office de votre boutique, ouvrez la page "Maintenance" depuis le menu "Préférences", puis choisissez "Non" pour l'option "Activer la boutique".

Si vous mettez à jour depuis PrestaShop 1.4, ce réglage est directement disponible depuis l'onglet "Préférences".

Dans le champ "IP de maintenance", situé juste en dessous de la case "Activer la boutique", saisissez votre propre adresse IP, de sorte que vous pouvez continuer à utiliser le front-office de votre boutique lors de la mise à jour. Cela vous permettra de tester la boutique, tout en faisant en sorte que des visiteurs ne puissent pas accéder au site Web.\
&#x20;Afin de connaître votre adresse IP, rendez-vous sur cette page : [http://www.mon-ip.com/](http://www.mon-ip.com/)

#### Sauvegarder vos fichiers <a href="#miseajourmanuelle-sauvegardervosfichiers" id="miseajourmanuelle-sauvegardervosfichiers"></a>

Vous devez récupérer tous les fichiers de votre boutique PrestaShop pour les stocker sur votre ordinateur.

Il y a principalement deux manières de les enregistrer :

* **Demandez à votre hébergeur de le faire pour vous**.\
  &#x20;Assurez-vous qu'il s'agit d'une sauvegarde pleinement fonctionnelle, récente, et surtout qu'elle reflète pleinement le contenu de votre boutique actuelle.

...ou...

* **Copiez tous vos fichiers depuis votre hébergement vers votre ordinateur à l'aide d'un client FTP**.\
  &#x20;Cette méthode n'est possible que si votre hébergeur vous donne accès à votre serveur FTP. Créer un dossier "prestashop-prod" sur le Bureau de votre ordinateur, puis à l'aide d'un client FTP (tel que FileZilla, que vous pouvez télécharger sur [http://filezilla-project.org/](http://filezilla-project.org/)), sélectionnez tous les fichiers et dossiers de PrestaShop sur votre serveur (utilisez le raccourcis clavier Ctrl-A) et copiez-les dans votre dossier "prestashop-prod".

#### Sauvegarder votre base de données <a href="#miseajourmanuelle-sauvegardervotrebasededonnees" id="miseajourmanuelle-sauvegardervotrebasededonnees"></a>

Vous devez absolument faire une sauvegarde de toute la base de données de votre boutique PrestaShop.

Il y a trois manières de réaliser cette sauvegarde :

* **Demandez à votre hébergeur de la faire pour vous**.\
  &#x20;Assurez-vous qu'il s'agit d'une sauvegarde pleinement fonctionnelle, récente, et surtout qu'elle contient bien toutes les données de votre boutique actuelle.

...ou...

*   **Téléchargez une sauvegarde depuis le back-office de PrestaShop**.\
    Ouvrez la page "Sauvegarde BDD", puis suivez les instructions sur la page.

    Cette page se trouve :

    * PrestaShop 1.4 : dans l'onglet "Outils", sous-onglet "Sauvegarde BDD".
    * PrestaShop 1.5 et + : dans le menu "Paramètres avancés", page "Sauvegarde BDD".

    Le processus entier peut prendre entre 1 et 20 minutes, en fonction de la taille de votre base de données, après quoi vous verrez un lien apparaître sur la page, "Téléchargez le fichier de sauvegarde (_taill_)". Cliquez-le, et assurez-vous que la sauvegarde est fonctionnelle, récente, et surtout qu'elle contient bien toutes les données de votre site web. Ouvrez le fichier zip et vérifiez qu'il n'y a absolument AUCUNE ERREUR dans le fichier `.sql` avant de continuer le processus de mise à jour.

...ou...

* **Téléchargez une copie de vos données en passant par phpMyAdmin**.\
  &#x20;Assurez-vous que votre base de données est fonctionnelle, récente, et surtout qu'elle contient toutes les données de votre boutique PrestaShop. Si votre base de données est trop volumineuse, il se peut que phpMyAdmin vous renvoie une erreur. Dans ce cas, passez par votre hébergeur.

Conservez ce fichier dans le dossier "prestashop-prod" de votre ordinateur, que vous devez avoir créé à l'étape précédente et qui devrait déjà contenir vos fichiers.

#### Sauvegarder vos traductions personnalisées <a href="#miseajourmanuelle-sauvegardervostraductionspersonnalisees" id="miseajourmanuelle-sauvegardervostraductionspersonnalisees"></a>

Si vous n'avez pas modifié les traductions, ni ajouté de nouvelles traductions (que ce soit pour PrestaShop ou vos modules), passez directement à l'étape suivante.

Pour conserver vos modifications de traduction :

1.  Rendez-vous dans la page "Traductions" votre back-office.

    Cette page se trouve :

    * PrestaShop 1.4 : dans l'onglet "Outils", sous-onglet "Traductions".
    * PrestaShop 1.5 et + : dans le menu "Localisation", page "Traductions".
2. Dans la section "Exporter des traductions", sélectionnez la langue dans laquelle vous avez fait vos modifications, puis sélectionnez le thème actuel, et cliquez sur "Exporter".
3. Enregistrez le fichier téléchargé dans le dossier "prestashop-prod" sur votre ordinateur.

Répétez ce processus pour toutes les langues que vous avez personnalisé, que ce soit celles que vous avez créé/ajouté et celle que vous avez modifié/corrigé.

Vérifiez vos dossier de sauvegarde&#x20;

Le dossier "prestashop-prod" contient-il...

* ...une copie complète de tous les fichiers de votre boutique actuellement en production ?
* ...une copie complète et sans erreur de votre base de données, sous forme d'une fichier `.sql` ?
* ...une copie de vos traductions personnalisées (facultatif) ?

Vous devez avoir vérifié l'intégralité de votre dossier de sauvegarde, et fait en sorte que tout y soit correct et que, au besoin, vous pourrez récupérer vos données.

Si vous avez répondu oui à toutes les questions ci-dessus, passez à l'étape 2.

### Deuxième étape – Se préparer pour la nouvelle version <a href="#miseajourmanuelle-deuxiemeetape-sepreparerpourlanouvelleversion" id="miseajourmanuelle-deuxiemeetape-sepreparerpourlanouvelleversion"></a>

#### Télécharger et décompresser la dernière version de PrestaShop <a href="#miseajourmanuelle-telechargeretdecompresserladerniereversiondeprestashop" id="miseajourmanuelle-telechargeretdecompresserladerniereversiondeprestashop"></a>

Rendez-vous sur [http://www.prestashop.com](http://www.prestashop.com) et téléchargez la dernière version de PrestaShop (cliquez sur le bouton "Téléchargement", remplissez le formulaire, et validez).

Vous devriez obtenir un fichier sous la forme `prestashop_1.5.x.zip` (où "x" est un chiffre du numéro de version).

Décompressez ce fichier zip sur votre ordinateur, et placez son contenu dans un dossier "prestashop-prep" que vous aurez créé sur votre ordinateur, au même niveau que le dossier "prestashop-prod" (par exemple, votre Bureau). C'est dans ce dossier que vous préparerez vos fichiers à la mise à jour.\
&#x20;Attention : faites en sorte de ne pas avoir le dossier `/prestashop` à la racine du dossier "prestashop-prep"; mais bien directement tous les fichiers et sous-dossiers qu'il contient, afin d'avoir le même aperçu du contenu des dossiers "prestashop-prod" et "prestashop-prep".

Si vous n'avez pas d'outil de décompression, vous pouvez en télécharger un gratuit ici : [http://www.7-zip.org/](http://www.7-zip.org/).

Dans ce dossier "prestashop-prep", sélectionnez le dossier `/admin` et donnez-lui le même nom que le dossier admin de votre boutique de production. Par exemple, si le dossier "prestashop-prod" contient un sous-dossier `/admin123`, donnez le même nom au sous-dossier `/admin` du dossier "prestashop-prep".

#### Copier dans "prestashop-prep" les fichiers qui ont été sauvegardés dans "prestashop-prod" <a href="#miseajourmanuelle-copierdans-prestashop-prep-lesfichiersquiontetesauvegardesdans-prestashop-prod" id="miseajourmanuelle-copierdans-prestashop-prep-lesfichiersquiontetesauvegardesdans-prestashop-prod"></a>

Vient maintenant le moment où vous allez copier les fichiers propres à votre installation de production au sein des fichiers de la nouvelle version. Dans les faits, l'objectif est d'aboutir à un dossier "prestashop-prep" contenant la dernière version des fichiers standards de l'installation, ainsi que tous les fichiers que vous avez mis en ligne depuis que vous avez installé PrestaShop : images, logos, photos, traductions, modules, etc.\
&#x20;C'est une étape importante, qui vous permet de conserver toutes les personnalisations de votre boutique. Prenez le temps de suivre les instructions.

Il va donc vous falloir parcourir les fichiers et dossiers sauvegardés dans le dossier "prestashop-prod" afin de les copier dans le dossier "prestashop-prep".\
&#x20;Choisissez "Oui" chaque fois que le système vous demandera s'il doit remplacer le fichier original par la copie.

Les dossiers suivants doivent être copiés depuis votre dossier "prestashop-prod" vers le dossier "prestashop-prep" :

* **`/mails`**. Contient tous les modèles de mails, dont ceux que vous avez modifiés.\
  &#x20;Si vous n'avez jamais modifié vos modèles de mails, ne copiez pas ce dossier.
* **`/img`**. Contient votre logo et toutes les images de votre boutique (catégories, produits, etc.). Prenez surtout soin de copier ces fichiers et dossiers :
  * `logo.jpg` - le logo de votre boutique
  * `favicon.ico` - le favicon de votre boutique
  * `logo_stores.gif` - le logo de votre boutique pour la carte de l'outil de découverte de magasins
  * `/c` - les images de vos catégories
  * `/cms` - les images de vos pages CMS
  * `/co` - les textures de couleur de vos attributs
  * `/m` - les logos de vos marques/fabricants
  * `/p` - les photos de vos produits
  * `/scenes` - les image-maps/scènes de vos catégories
  * `/st` - les photos de vos magasins physiques
  * `/su` - les logos de vos fournisseurs
  * ...en définitive, copiez tous les dossiers du dossier `/img`, sauf `/img/admin` et `/img/jquery-ui`.
* **`/modules`**. Ne copiez que les modules que vous avez ajoutés depuis que vous avez installé PrestaShop la première fois (et qui ne font donc pas partie de l'installation par défaut).
  * Certains de ces modules peuvent ne plus être actuellement activés ou installés : à vous de déterminer s'il peut vous être utile de les avoir sur votre installation mise à jour.
  * Notez également qu'il vous faudra peut-être mettre à jour les modules qui n'ont pas été conçus pour cette nouvelle version.
* **`/themes/votreTheme`**. Ne copiez que votre propre thème.
  * Si vous utilisez le thème par défaut de PrestaShop (non modifié), ne copiez pas son dossier (`/themes/prestashop`) : vous devriez utiliser le thème par défaut de la nouvelle version (`/themes/default`).
  * Si vous utilisez une version modifiée du thème par défaut, copiez son dossier.
* **`/download`** et **`/upload`**. Contiennent vos produits téléchargeables, les fichiers attachés, et les produits personnalisables. Si vous n'utilisiez pas ces fonctionnalités, ne copiez pas ces dossiers.
*   **`/classes`**. Dans le cas où vous avez ajouté des classes personnalisées dans ce dossier, copiez-les vers le nouveau dossier `/classes`.

    **Si vous faites une mise à jour depuis une version inférieure à la 1.4**, vous devrez faire des modifications manuelles aux classes de PrestaShop que vous avez personnalisé. **Vous n'avez à modifier à la main que celles que vous avez personnalisées**. Pour qu'elles puissent fonctionner correctement avec la dernière version de PrestaShop, toutes les classes doivent recevoir un nouveau suffixe pour leur nom, "Core". _Ne le faites que si vous êtes à l'aise avec les fichiers PHP_.\
    &#x20;Voici comment vous devez modifier les fichiers personnalisés que vous souhaitez conserver :

    *
      * Copiez les fichiers de classe que vous avez personnalisés dans le dossier `/classes` de "prestashop-prep".
      * Ouvrez tous les fichiers de classe que vous avez personnalisés, et trouvez ceux dont le nom de classe ne se termine pas par `Core`. Si vous faites une mise à jour depuis une version 1.4, vous ne devriez pas en trouver (sauf pour vos classes personnalisées, peut-être).
      * Changez le nom de la classe, en lui ajoutant `Core` à la fin. Par exemple, "`MyClass`" devient "`MyClassCore`".\
        &#x20;Ne changez que le nom de la classe PHP dans le fichier, pas le nom du fichier lui-même !
      * Si tous les fichiers ont déjà "Core" dans leur nom de classe (par exemple "`class AttributeCore extends ObjectModel`"), alors vous n'avez rien à faire.
    * Enregistrez les fichiers modifiés.
* **`/config`**. Ne copiez que le fichier `settings.inc.php`.
* `/translations` - si vous utilisez une autre langue que celles disponibles par défaut, vous devrez copier le dossier de votre langue dans le dossier `/translations` de votre nouvelle installation. Sans cela, la mise à jour ne fonctionnera pas.

Votre dossier "prestashop-prep" est maintenant terminé. Vous n'y toucherez plus, et ne travaillerez maintenant qu'avec des copies de ce dossier.

#### Placer le dossier "prestashop-prep" sur votre serveur local <a href="#miseajourmanuelle-placerledossier-prestashop-prep-survotreserveurlocal" id="miseajourmanuelle-placerledossier-prestashop-prep-survotreserveurlocal"></a>

Le dossier "prestashop-prep", que vous aviez décompressé à partir de l'archive de la dernière version de PrestaShop, contient maintenant toutes les personnalisations en provenance de votre dossier "prestashop-prod" (et donc, de votre boutique actuellement en ligne – et normalement en état de maintenance). La prochaine étape consiste à mettre ce dossier sur votre serveur web local afin de tester que la mise à jour se déroule correctement.

Lancez votre serveur local (WAMP, XAMPP, EasyPHP, MAMP ou autre) et assurez-vous que les serveurs Apache et MySQL fonctionnent bien.

L'idée est ici de vérifier localement que votre boutique peut être mise à jour sans problème sur un serveur local, afin de minimiser les risques d'échec lors de la mise à jour en ligne. De fait, il faudrait idéalement que la configuration de votre serveur local soit la plus proche possible de celle de votre hébergement web, afin de ne pas avoir de mauvaise surprise.

Contactez votre hébergeur pour avoir des informations sur la configuration Apache, PHP et MySQL de votre serveur web, et modifiez les fichiers `httpd.conf` (Apache), `php.ini` (PHP) et/ou `my.ini` (MySQL) en conséquence si vous le pouvez. Dans le cas le plus extrême, il vous faudra changer la version de chaque composant pour correspondre à ceux de votre hébergeur.\
&#x20;Ceci fait, redémarrez votre serveur local pour prendre en compte vos modifications.

Si vous ne pouvez pas modifier la configuration de votre serveur local, alors notez bien que les différences avec votre hébergement web peuvent avoir un impact certain sur le bon déroulement de la mise à jour, car ce qui marche dans un environnement peut ne pas fonctionner sur un autre. Typiquement, des limitations de mémoire ou des chemins absolus plutôt que relatifs.

Ouvrez le dossier web de votre serveur local (`/htdocs`, `/www`, `/web` ou autre en fonction du serveur), et copiez-y le dossier "prestashop-prep".

Ne déplacez pas "prestashop-prep" dans votre dossier web local !\
&#x20;Faites bien en sorte de copier le dossier, afin de conserver "prestashop-prep" intact de son côté.

Ainsi, en cas de problème avec la mise à jour locale, vous pouvez revenir au dossier "prestashop-prep" et y apporter des modifications nécessaires avant de copier à nouveau ce dossier dans le dossier web local et de retenter une mise à jour.

Mettez le dossier "prestashop-prep" sur le serveur local, à la racine du dossier web.

#### Recréer la base de données de production <a href="#miseajourmanuelle-recreerlabasededonneesdeproduction" id="miseajourmanuelle-recreerlabasededonneesdeproduction"></a>

Les fichiers locaux sont maintenant a priori à jour, mais la base de données doit également être modifiée. C'est à cela que servira le script de mise à jour manuelle, présent parmi les fichiers de PrestaShop 1.6.

Vous devez avoir une bonne connaissance de phpMyAdmin avant de vous lancer dans cette section.

À partir des fichiers `.sql` sauvegardés dans "prestashop-prod", vous allez donc recréer le base de données de production sur votre serveur local. Pour ce faire, vous devez suivre le processus suivant :

1. Ouvrir l'outil phpMyAdmin, qui doit être fourni avec votre serveur local. Il est le plus souvent à l'adresse [127.0.0.1/phpmyadmin](https://app.gitbook.com/pages/createpage.action?spaceKey=PS16\&title=127.0.0.1%2Fphpmyadmin\&linkCreation=true\&fromPageId=23069397), ou [127.0.0.1/mysql](https://app.gitbook.com/pages/createpage.action?spaceKey=PS16\&title=127.0.0.1%2Fmysql\&linkCreation=true\&fromPageId=23069397).
2. Si ce n'est pas déjà fait, créez une base de données spécialement pour ce projet. Donnez-lui un nom distinctif, comme "prestashop\_update" ou même le nom de la base de données de votre boutique en production, par exemple.\
   &#x20;Si vous aviez déjà créé une base de données lors d'un test de mise à jour locale précédent, effacez toutes ses tables.
3. Ouvrez la base de données, et cliquez sur l'onglet "Importer" situé en haut de l'écran.
4.  Cliquez sur le bouton "Parcourir" et sélectionnez le fichier `.sql` de sauvegarde de votre base de production, qui doit normalement se trouver dans le dossier "prestashop-prod".\
    &#x20;Vérifier que la "Taille maximum" affichée par phpMyAdmin est supérieure à la taille du fichier `.sql`. Si ce n'est pas le cas, il vous faudra modifier le fichier `php.ini` de votre serveur local, notamment les directives `upload_max_filesize`, `post_max_size` et en dernier recours, `memory_limit`. Ceci fait, relancer vos serveurs Apache et MySQL locaux afin de prendre en compte vos modifications.

    Au lieu de modifier les réglages du serveur, vous pouvez plus simplement compresser le fichier `.sql` à l'aide d'un outil de gestion Zip, tel que [http://www.7-zip.org/](http://www.7-zip.org/). phpMyAdmin devrait accepter les fichiers `.sql.zip`, et se chargera des décompresser le fichier avant d'en importer les données.
5. Cliquez sur le bouton "Exécuter" pour importer votre fichier SQL.

Patientez pendant que phpMyAdmin met le fichier en ligne et intègre les tables à la base de données. Ceci fait, vous verrez les tables apparaître dans la colonne latérale gauche de phpMyAdmin.

Reste maintenant à lier les fichiers PHP de PrestaShop aux données sur votre serveur MySQL local. Pour ce faire, vous devez modifier les identifiants de base de données enregistrés dans PrestaShop pour les faire pointer vers la base locale.

Ouvrez le fichier `/config/settings.inc.php`, et modifiez les lignes suivantes :

* `_DB_SERVER_` : remplacez l'adresse du serveur MySQL de votre boutique de production par celle du serveur local. A priori, ce devrait être "localhost" ou "127.0.01".
* `_DB_NAME_` : remplacez le nom de la base de données de votre boutique de production par celui de la base de données locale dans laquelle vous avez importé les tables de votre base de production.
* `_DB_USER_` : remplacez l'identifiant utilisateur de votre boutique de production par celui du serveur local. A priori, ce devrait être "root".
* `_DB_PASSWD_` : remplacez le mot de passe de l'utilisateur MySQL de votre boutique de production par celui du serveur local. A priori, ce devrait être un champ vide : "".

PrestaShop a maintenant accès à votre base de production votre serveur local, il ne vous reste plus qu'à lancer le script de mise à jour.

#### Tout vérifier avant d'aller plus loin <a href="#miseajourmanuelle-toutverifieravantdallerplusloin" id="miseajourmanuelle-toutverifieravantdallerplusloin"></a>

Avez-vous suivi ces étapes ?

1. Vous avez téléchargé la dernière version de PrestaShop.
2. Vous avez décompressé cette version, et l'avez stockée dans le nouveau dossier local "prestashop-prep".
3. Vous avez copié vos fichiers personnalisés depuis votre sauvegarde locale ("prestashop-prod") vers ce dossier "prestashop-prep".
4. Vous avez copié le dossier "prestashop-prep" dans le dossier web sur votre serveur local.
5. Vous avez importé les données de votre boutique de production dans votre serveur MySQL local.
6. Vous avez mis les bons identifiants de base de données locale dans le fichier de configuration.

Si vous avez répondu oui pour tout, passez à l'étape 3.

### Troisième étape – Lancer la mise à jour locale <a href="#miseajourmanuelle-troisiemeetape-lancerlamiseajourlocale" id="miseajourmanuelle-troisiemeetape-lancerlamiseajourlocale"></a>

#### Lancement du script de mise à jour <a href="#miseajourmanuelle-lancementduscriptdemiseajour" id="miseajourmanuelle-lancementduscriptdemiseajour"></a>

Rendez-vous sur l'adresse locale du script de mise à jour, par exemple [http://127.0.0.1/prestashop-prep/install/upgrade/upgrade.php](http://127.0.0.1/prestashop-prep/install/upgrade/upgrade.php) (remplacez "prestashop-prep" par le vrai nom du dossier que vous avez copié dans le dossier web de votre serveur local).

Si l'adresse renvoie une erreur 404, peut-être avez oublié certains fichiers de la dernière version de PrestaShop 1.6. Refaites les différentes étapes du processus : effacez le dossier que vous avez copié dans le dossier web local (mais mettez de côté le fichier `settings.inc.php` afin de ne pas avoir à la modifier à nouveau), modifiez le contenu du dossier "prestashop-prep" en fonction des besoins, et copiez à nouveau "prestashop-prep" dans le dossier web du serveur local.

Une fois le script lancé, **ne touchez plus à votre navigateur web !** Ne le fermez pas, ne cliquez pas sur le bouton "Retour" : le script de mise à jour travaille, et cela peut prendre plusieurs minutes. Laissez-le faire !

Le script de mise à jour s'occupe principalement de mettre à jour la base de données SQL, ce qui peut s'avérer très complexe. Il prend également en charge la mise à jour du fichier des réglages de base `config/settings.inc.php` en fonction de votre configuration et de l'environnement, ainsi que d'autres aspects du fonctionnement de PrestaShop.

#### Terminer la mise à jour locale <a href="#miseajourmanuelle-terminerlamiseajourlocale" id="miseajourmanuelle-terminerlamiseajourlocale"></a>

Une fois la mise à jour terminée, un fichier XML devrait s'afficher dans votre navigateur. C'est absolument normal, mais cela peut vous surprendre, car l'affichage ne ressemble pas à une page web classique, et chaque navigateur web a sa propre manière de l'afficher. Par exemple, Firefox affichera d'abord un message d'avertissement, "_Aucune information de style ne semble associée à ce fichier XML. L'arbre du document est affiché ci-dessous_", au-dessus du contenu du fichier XML lui-même. Ce sera amélioré dans les versions ultérieures du script.

La page doit commencer par la ligne suivante :

```
<action result="ok" error=""> 
```

C'est le "ok" qui compte : ça a marché ! Le plus dur est fait, restent les détails.

Sur votre serveur web local, dans le dossier `/prestashop-prep`, vous devriez effacer :

* Le dossier `/install`, qui contient le script d'installation.
* Les fichiers `README`, qui contiennent des informations sur votre installation de PrestaShop.
* Le fichier `CHANGELOG`, qui contient des informations sur les dernières modifications apportées à PrestaShop.

Vous pouvez maintenant vous rendre sur votre boutique locale à l'adresse publique ([http://127.0.0.1/prestashop-prep](http://127.0.0.1/prestashop-prep) dans notre exemple), qui devrait afficher la page de maintenance avec votre logo, étant donné que votre boutique est censée être en mode de maintenance.

Si cette page de maintenance ou votre thème n'apparaît pas, mais qu'à la place vous obtenez un message disant "Votre thème n'est pas disponible : -_nom du thème_'. Veuillez vérifier le nom du répertoire du thème et ces permissions", alors vous avez sans doute oublié de copier votre thème vers le dossier "prestashop-prep".

Depuis le dossier `/themes` de votre dossier "prestashop-prod", copiez votre thème vers le dossier `/themes` de "prestashop-prep". Rechargez le contenu de votre navigateur pour voir la page de maintenance – ou votre thème.

Si votre logo ne s'affiche page, mais qu'à la place vous avez un logo "YourLogo", alors vous avez sans doute oublié l'étape où vous deviez copier vos images personnalisées depuis le dossier "prestashop-prod" vers le dossier "prestashop-prep".

Relisez l'étape 2 de ce chapitre ("Deuxième étape – Se préparer pour la nouvelle version") afin de copier les bons fichiers et dossiers.

Maintenant, rendez-vous sur la page d'administration de votre boutique, avec le nom de dossier `/admin` que vous aviez personnalisé. Vous devrez vous connecter à l'aide de vos identifiants. Parcourez les différentes pages de l'administration pour vérifier que votre contenu est bien là et que toutes les pages du back-office fonctionnent, puis sortez la boutique du mode de maintenance afin d'explorer les pages du front-office comme le ferait un visiteur no\
&#x20;rmal, et assurez-vous que toutes fonctionnent.

**En cas d'échec de la mise à jour**

Toutes les mises à jour ne se terminent pas forcément bien, et les raisons très variées. Pour vous aider, le script de mise à jour vous affiche un code d'erreur au début du résultat XML. En cas d'erreur, la page commence ainsi :

```
<action result="fail" error="27" />
```

Notez donc que `result` ne contient plus "ok" mais "fail".

Voici quelques-unes des erreurs les plus courantes :

| Code d'erreur | Signification                                                 | Solution possible                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| ------------- | ------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 5             | Le fichier de configuration n'est pas accessible en lecture.  | Changez les droits d'accès du fichier `/config/settings.inc.php`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| 6             | Le fichier de configuration n'est pas accessible en écriture. | Changez les droits d'accès du fichier `/config/settings.inc.php`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| 27            | Le script d'installation est trop vieux.                      | Vous devez utiliser la dernière version de PrestaShop.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| 28            | Vous utilisez déjà la version cible.                          | <p>La version vers laquelle vous essayez de mettre à jour est la même que celle déjà installée. S'il s'agit de la version la plus récente de PrestaShop, inutile de faire une mise à jour. Sinon, téléchargez la dernière version de PrestaShop.<br>Cette erreur peut également survenir quand vous avez relancé la mise à jour après une première tentative. Si c'est le cas, vérifiez que l'administration fonctionne et indique bien la dernière version en date. Le cas échéant, utilisez vos sauvegardes/backups (fichiers et base de données) pour revenir à zéro, et repartez de là.</p> |
| 29            | Il n'y a pas de version plus ancienne.                        | Avez-vous bien copié le fichier `config/settings.inc.php` tel quel ?                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| 31            | Fichiers de mise à jour SQL introuvables.                     | Vérifiez que le dossier `/install/upgrade/sql` n'est pas vide. Si c'est le cas, récupérez les fichiers SQL de mises à jour à partir de l'archive de la dernière version.                                                                                                                                                                                                                                                                                                                                                                                                                        |
| 32            | Impossible de mettre à jour.                                  | Certains fichiers sont sans doute absent ou mal copiés. Reprenez le processus depuis le début.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| 33            | Erreur lors de la lecture des fichiers SQL de mise à jour.    | Vérifiez que les fichiers du dossier `/install/upgrade/sql` sont bien présents et accessibles en lecture.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| 34            | Erreur SQL interne.                                           | Les fichiers de mise à jour SQL sont sans doute corrompus. Retéléchargez l'archive de la nouvelle version, et utilisez les fichiers du dossier `/install/upgrade/sql` de cette archive.                                                                                                                                                                                                                                                                                                                                                                                                         |
| 35            | Le cache est activé.                                          | Désactivez le cache de PrestaShop avant de lancer le script de mise à jour : ouvrez le fichier `config/settings.inc.php`, et vérifiez que `define('`_`PS_CACHE_ENABLED`_`', '0');` est bien à 0.                                                                                                                                                                                                                                                                                                                                                                                                |

Lorsque le script de mise à jour échoue, il est difficile de savoir s'il a pu faire une partie de cette mise à jour. Avant de retenter la mise à jour, il est donc préférable de remettre en place vos fichiers et base de données sauvegardées :

* effacez tous les fichiers du dossier web local et remplacez-les par ceux du dossier "prestashop-prep", intacts car gardés de côté.
* effacez toutes les tables de la base de données de test, et remplacez-les par celles de l'installation originale.

### Quatrième étape – tests et assurance qualité <a href="#miseajourmanuelle-quatriemeetape-testsetassurancequalite" id="miseajourmanuelle-quatriemeetape-testsetassurancequalite"></a>

#### Importer vos traductions <a href="#miseajourmanuelle-importervostraductions" id="miseajourmanuelle-importervostraductions"></a>

Si vous avez exporté vos traductions personnalisées durant la première étape, il vous faut les importer dans votre nouvelle boutique en vous rendant dans la page "Traductions" du menu "Localisation", et utiliser le formulaire de la section "Ajouter / Mettre à jour une langue".

#### Tests à faire sur votre boutique locale mise à jour <a href="#miseajourmanuelle-testsafairesurvotreboutiquelocalemiseajour" id="miseajourmanuelle-testsafairesurvotreboutiquelocalemiseajour"></a>

Pour vous assurer que tout fonctionne correctement sur votre boutique mise à jour localement, nous vous recommandons de faire les tests suivants :

* Charger tous les types de pages (accueil, catégorie, produit, comparaison, CMS, etc.)
* Créer un compte client
* Faire une commander (ajouter des produits à un panier et valider)
* Vérifier que le paiement se passe sans problème (carte de crédit, PayPal, etc.)
* Dans le back-office, vérifier que les commandes passées sont bien reçues
* Envoyer un e-mail depuis la page de contact, récupérer votre mot de passe
* Relire la facture
* Vérifier les fonctionnalités de tous les modules que vous avez activés

Cette liste est loin d'être exhaustive, vous devriez faire autant de tests que possible, et créer les vôtres.

Si vous remarquez que certains aspects de la boutique mise à jour ne fonctionnent pas correctement :

1. modifiez le contenu de "prestashop-prep" pour palier à ces problèmes (fichiers manquants, mauvaise configuration, etc.),
2. relancez le processus de mise à jour local :
   1. effacez le sous-dossier de votre test PrestaShop dans le dossier web de votre serveur local,
   2. effacez les tables MySQL de votre test de mise à jour,
   3. copiez les fichiers modifiés de "prestashop-prep" dans le dossier web local,
   4. remettez sur votre serveur MySQL local les tables sauvegardées, tirées du fichier `.sql` stocké dans le dossier "prestashop-prod",
   5. relancez le script de mise à jour.

Si tous vos tests se passent sans problème, félicitations ! Passez à l'étape 5.

### Cinquième étape – Lancer la mise à jour sur votre hébergement web <a href="#miseajourmanuelle-cinquiemeetape-lancerlamiseajoursurvotrehebergementweb" id="miseajourmanuelle-cinquiemeetape-lancerlamiseajoursurvotrehebergementweb"></a>

Parvenu à cette étape, vous devez avoir réussi à mettre à jour votre boutique sur votre serveur local. Ce faisant, vous vous offrez une meilleure garantie que la mise à jour sur votre hébergement web se déroulera sans problème. Votre dossier "prestashop-prep" contient tous les fichiers nécessaires, car vous avez modifié son contenu en fonction des manques remarqués lors de vos tests de l'étape précédente.

Cette "garantie" ne peut jamais être à 100% tant les deux environnements (serveur local et hébergement web) peuvent différer. Votre meilleure chance reste de configurer votre serveur local de telle sorte qu'il corresponde le mieux possible à votre serveur de production, chez votre hébergeur web.

Votre boutique en ligne est en mode maintenance depuis le début de votre processus, afin de ne pas perdre de commandes, de paniers ou même de nouveaux clients lors de la mise à jour. Si ce n'est pas déjà le cas, mettez la boutique en mode maintenance maintenant, et recommencez le processus du début – à moins que vous ne craigniez pas de perdre les modifications survenues depuis le début.

Outre le fait de mettre les fichiers en ligne plutôt que sur votre serveur local, le processus ne varie que peu de celui déjà testé localement :

1. À l'aide de votre client FTP, remplacez les fichiers de votre boutique en ligne par ceux de votre dossier "prestashop-prep".\
   &#x20;Vous ne devriez rien avoir à craindre, car tous vos fichiers ont été sauvegardés au début du processus dans le dossier "prestashop-prod", donc vous pouvez revenir à cette sauvegarde à n'importe quel moment. Idem pour votre base de données, sauvegardée également dans le dossier "prestashop-prod" sous forme de fichier `.sql`.
2. Lancez le script de mise à jour sur votre boutique en production, en y accédant avec votre navigateur. Dans la version 1.6, le script est situé à l'adresse `/install/upgrade/upgrade.php`.
3. Vérifiez tous les paramètres avant la mise à jour : suivez les instructions à l'écran et assurez-vous que votre serveur est conforme aux exigences techniques de la nouvelle version.
4. Fin de la mise à jour : une fois la mise à jour terminée, supprimez le dossier `/install` et rendez-vous sur votre front-office et votre back-office pour vous assurer que tout fonctionne.

### Sixième étape – tests et assurance qualité <a href="#miseajourmanuelle-sixiemeetape-testsetassurancequalite" id="miseajourmanuelle-sixiemeetape-testsetassurancequalite"></a>

Il vous faut refaire tous les tests déjà réalisés en local, afin de vous assurer que rien ne passe au travers du filet malgré le changement d'un environnement local à un environnement de production.

#### Importer vos traductions <a href="#miseajourmanuelle-importervostraductions.1" id="miseajourmanuelle-importervostraductions.1"></a>

Si vous avez exporté vos traductions personnalisées durant la première étape, il vous faut les importer dans votre nouvelle boutique en vous rendant dans la page "Traductions" du menu "Localisation", et utiliser le formulaire de la section "Ajouter / Mettre à jour une langue".

#### Vérification de votre nom de domaine <a href="#miseajourmanuelle-verificationdevotrenomdedomaine" id="miseajourmanuelle-verificationdevotrenomdedomaine"></a>

Vous devez vérifier que le nom domaine assigné dans la base de données correspond à celui avec lequel vous travaillez. Pour ce faire, rendez-vous dans la page "SEO & URLs", sous le menu "Préférences".

Vérifiez les informations suivantes, dans la section "URL de la boutique" :

* "Domaine" : il doit s'agir du nom de domaine auquel vous êtes connecté. Si ce n'est pas le cas, tous les liens de votre boutique ne fonctionneront pas, car ils pointeront vers un autre domaine.
* "Chemin" : il doit s'agir du dossier que vous avez transféré sur vos serveurs FTP ; dans ce tutoriel, il s'agit de `/prestashop`.

Si vous ne pouvez pas passer par l'interface d'administration, il vous faudra passer par l'outil de gestion de base de données installé chez votre hébergeur, comme phpMyAdmin :

1. Ouvrez la base de données de votre boutique de production,
2. Ouvrez la table `ps_shop_url`,
3. Modifiez les colonnes `domain`, `domain_ssl` et `physical_uri` pour qu'elles correspondent à l'emplacement de votre boutique de production.

Comme vous pouvez le constater, l'adresse et le chemin de votre boutique ne sont plus stockés dans le fichier `/config/settings.inc.php` à partir de la version 1.5 de PrestaShop, mais dans la base de données.

Vous pouvez donc ouvrir le fichier `/config/settings.inc.php` et supprimer la ligne `define('_`_`PS_BASE_URI`_`_', '/le_chemin_de_la_boutique/');` si la mise a jour ne s'en est pas chargé.

#### Tests à faire sur votre boutique de production mise à jour <a href="#miseajourmanuelle-testsafairesurvotreboutiquedeproductionmiseajour" id="miseajourmanuelle-testsafairesurvotreboutiquedeproductionmiseajour"></a>

Pour vous assurer que tout fonctionne correctement sur votre boutique mise à jour, nous vous recommandons de faire les tests suivants :

* Charger tous les types de pages (accueil, catégorie, produit, comparaison, CMS, etc.)
* Créer un compte client
* Faire une commande (ajouter des produits à un panier et valider)
* Vérifier que le paiement se passe sans problème (carte de crédit, PayPal, etc.)
* Dans le back-office, vérifier que les commandes passées sont bien reçues
* Envoyer un e-mail depuis la page de contact, récupérer votre mot de passe
* Relire la facture
* Vérifier les fonctionnalités de tous les modules que vous avez activés

Cette liste est loin d'être exhaustive, vous devriez faire autant de tests que possible, et créer les vôtres.

Si vous remarquez que certains aspects ne fonctionnent pas correctement :

1. modifiez le contenu de "prestashop-prep" pour palier à ces problèmes (fichiers manquants, mauvaise configuration, etc.),
2. relancez le processus de mise à jour local :
   1. effacez le sous-dossier de votre test PrestaShop dans le dossier web de votre serveur local,
   2. effacez les tables MySQL de votre test de mise à jour,
   3. mettez en place les fichiers modifiés de "prestashop-prep",
   4. remettez sur votre serveur MySQL local les tables sauvegardés, tirées du fichier `.sql` stocké dans le dossier "prestashop-prod".

Si tous vos tests se passent sans problème, félicitations ! Passez à l'étape 7.

### Septième étape – Relancer votre boutique mise à jour <a href="#miseajourmanuelle-septiemeetape-relancervotreboutiquemiseajour" id="miseajourmanuelle-septiemeetape-relancervotreboutiquemiseajour"></a>

Félicitations, vous êtes parvenu sans encombre au bout du processus de mise à jour !

Il ne vous reste plus qu'à réactiver la boutique. Rendez-vous dans la page "Maintenance" du menu "Préférences", et choisissez "Oui" pour l'option "Activer la boutique".

Allez à la page d'accueil de votre boutique, et parcourez-en toutes les pages afin de vous assurer une dernière fois que tout fonctionne correctement pour vos clients.

C'est terminé ! Félicitations, vous avez terminé votre mise à jour vers la dernière et meilleure version PrestaShop !
