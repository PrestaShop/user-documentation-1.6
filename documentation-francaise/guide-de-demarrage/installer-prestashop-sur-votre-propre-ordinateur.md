# Installer PrestaShop sur votre propre ordinateur

Il se peut que vous préfériez d'abord installer PrestaShop sur votre propre ordinateur pour commencer, soit pour tester l'application avant d'investir dans un serveur et un nom de domaine, ou pour personnaliser votre boutique en local avant de mettre vos modifications en ligne sur le PrestaShop que vous auriez déjà installé sur votre hébergement web.

Installer n'importe quelle application web localement requiert que vous installiez d'abord un environnement adéquat, à savoir le serveur web Apache, l'interpréteur de langage PHP, le serveur de base de données MySQL, et idéalement l'outil phpMyAdmin. L'ensemble est connu sous l'acronyme AMP : Apache+MySQL+PHP. Cet ensemble existe pour tous les systèmes d'exploitation, en ajoutant une lettre à l'acronyme : WAMP (Windows+Apache+MySQL+PHP), MAMP (Mac OS X+...) et LAMP (Linux+...).

## Choisir un package AMP <a href="#installerprestashopsurvotrepropreordinateur-choisirunpackageamp" id="installerprestashopsurvotrepropreordinateur-choisirunpackageamp"></a>

Il vous faudrait vous plonger dans la technique pour tout installer. Heureusement, il existe de nombreux pack préconstruits qui s'installent facilement. Ils ne vous empêcheront pas de devoir vous plonger dans la technique ici et là, mais ils aident grandement. Étant donné que tous les logiciels de ce pack sont open-source, les installeurs de ces environnements sont la plupart du temps gratuits. Voici une sélection d'installeurs AMP gratuits :

* EasyPHP : [http://www.easyphp.org/](http://www.easyphp.org/) (Windows)
* MAMP : [http://www.mamp.info/](http://www.mamp.info/) (Mac OS X)
* WampServer : [http://www.wampserver.com/en/](http://www.wampserver.com/en/) (Windows)
* XAMPP : [http://www.apachefriends.org/en/xampp.html](http://www.apachefriends.org/en/xampp.html) (Windows, Mac OS X, Linux, Solaris)\
  \


EasyPHP dispose d'un package tout-en-un, qui inclue une installation prête-à-l'emploi de PrestaShop 1.6 ! C'est la manière la plus simple de découvrir la dernière version de PrestaShop et, pour les développeurs, de concevoir des thèmes et modules.

Téléchargez-le pack ici : [http://www.easyphp.org/prestashop.php](http://www.easyphp.org/prestashop.php)

Choisissez le pack avec lequel vous êtes le plus à l'aise, et lancez-le.

## Vérifier que tout fonctionne <a href="#installerprestashopsurvotrepropreordinateur-verifierquetoutfonctionne" id="installerprestashopsurvotrepropreordinateur-verifierquetoutfonctionne"></a>

Avant de vous lancer dans le tutoriel d'installation de PrestaShop, vérifiez que tous les composants fonctionnent correctement :

*   **Le serveur web doit être lancé**. Vous devriez pouvoir y accéder à l'aide de votre navigateur, en saisissant "127.0.0.1" dans la barre d'adresse.

    [`http://127.0.0.1`](http://127.0.0.1) est l'adresse "localhost", qui correspond à votre ordinateur : il s'agit d'une adresse de retour, qui envoie votre navigateur vers le serveur web local.

    Dans les faits, [`http://127.0.0.1`](http://127.0.0.1) et [`http://localhost`](http://localhost) sont synonymes : vous pouvez utiliser l'un ou l'autre sans voir de différence, les deux vous renverront vers le dossier racine de votre serveur web local.

    Certains serveurs web peuvent ne pas pouvoir se lancer parce que les ports de connexion (typiquement, le port 80) sont déjà utilisés par une autre application.

    Cela arrive souvent lorsque Skype est utilisé. Pour empêcher Skype de bloquer le lancement de votre serveur web loca, rendez-vous dans les réglages avancés de Skype (Outils > Options > Avancées > Connexions) et décochez l'option "Utiliser les ports 80 et 443 comme alternative". Relancez ensuite Skype, et relancez votre serveur web local.
* **Le serveur de base de données doit être lancé**. PrestaShop stocke toutes ses données dans une base de données MySQL. Le pack AMP doit vous donner un indicateur clair du lancement ou non de MySQL.
* **L'outil phpMyAdmin doit être lancé**. Il s'agit d'une application web qui vous aide à gérer les données stockées dans MySQL. Son adresse dépend du pack AMP que vous avez choisi : elle peut se trouver à l'adresse [`http://127.0.0.1/phpmyadmin`](http://127.0.0.1/phpmyadmin) (XAMPP, WampServer, MAMP), [`http://127.0.0.1/mysql`](http://127.0.0.1/mysql) (EasyPHP), ou une autre adresse. Lisez la documentation de votre pack AMP – peut-être même l'interface du pack vous offre-t-elle un bouton qui ouvrira directement votre navigateur web à la bonne adresse.

## Trouver le dossier racine du serveur web local <a href="#installerprestashopsurvotrepropreordinateur-trouverledossierracineduserveurweblocal" id="installerprestashopsurvotrepropreordinateur-trouverledossierracineduserveurweblocal"></a>

Une fois que vous avez vérifié que le pack est bien installé et que tous ses composants sont lancés, vous devez trouver le dossier racine de votre serveur web.

Il s'agit du dossier local où vous aller placer les fichiers de vos applications, et qui peut se comparer au dossier racine de votre serveur en ligne, sauf que son contenu est ici accessible via [`http://127.0.0.1`](http://127.0.0.1).

L'emplacement effectif de ce dossier sur votre machine dépend grandement du pack AMP que vous utilisez, et peut souvent être personnalisé :

* EasyPHP : `C:\easyphp\www`
* MAMP : `/Applications/MAMP/htdocs/`
* WampServer : `C:\wamp\www`
* XAMPP : `C:\xampp\htdocs` ou `/Applications/xampp/htdocs`

## Trouver les informations sur l'utilisateur MySQL <a href="#installerprestashopsurvotrepropreordinateur-trouverlesinformationssurlutilisateurmysql" id="installerprestashopsurvotrepropreordinateur-trouverlesinformationssurlutilisateurmysql"></a>

Finalement, vous devez connaître le nom d'administrateur (_root user_) de MySQL et son mot de passe, afin d'installer PrestaShop.

**La plupart des packs utilisent le nom "root" avec un mot de passe vide**, y compris EasyPHP, MAMP, WampServer et XAMPP.

Lisez la documentation de votre pack.

## Une dernière note avant le tutoriel d'installation <a href="#installerprestashopsurvotrepropreordinateur-unedernierenoteavantletutorieldinstallation" id="installerprestashopsurvotrepropreordinateur-unedernierenoteavantletutorieldinstallation"></a>

Une fois tout ceci correctement réglé, vous pouvez suivre la suite du guide de démarrage et commencer à installer PrestaShop normalement.

Lorsque vous faites une installation locale, gardez en tête que :

* les fichiers ne doivent pas être mis en ligne sur un serveur web à l'aide d'un logiciel FTP (type Filezilla), mais simplement placés dans votre dossier racine local, comme indiqué ci-dessus.
* Vous n'avez pas à créer un nom de domaine local : PrestaShop sera accessible par le biais de l'adresse locale indiquée ci-dessus, qui sera [`http://localhost`](http://localhost) ou [`http://127.0.0.1`](http://127.0.0.1). Ajoutez le sous-dossier dans lequel se trouvent les fichiers de PrestaShop pour accéder à votre boutique locale, par exemple [`http://localhost/prestashop`](http://localhost/prestashop) or [`http://127.0.0.1/prestashop`](http://127.0.0.1/prestashop) si les fichiers sont dans le sous-dossier `/prestashop/` du dossier racine. Lorsque vous accédez à l'adresse de PrestaShop pour la première fois, vous serez automatiquement renvoyé vers l'installateur de PrestaShop, disponible à l'adresse [`http://localhost/prestashop/install`](http://localhost/prestashop/install) ou [`http://127.0.0.1/prestashop/install`](http://127.0.0.1/prestashop/install) .\


Avez-vous bien tout lu ? Maintenant, lisez le guide d'installation normal, en commençant directement par la section "Créer une base de données pour votre boutique" : [Installer PrestaShop](installer-prestashop.md).
