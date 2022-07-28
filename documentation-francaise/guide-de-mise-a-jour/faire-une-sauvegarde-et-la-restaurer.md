# Faire une sauvegarde et la restaurer

**Contenu**

* [Faire une sauvegarde et la restaurer](faire-une-sauvegarde-et-la-restaurer.md#Faireunesauvegardeetlarestaurer-Faireunesauvegardeetlarestaurer)
  * [Faire votre propre sauvegarde](faire-une-sauvegarde-et-la-restaurer.md#Faireunesauvegardeetlarestaurer-Fairevotrepropresauvegarde)
    * [Sauvegarder vos fichiers](faire-une-sauvegarde-et-la-restaurer.md#Faireunesauvegardeetlarestaurer-Sauvegardervosfichiers)
    * [Sauvegarder votre base de données](faire-une-sauvegarde-et-la-restaurer.md#Faireunesauvegardeetlarestaurer-Sauvegardervotrebasededonnées)
      * [Utiliser l'outil de sauvegarde de PrestaShop](faire-une-sauvegarde-et-la-restaurer.md#Faireunesauvegardeetlarestaurer-Utiliserl%27outildesauvegardedePrestaShop)
      * [Utiliser phpMyAdmin](faire-une-sauvegarde-et-la-restaurer.md#Faireunesauvegardeetlarestaurer-UtiliserphpMyAdmin)
      * [À l'aide de l'outil de gestion de base de données de votre hébergeur](faire-une-sauvegarde-et-la-restaurer.md#Faireunesauvegardeetlarestaurer-Àl%27aidedel%27outildegestiondebasededonnéesdevotrehébergeur)
  * [Restaurer votre sauvegarde](faire-une-sauvegarde-et-la-restaurer.md#Faireunesauvegardeetlarestaurer-Restaurervotresauvegarde)
    * [Nettoyer votre serveur](faire-une-sauvegarde-et-la-restaurer.md#Faireunesauvegardeetlarestaurer-Nettoyervotreserveur)
      * [Créer une page de maintenance](faire-une-sauvegarde-et-la-restaurer.md#Faireunesauvegardeetlarestaurer-Créerunepagedemaintenance)
      * [Supprimer les fichiers](faire-une-sauvegarde-et-la-restaurer.md#Faireunesauvegardeetlarestaurer-Supprimerlesfichiers)
      * [Supprimer les données](faire-une-sauvegarde-et-la-restaurer.md#Faireunesauvegardeetlarestaurer-Supprimerlesdonnées)
    * [Restaurer vos fichiers et données](faire-une-sauvegarde-et-la-restaurer.md#Faireunesauvegardeetlarestaurer-Restaurervosfichiersetdonnées)
      * [Restaurer vos fichiers](faire-une-sauvegarde-et-la-restaurer.md#Faireunesauvegardeetlarestaurer-Restaurervosfichiers)
      * [Restaurer vos fichiers](faire-une-sauvegarde-et-la-restaurer.md#Faireunesauvegardeetlarestaurer-Restaurervosfichiers.1)

## Faire une sauvegarde et la restaurer <a href="#faireunesauvegardeetlarestaurer-faireunesauvegardeetlarestaurer" id="faireunesauvegardeetlarestaurer-faireunesauvegardeetlarestaurer"></a>

Que vous soyez en train de mettre à jour votre installation de PrestaShop à l'aide de la méthode automatique ou manuelle, vous devez vous assurer que vous avec à votre disposition votre propre sauvegarde de vos données, une sauvegarde que vous avez complète et qui vous servirait à revenir en arrière en cas de problème.

Lorsque vous faites une mise à jour de la boutique, il est fortement recommandé de ne faire votre sauvegarde qu'une fois que la boutique a été mise en mode de maintenance. Ainsi, vous vous assurez qu'aucune donnée client n'est perdue si vous devez annuler la mise à jour revenir à cette sauvegarde.\
Ne lancez pas la mise à jour avant d'avoir correctement sauvegardé autant vos fichiers que vos données sur votre ordinateur.

Le processus décrit dans ce chapitre va vous faire transférer des fichiers à l'aide d'un logiciel FTP, télécharger des données depuis un serveur web à l'aide d'outils en ligne, et même effacer toutes vos données et tous vos fichiers en ligne. ne vous lancez pas si vous n'avez pas déjà une bonne connaissance de ces outils et technologies. Si vous le devez (par exemple, si votre boutique ne marche plus après une mise à jour), demandez de l'aide à un ami plus technique, et prenez le temps de parcourir chaque étape en totalité. Le cas échéant, vous risquez de perdre votre boutique à jamais.

### Faire votre propre sauvegarde <a href="#faireunesauvegardeetlarestaurer-fairevotrepropresauvegarde" id="faireunesauvegardeetlarestaurer-fairevotrepropresauvegarde"></a>

Tout d'abord, créer un dossier sur votre ordinateur, où vous stockerez à la fois vos fichiers PrestaShop et vos données. Nommez-le avec la date actuelle, afin de savoir exactement de quand date cette sauvegarde.

#### Sauvegarder vos fichiers <a href="#faireunesauvegardeetlarestaurer-sauvegardervosfichiers" id="faireunesauvegardeetlarestaurer-sauvegardervosfichiers"></a>

C'est très facile :

1. Connectez-vous à votre serveur web à l'aide de n'importe quel logiciel FTP, par exemple FileZilla.
2. Téléchargez tous les fichiers du dossier en ligne de PrestaShop, dans le dossier de sauvegarde de votre ordinateur.

Ce processus peut prendre du temps, en fonction de la vitesse de votre serveur. PrestaShop utilise environ 10 000 fichiers dans 2 000 dossiers, et ce sans compter vos propres fichiers (images de produit, thèmes, modules, etc.) ni les images personnalisées de vos clients. Laissez tourner le processus jusqu'au bout : ne touchez pas à votre logiciel FTP avant la fin du transfert.

#### Sauvegarder votre base de données <a href="#faireunesauvegardeetlarestaurer-sauvegardervotrebasededonnees" id="faireunesauvegardeetlarestaurer-sauvegardervotrebasededonnees"></a>

Tandis que les fichiers sont téléchargés, vous pouvez prendre le temps de sauvegarder vos données. Pour ce faire, il existe deux possibilités :

**Utiliser l'outil de sauvegarde de PrestaShop**

PrestaShop dispose de son propre outil de sauvegarde de données, nommé "Sauvegarde BDD" et situé dans le menu "Paramètres avancés". Cet outil est expliqué en détails dans le chapitre "Comprendre les paramètres avancés" du guide de l'utilisateur PrestaShop, mais en voici le principal :

1. Lisez l'avertissement, et cliquez sur "J'ai lu l'avertissement - Créer une sauvegarde". PrestaShop crée alors une archive zip de toutes les tables de votre base de données.
2. Cliquez sur le dernier fichier de sauvegarde dans le tableau sous l'avertissement. Votre navigateur se mettra alors à télécharger l'archive de sauvegarde, nommée sous la forme "`1349964600-71d48cfe.sql.bz2`". Enregistrez ce fichier dans votre dossier de sauvegarde.

**Utiliser phpMyAdmin**

Si vous préférez faire confiance à la fonctionnalité de sauvegarde de phpMyAdmin plutôt qu'à l'outil de PrestaShop, aucun problème ! Voici le processus à suivre :

1. Connectez-vous à phpMyAdmin sur votre serveur web.
2. Depuis l'écran principal sélectionnez "Bases de données".
3. Cliquez sur le nom de la base de données de PrestaShop afin de l'ouvrir.
4. Dans l'écran de la base de données, cliquez sur l'onglet "Exporter" en haut de l'écran.
5. Dans l'écran d'export :
   1. Assurez-vous que vous les tables de PrestaShop sont sélectionnées, et seulement celles-là. Elles devraient utiliser le préfixe `ps_` (ou le préfixe que vous avez choisi lors de l'installation de PrestaShop).
   2. Assurez-vous que l'option "SQL" est sélectionnée.
   3. Dans la section "Structure", cochez les cases suivantes :\

      * "Structure".
      * "Ajouter DROP TABLE / VIEW / PROCEDURE / FUNCTION".
      * "Ajouter IF NOT EXISTS".
      * "Ajouter AUTO\_INCREMENT".
      * "Entourer les noms des tables et des colonnes par des guillemets obliques".
   4. Dans la section "Données", cochez au moins la case suivante ::
      * "Données".
   5. Dans la section "Modèle de nom de fichier" :
      * Cochez "Diriger la sortie vers un fichier".
      * Laissez l'exemple tel quel (normalement, "`__DB__`").
      * Choisissez "zippé" ou "gzippé" pour la compression.
   6. Cliquez sur le bouton "Exécuter".
6. Le navigateur devrait lancer le téléchargement automatiquement. Enregistrez le fichier dans le dossier de sauvegarde de votre ordinateur.

Si votre serveur n'est pas assez puisant pour vous permettre d'exporter toutes vos tables d'un coup, divisez votre sauvegarde. Par exemple, choisissez les 20 premières tables `ps_` et exportez-les, en indiquant clairement dans le nom de fichier que c'est la première archive parmi plusieurs. Une fois que c'est tables ont été sauvegardées et sont en sûreté sur votre ordinateur, faites de mêmes pour les 20 tables suivantes, et ainsi de suit, en n'oubliant pas d'indiquer le numéro de l'archive dans son nom.

**À l'aide de l'outil de gestion de base de données de votre hébergeur**

Votre hébergeur peut ne pas vous donner accès à phpMyAdmin, et propose au lieu de cela soit un outil qui lui est propre, ou un autre outil moins connu, comme celui intégré au sein de cPanel. Lisez la documentation de votre hébergeur. L'objectif est d'exporter vos données au format SQL, dans une archive compressée ou non.

### Restaurer votre sauvegarde <a href="#faireunesauvegardeetlarestaurer-restaurervotresauvegarde" id="faireunesauvegardeetlarestaurer-restaurervotresauvegarde"></a>

Après qu'une mise à jour a échoué (ce qui est la seule raison pour laquelle vous devriez avoir recours à votre sauvegarde), si vous pouvez encore accéder à l'administration de PrestaShop et utiliser le module Mise à jour en 1 clic, utilisez l'outil de restauration de ce module afin de lancer le processus tant pour vos fichiers et vos données que le module a sauvegarde lorsque vous avez lancé la mise à jour automatique. Lisez le guide de la mise à jour automatique pour plus d'information sur ce processus.

Si vous ne pouvez pas accéder à l'administration ou au module, ou si vous n'avez simplement pas utilisé le module de Mise à jour en 1 clic pour passer à la dernière version de PrestaShop, suivez alors les instructions dans cette section.

Vous devez être connecté à l'administration de votre PrestaShop pour utiliser le module Mise à jour en 1 clic, et donc pour lancer la restauration de la version précédente - et sous certaines configuration imprévisibles, la mise à jour peut vous empêcher de vous reconnecter, ou peut même rendre l'administration de PrestaShop inutilisable (note : videz le cache du navigateur et rechargez l'administration plusieurs fois avant de décider que l'interface est inutilisable... Il s'agit peut-être simplement d'un problème CSS temporaire).

C'est la raison pour laquelle le module de mise à jour vous pousse à faire vos propres sauvegardes : avant de tenter la moindre mise à jour, vous devriez avoir sur votre disque dur une copie exacte de votre boutique. En résumé :

* Un dossier (ou une archive zip) contenant tous les fichiers de PrestaShop, en particulier ceux propres à votre installation : fichier de configuration, thèmes, modules, images, envois des clients, templates PDF et e-mail, classes personnalisées, etc.
* Une copie complète de votre base de données, au format SQL brut ou dans une archive zip.

Cette copie locale de votre site doit être extrêmement récente : au mieux, elle devrait être faite juste après avoir mis votre boutique en maintenance, et avant d'avoir lancé le script de mise à jour (que ce soit automatiquement ou manuellement). Ainsi, vous vous assurez de pouvoir revenir à la version la plus récente de votre boutique, et de ne pas perdre de données (clients, ventes, statistiques, etc.).

#### Nettoyer votre serveur <a href="#faireunesauvegardeetlarestaurer-nettoyervotreserveur" id="faireunesauvegardeetlarestaurer-nettoyervotreserveur"></a>

Vous disposez donc d'une copie complète et récente de votre boutique dans sa version précédente, et votre tentative mettre PrestaShop a jour à échoué, aboutissant à une administration inutilisable (le front-office devrait être inaccessible, étant donné que votre boutique est en mode de maintenance). Revenir à la version précédente signifie restaurer votre copie locale sur votre serveur en ligne, et cela implique de faire table rase afin d'éviter que les anciennes et nouvelles données ne se mélangent et ne cassent encore plus votre site.

Cela signifie donc de supprimer tous les fichiers PrestaShop de votre serveur, et toutes les tables PrestaShop de votre base de données.

Ne vous inquiétez pas : étant donné que ces fichiers et ces données sont déjà en sécurité sur votre ordinateur, vous allez pouvoir les restaurer rapidement. Mais vu que les clients continuent de venir sur votre boutique, vous devez afficher une page de maintenance personnalisée tandis que vous travaillez à restaurer votre boutique.

**Créer une page de maintenance**

Il vous faut prévoir du temps pour faire revenir votre boutique à sa version précédente, en fonction de la taille de celle-ci, c'est-à-dire en fonction du nombre de fichiers et de la quantité de données que vous devrez transférer. Il est donc important d'avoir une page de maintenance qui ne dépende pas de PrestaShop.

En effet, la page de maintenance actuellement en place repose sur PrestaShop pour afficher certaines informations : nom de la boutique, logo de la boutique, traduction, fichier CSS, méta données, etc. Même si votre boutique est actuellement en mode de maintenance, et affiche donc la page de maintenance à vos visiteurs, cette page ne fonctionnera plus dès que vous aura supprimé vos données... et ne sera même plus présente une fois que vous aurez supprimé vos fichiers, étant donné que la page de maintenance se trouve dans le thème actuel, sous le nom `maintenance.tpl`.

C'est pourquoi il vous faut une page de maintenance personnalisée. Elle n'a pas à être jolie ou bien faite, car son rôle consiste simplement à informer vos visiteurs, en leur demandant de revenir plus tard.

Voici un exemple très basique :**Exemple de page de maintenance**

```
<!DOCTYPE html>
<html>
  <head>
    <title>Our shop is under maintenance</title>    
  </head>
  <body>
    <p>In order to perform site maintenance, our online shop has shut down temporarily.</p>
    <p>We apologize for the inconvenience and ask that you please try again later.</p>
  </body>
</html>
```

Copiez ce code dans un fichier `index.html`, et mettez-la en ligne dans le dossier de PrestaShop à l'aide de votre logiciel FTP. Sur la plupart des serveurs, le fichier `index.html` prend le pas sur le fichier `index.php`, donc dès que vous aurez mis en ligne `index.html` dans le dossier racine de PrestaShop, votre boutique devrait afficher cette page de maintenance au lieu de celle de PrestaShop. Vérifiez les réglages de votre serveur pour vous en assurer.

**Supprimer les fichiers**

Connectez-vous à votre espace d'hébergement à l'aide de votre logiciel FTP. Allez dans le dossier de PrestaShop (s'il ne se trouve pas à la racine), sélectionnez tous les dossiers et fichiers du dossier de PrestaShop (sauf `index.html`, votre page de maintenance personnalisée) et supprimez-les tous. De toute évidence, vous ne devriez faire ceci que si vous êtes totalement certain d'avoir une copie exacte de vos fichiers sauvegardée sur votre serveur.

Cela peut prendre quelques minutes, car PrestaShop a plus de 7 000 fichiers. Tandis que la suppression se fait, allez effacer les tables de données (section suivante).

**Supprimer les données**

Ouvrez votre gestionnaire de base de données – normalement, votre hébergeur devrait vous en fournir un, comme phpMyAdmin ou un outil personnalisé. Ouvrez la base de données de votre installation de PrestaShop. Sélectionnez toutes les tables qui commencent par `ps_` (ou le préfixe de table que vous aurez choisi lors de l'installation de PrestaShop). Si PrestaShop est le seul outil utilisant la base de données, vous pouvez simplement cliquer sur lien "Tout cocher" en bas de la liste afin de faire une sélection instantanée.

Ouvrez ensuite le menu déroulant "Pour la sélection" en bas de tables, et sélectionnez "Supprimez". Sur l'écran suivant, phpMyAdmin vous demandera une confirmation : cliquez sur le bouton "Oui". Ici encore, vous ne devriez faire ceci que si vous êtes totalement certain d'avoir une copie exacte de vos données sauvegardée sur votre ordinateur.

Cela peut prendre quelques minutes. Une fois le processus terminé, phpMyAdmin affiche une base de données vide de toute table.

Votre serveur ne contient maintenant plus de fichiers ni de données liées à PrestaShop, en dehors du fichier de maintenance `index.html`. Il est maintenant temps de remettre votre boutique en ligne, cette fois avec des fichiers et données qui marchent !

#### Restaurer vos fichiers et données <a href="#faireunesauvegardeetlarestaurer-restaurervosfichiersetdonnees" id="faireunesauvegardeetlarestaurer-restaurervosfichiersetdonnees"></a>

Dès que votre logiciel FTP a terminé de supprimer les fichiers en ligne, commencez à mettre en ligne ceux que vous avez sauvegardé sur votre ordinateur ! Etant donné que ce processus peut prendre du temps, il est important de ne pas perdre de précieuses minutes (et donc autant de ventes potentielles) en gardant votre boutique hors ligne plus longtemps que nécessaire.

**Restaurer vos fichiers**

Ce processus est aussi simple que celui que vous avez suivi pour sauvegarder vos fichiers :

1. Connectez-vous à votre serveur web à l'aide d'un logiciel FTP, tel que FileZilla.
2. Mettez en ligne, dans le dossier de PrestaShop, tous les fichiers de votre dossier de sauvegarde local.

Le dossier en ligne de PrestaShop devrait être vide, afin de s'assurer qu'anciens et nouveaux fichiers n'entrent pas en conflit. Si vous n'avez supprimé aucun fichier en ligne (après les avoir sauvegardé, bien entendu), vous devez dire à votre logiciel FTP de réécrire par-dessus tous ces fichiers existants. Vous ne devez garder aucune trace des fichiers provenant de la mise à jour qui a échoué.

**Restaurer vos fichiers**

Le processus décrit ici utilise phpMyAdmin, qui est un outil standard. Si votre hébergeur vous oblige à utiliser un outil pour gérer vos bases de données, vous devrez adapter ce processus à cet outil. Consultez la documentation de votre hébergeur sur le sujet.

Le processus de restauration des données est aussi simple que celui utilisé pour sauvegarder les données :

1. Connectez-vous à phpMyAdmin sur votre serveur web.
2. Depuis l'écran principal sélectionnez "Bases de données".
3. Cliquez sur le nom de la base de données de PrestaShop afin de l'ouvrir.
4. Dans l'écran de la base de données, cliquez sur l'onglet "Importer" en haut de l'écran.
5. Dans l'écran d'import :
   1. Dans la section "Fichier à importer", cliquez sur "Parcourir..." et trouvez le fichier de sauvegarde de vos données. Il peut s'agir de commande SQL brutes (`.sql`), ou une version compressée (`.sql.zip`, `.sql.gzip`, `.sql.tar.gz`, etc.).
   2. Dans la section "Format", choisissez bien "SQL".
   3. Cliquez sur le bouton "Exécuter".
6. Le navigateur devrait lancer la mise en ligne automatiquement.

Si vous avez plus d'un fichier de sauvegarde, importez-les l'un après l'autre.

Enfin, enlevez votre fichier de maintenance (nommé `index.html`). Et voilà : votre boutique est de retour en ligne !
