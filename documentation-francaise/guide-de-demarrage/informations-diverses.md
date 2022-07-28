# Informations diverses

**Contenu**

/\*\<!\[CDATA\[\*/\
div.rbtoc1597053582924 {padding: 0px;}\
div.rbtoc1597053582924 ul {list-style: disc;margin-left: 0px;}\
div.rbtoc1597053582924 li {margin-left: 0px;padding-left: 0px;}\
\
/\*]]>\*/

* [Informations diverses](informations-diverses.md#Informationsdiverses-Informationsdiverses)
  * [Gardez une version de test à portée de main](informations-diverses.md#Informationsdiverses-Gardezuneversiondetestàportéedemain)
  * [Vérifiez la bibliothèque GD](informations-diverses.md#Informationsdiverses-VérifiezlabibliothèqueGD)
  * [Activez PHP5](informations-diverses.md#Informationsdiverses-ActivezPHP5)
    * [1&1](informations-diverses.md#Informationsdiverses-1&1)
    * [Free.fr](informations-diverses.md#Informationsdiverses-Free.fr)
    * [OVH](informations-diverses.md#Informationsdiverses-OVH)
    * [GoDaddy](informations-diverses.md#Informationsdiverses-GoDaddy)
    * [Lunarpages (mutualisé)](informations-diverses.md#Informationsdiverses-Lunarpages\(mutualisé\))

## Informations diverses <a href="#informationsdiverses-informationsdiverses" id="informationsdiverses-informationsdiverses"></a>

### Gardez une version de test à portée de main <a href="#informationsdiverses-gardezuneversiondetestaporteedemain" id="informationsdiverses-gardezuneversiondetestaporteedemain"></a>

Après avoir installé et réglé votre boutique afin qu'elle corresponde le mieux à vos besoins, mais avant de l'ouvrir officiellement au public, nous vous recommandons **fortement** d'installer une version locale de test sur votre ordinateur (à l'aide de [WAMP](http://en.wikipedia.org/wiki/Comparison\_of\_WAMPs) pour Windows, [MAMP](http://en.wikipedia.org/wiki/MAMP) pour Mac, ou [LAMP](http://en.wikipedia.org/wiki/LAMP\_\(software\_bundle) pour Linux, ou [XAMPP](http://www.apachefriends.org/en/xampp.html) pour n'importe laquelle de ces plateformes), ou sur un autre emplacement de votre serveur d'hébergement.

Cette seconde installation vous sera utile en tant qu'environnement de pré-production, sur laquelle vous pourrez tester toutes vos idées de modifications pour votre boutique, sans affecter la boutique en ligne. Ainsi, si une erreur se produit sur cet environnement de test, votre boutique réelle ne serait pas affectée.

Après avoir confirmé que votre version de test fonctionne, copiez ses fichiers sur ceux de votre version en ligne. Il est préférable de faire cette copie en dehors des heures d'affluence, et en ayant pris soin de mettre temporairement votre boutique en mode maintenance.

### Vérifiez la bibliothèque GD <a href="#informationsdiverses-verifiezlabibliothequegd" id="informationsdiverses-verifiezlabibliothequegd"></a>

La [bibliothèque GD](http://www.boutell.com/gd/) permet à PrestaShop de retoucher les images que vous mettez en ligne, notamment d'en changer la taille.

Une installation standard de PHP devrait avoir la bibliothèque GD activée, mais si ce n'est pas le cas pour votre installation, les instructions Windows sont :

1. Dans le dossier racine de votre dossier PHP, ouvrez le fichier `php.ini`,
2. Décommentez a la ligne `extension=php_gd2.dll` (située vers la moitié du fichier, au milieu d'une longue liste d'extensions) en effaçant le ";" au début de la ligne.
3. Relancez les services PHP.

Si vous n'avez pas accès au fichier `php.ini` (ce qui est souvent le cas sur les hébergements mutualisé), contactez votre hébergeur en lui indiquant votre besoin.

### Activez PHP5 <a href="#informationsdiverses-activezphp5" id="informationsdiverses-activezphp5"></a>

La plupart du temps, les serveurs dédiés ou mutualisés disposent à la fois de PHP 4 et PHP 5, mais PHP 4 reste encore la version activée par défaut.

Pour installer PrestaShop, PHP 5 doit être activé. Si vous tentez de faire fonctionner PrestaShop avec PHP 4, vous verrez de nombreux messages d'erreur s'afficher, notamment celui-ci :

```
Parse error: parse error, unexpected T_STATIC, expecting T_OLD_FUNCTION or T_FUNCTION or T_VAR or '}' in [php file] on line X.
```

Voici une liste de procédures pour activer PHP5, en fonction des hébergeurs...

#### 1&1 <a href="#informationsdiverses-1-and-1" id="informationsdiverses-1-and-1"></a>

Ajoutez cette ligne à votre fichier `.htaccess` :

```
AddType x-mapp-php5 .php
```

Pour la réécriture d'URL, ajoutez ces lignes :

```
Options +FollowSymLinks
RewriteEngine On
```

#### Free.fr <a href="#informationsdiverses-free.fr" id="informationsdiverses-free.fr"></a>

Ajoutez cette ligne à votre fichier `.htaccess` :

```
php 1
```

#### OVH <a href="#informationsdiverses-ovh" id="informationsdiverses-ovh"></a>

Ajoutez cette ligne à votre fichier `.htaccess` :

```
SetEnv PHP_VER 5
```

Pour désactiver les variables globales :

```
SetEnv REGISTER_GLOBALS 0
```

#### GoDaddy <a href="#informationsdiverses-godaddy" id="informationsdiverses-godaddy"></a>

Pour voir votre version de PHP :

1. Connectez-vous à votre Account Manager.
2. Dans la section Products, cliquez sur Web Hosting.
3. À côté du compte d'hébergement que vous voulez utiliser, cliquez sur Launch.

Dans la section Server, vous pourrez voir la version de PHP.

Pour modifier la version de PHP :

1. Dans le menu Content, sélectionnez Programming Languages.
2. Sélectionnez la version de PHP que vous souhaitez utiliser, puis cliquez sur Continue.
3. Cliquez sur Update.

Les modifications peuvent mettre jusqu'à 24h à être prises en compte.

#### Lunarpages (mutualisé) <a href="#informationsdiverses-lunarpages-mutualise" id="informationsdiverses-lunarpages-mutualise"></a>

1. Connectez-vous à cPanel. Il devrait se trouver à l'adresse [http://www.(votre\_domaine).(com/net/org/etc.)/cpanel](http://www.\(votre\_domaine\).\(com/net/org/etc.\)/cpanel)
2. Saisissez vos identifiants.
3. Dans la page qui s'affiche, cliquez sur l'icône "Enable/Disable PHP 5".
4. Dans la page qui s'affiche, cliquez sur "Add PHP 5 To Your Account!".

Les modifications peuvent mettre jusqu'à 24h à être prises en compte.
