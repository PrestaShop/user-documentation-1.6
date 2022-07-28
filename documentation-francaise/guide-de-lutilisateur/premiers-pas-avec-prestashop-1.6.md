# Premiers pas avec PrestaShop 1.6

**Contenu**

* [Premiers pas avec PrestaShop 1.6](premiers-pas-avec-prestashop-1.6.md#PremierspasavecPrestaShop1.6-PremierspasavecPrestaShop1.6)
  * [Désactiver votre boutique](premiers-pas-avec-prestashop-1.6.md#PremierspasavecPrestaShop1.6-Désactivervotreboutique)
  * [Effacer le contenu de la boutique par défaut](premiers-pas-avec-prestashop-1.6.md#PremierspasavecPrestaShop1.6-Effacerlecontenudelaboutiquepardéfaut)
  * [Configurer les informations de votre boutique](premiers-pas-avec-prestashop-1.6.md#PremierspasavecPrestaShop1.6-Configurerlesinformationsdevotreboutique)
    * [Réglages de base de la boutique](premiers-pas-avec-prestashop-1.6.md#PremierspasavecPrestaShop1.6-Réglagesdebasedelaboutique)
    * [Langues de la boutique](premiers-pas-avec-prestashop-1.6.md#PremierspasavecPrestaShop1.6-Languesdelaboutique)
    * [Informations sur les employés](premiers-pas-avec-prestashop-1.6.md#PremierspasavecPrestaShop1.6-Informationssurlesemployés)
  * [Configurer les méthodes de paiement](premiers-pas-avec-prestashop-1.6.md#PremierspasavecPrestaShop1.6-Configurerlesméthodesdepaiement)
  * [Configurer le transport](premiers-pas-avec-prestashop-1.6.md#PremierspasavecPrestaShop1.6-Configurerletransport)
  * [Choisir votre thème](premiers-pas-avec-prestashop-1.6.md#PremierspasavecPrestaShop1.6-Choisirvotrethème)
  * [Choisir vos modules](premiers-pas-avec-prestashop-1.6.md#PremierspasavecPrestaShop1.6-Choisirvosmodules)
  * [Créer des produits et des catégories de produits](premiers-pas-avec-prestashop-1.6.md#PremierspasavecPrestaShop1.6-Créerdesproduitsetdescatégoriesdeproduits)
  * [Créer du contenu statique](premiers-pas-avec-prestashop-1.6.md#PremierspasavecPrestaShop1.6-Créerducontenustatique)
  * [Construire votre menu](premiers-pas-avec-prestashop-1.6.md#PremierspasavecPrestaShop1.6-Construirevotremenu)
  * [Activez votre boutique](premiers-pas-avec-prestashop-1.6.md#PremierspasavecPrestaShop1.6-Activezvotreboutique)

## Premiers pas avec PrestaShop 1.6 <a href="#premierspasavecprestashop1.6-premierspasavecprestashop1.6" id="premierspasavecprestashop1.6-premierspasavecprestashop1.6"></a>

Il vous faut prendre le temps de vous assurer que toutes les fonctionnalités de votre future boutique sont bien en place, validées et prêtes à prendre vos premières commandes.

PrestaShop facilite grandement la création d'une boutique en ligne, mais pas au point de pouvoir se mettre à vendre des produits dès les premières minutes suivant l'installation : ici, vous avez affaire à des produits, des clients, et surtout à un réel échange de devises, qui devront circuler de vos clients vers votre compte bancaire. De toute évidence, vous préféreriez qu'aucune faille ne vienne empêcher les transactions d'être validées, les produits d'être trouvés dans votre entrepôt et envoyés à vos clients sans erreur, ou même que quoi que ce soit d'inattendu n'arrive sans que vous ne soyez tenu au courant.

PrestaShop est un outil très complet, et l'étendue des possibilités peut sembler écrasante. Nous avons créé ce chapitre afin de vous aider à réaliser les principales actions à mettre en place pour préparer votre boutique à son grand lancement. Beaucoup de choses peuvent être faites avant l'ouverture des ventes, mais ces étapes sont essentielles pour n'importe quel type de boutique.

### Désactiver votre boutique <a href="#premierspasavecprestashop1.6-desactivervotreboutique" id="premierspasavecprestashop1.6-desactivervotreboutique"></a>

Nous allons partir du principe que vous venez tout juste d'installer PrestaShop, et comptez l'utiliser en mode monoboutique.

Désactiver votre boutique signifie que vous serez le seul à y avoir accès tout du long de votre mise en place du site : changer le thème, installer des modules, ajouter des produits et régler leurs prix et les taxes, configurer des transporteurs... Cette opération s'appelle "la mise en maintenance de la boutique."

![](../../.gitbook/assets/23038236.png)

Dans votre back-office, rendez-vous dans la page "Préférences / Maintenance". Il contient deux réglages :

* **Activer la boutique**. Choisissez "Non", et l'accueil de votre site affichera la page de maintenance à vos visiteurs, qui indique simplement que votre site sera bientôt de retour.
* **IP de maintenance**. C'est ici que vous devez saisir votre propre adresse IP, afin de toujours pouvoir accéder à votre boutique et parcourir les pages, pour vérifier que tout est bien en place. Cette option doit être remplie à chaque fois que vous mettez votre boutique en mode de maintenance, étant donné que vous aurez toujours besoin de vos pages publiques pour vérifier que tout es bien en place.

Si vous avez déjà mis en place votre thème et vos produits, vous pouvez simplement passer votre boutique en mode Catalogue. Ainsi, vos visiteurs pourront parcourir les pages de votre boutique, mais aucun prix ne sera affiché, et ils ne pourront rien acheter tant que vous ne serez pas sorti du mode Catalogue.

Pour activer le mode Catalogue, rendez-vous dans la page "Préférence / Produits", dont c'est le premier réglage.

![](../../.gitbook/assets/23038238.png)

### Effacer le contenu de la boutique par défaut <a href="#premierspasavecprestashop1.6-effacerlecontenudelaboutiquepardefaut" id="premierspasavecprestashop1.6-effacerlecontenudelaboutiquepardefaut"></a>

L'installation par défaut de PrestaShop comprend une poignée de produits, pour la plupart des produits Apple accompagné d'accessoires tiers. Leur seul intérêt est de vous permettre d'explorer et comprendre la mise en place d'une boutique fonctionnelle. Après avoir appris les subtilités des liens entre produits, catégories, commandes et clients, vous devriez effacer tout ce contenu initial afin de partir d'une base saine et propre.

![](../../.gitbook/assets/23038240.png)

Vous devez donc effacer toutes les données par défaut, c'est à dire :

* les produits et leurs...
  * catégories
  * attributs
  * caractéristiques
  * marques
  * fournisseurs
  * scènes
  * tags
* les commandes
  * les messages liés aux commandes
* les clients
  * leurs paniers
* les transporteurs
  * les tranches de prix
  * les tranches de poids
* Les infos de contact et les magasins (à effacer ou à adapter aux besoins de la boutique)
* les pages de contenu CMS (à effacer ou à adapter aux besoins de la boutique)

Cela supposerait que vous ayez à parcourir les nombreux écrans du back-office et supprimer votre contenu sur chaque écran, mais il y a une méthode bien plus facile :

1. Allez dans la page "Modules > Modules",
2. Trouvez le module "Nettoyage de la base de données" (Database Cleaner) et cliquez sur son bouton "Installation",
3. Vous êtes immédiatement envoyé sur sa page de configuration (si ce n'est pas le cas, cliquez sur son bouton "Configuration"),
4. Lisez et acceptez l'avertissement, puis cliquez sur le bouton "Effacer le catalogue" : il supprimera tous vos produits et vos attributs, vos fabricants, etc.
5. Lisez et acceptez l'avertissement, puis cliquez sur le bouton "Effacer les commandes et clients" : il supprimera toutes vos clients et leurs commandes, paniers, etc.
6. Cliquez sur le bouton "Vérifier et corriger" pour rétablir les contraintes d'intégrité de votre base de données,
7. Cliquez sur le bouton "Nettoyer et optimiser" pour réorganiser le stockage physique des données de vos tables et les index de données associées, afin de réduire l'espace de stockage et améliorer l'efficace de lecture/écriture lors de l'accès aux tables.

VOS MODIFICATIONS SONT DÉFINITIVES. Assurez-vous de ne cliquez sur ces boutons que si vous souhaitez vraiment effacer le contenu par défaut de votre base de données.

### Configurer les informations de votre boutique <a href="#premierspasavecprestashop1.6-configurerlesinformationsdevotreboutique" id="premierspasavecprestashop1.6-configurerlesinformationsdevotreboutique"></a>

Maintenant que vous disposez d'une boutique propre, vous pouvez commencer à en prendre possession, et cela implique de tout mettre à votre goût, à commencer par vos informations personnelles et vos préférences.

#### Réglages de base de la boutique <a href="#premierspasavecprestashop1.6-reglagesdebasedelaboutique" id="premierspasavecprestashop1.6-reglagesdebasedelaboutique"></a>

Vous devriez faire attention aux réglages suivants, qui sont importants car ils ont un impact direct sur le front-office, et donc que vos clients les voient.

Certains de ces réglages nécessitent que vous configuriez un module plutôt que de changer les préférences de PrestaShop.

Un module se configure très facilement :

1. Allez dans le menu "Modules".
2. Saisissez le nom du module (ou même une partie) dans le moteur de recherche des modules. Les résultats devraient s'afficher dès que vous saisissez des lettres.
3. Une fois que vous avez trouvé le bon module, cliquez sur son bouton "Configurer", et suivez les instructions.

Pour chaque module présenté ici, vous devriez lire leur documentation pour avoir plus d'information.

| Réglage                                               | Description                                                                                                                                                                                                                                                                                                                                                                                                                                | Emplacement dans le back-office                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| ----------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Nom de la boutique                                    | Définit votre marque, notamment auprès des moteurs de recherche.                                                                                                                                                                                                                                                                                                                                                                           | Menu "Préférences", page "Coordonnées & magasins", puis dans la section "Coordonnées", modifiez le champ en question.                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| Logo de la boutique                                   | <p>Définit votre marque visuellement. Le logo par défaut se lit "YourLogo" pour vous pousser à utiliser le vôtre.<br>Affiché en haut à gauche de toutes les pages de la boutique, ainsi que sur vos factures et vos e-mails automatiques.</p>                                                                                                                                                                                              | Menu "Préférences", page "Thèmes", section "Apparence", puis changez les différents logos.                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| Devise par défaut de la boutique                      | La monnaie dans laquelle vous allez saisir les prix par défaut de vos produits.                                                                                                                                                                                                                                                                                                                                                            | <p>Menu "Localisation", page "Localisation", section "Configuration".<br>Si la devise n'est pas disponible, vous devez en premier lieu importer le pack de localisation de son pays : utilisez l'outil "Importer le pack de localisation" de cette même page.</p>                                                                                                                                                                                                                                                                                                        |
| Informations du SAV                                   | <p>Un bloc présentant le numéro de téléphone votre service clientèle et un bouton permettant de vous envoyer un mail.<br>Affiché sur le front-office, dans la colonne de droite.</p>                                                                                                                                                                                                                                                       | Module "Bloc contact".                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| Informations de contact / Informations sur la société | <p>Un bloc présentant votre adresse de contact, le numéro de téléphone votre service clientèle et un lien permettant de vous envoyer un mail.<br>Affiché dans le pied de page.</p>                                                                                                                                                                                                                                                         | Module "Bloc informations de contact".                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| Publicité                                             | <p>Un bloc présentant une image avec un lien vers un autre site.<br>Affiché dans la colonne de gauche.</p>                                                                                                                                                                                                                                                                                                                                 | Module "Bloc publicités".                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| Carrousel d'images (slider)                           | <p>Le carrousel d'image présente plusieurs images qui défilent l'une après l'autre. C'est une signature visuelle forte de votre boutique et de vos produits.<br>Généralement placé au centre de la page d'accueil.</p>                                                                                                                                                                                                                     | Module "Carrousel d'image (slider)".                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| Page CMS                                              | <p>Il s'agit des pages statiques, telles que les pages "À propos", "Livraison", "Mentions légales", "Conditions générales de vente" et "Paiement sécurisé". La plupart d'entre elles ont un contenu par défaut, que vous devez adapter à vos besoins ; d'autres sont vides, et vous devez ajouter votre propre texte.<br>Affichées dans le bloc "Information" de la colonne de gauche, et dans la zone "Informations" du pied de page.</p> | Menu "Préférences", page "CMS", puis modifiez et créez des pages selon vos besoin.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| Réseaux sociaux                                       | <p>Un bloc présentant trois liens : la page Facebook de votre société, le compte Twitter de votre société, et le flux RSS du blog (ou site d'actualités) de votre société.<br>Par défaut, tous ces liens sont ceux de la société PrestaShop. Il est donc important d'indiquer les vôtres.<br>Affichés dans la section "Nous suivre" du pied de page.</p>                                                                                   | Module "Bloc social".                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| Menu principal                                        | Le haut du thème par défaut utilise un menu pour indiquer les catégories que le visiteur peut parcourir, ainsi que des liens vers d'autres adresses web – par exemple, l'installation par défaut a un lien "Blog" qui renvoie vers le blog de PrestaShop.                                                                                                                                                                                  | Module "Menu Haut horizontal".                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| Contenu de la page d'accueil                          | Le thème par défaut contient beaucoup de contenu d'exemple : textes, images, liens, etc. Si vous souhaitez utiliser ce thème pour votre propre boutique au lieu d'installer le vôtre, vous devriez faire en sorte d'enlever avant tout ce contenu par défaut.                                                                                                                                                                              | <p>Module "Configurateur du thème" : ce module gère beaucoup de choses sur votre thème. Il permet principalement d'activer/désactiver des fonctionnalités (boutons de partage, bannière supérieure, logos de paiement, etc.), et, plus important encore, il vous permet d'ajouter ou changer les images de votre page d'accueil.</p><p>Module "Bloc CMS d'information client" : ce module vous aider à gérer les deux derniers blocs en bas de la page d'accueil, juste avant le pied de page : le bloc "Livraison gratuite" et celui avec le contenu personnalisé..</p> |

Ce sont là les modifications à faire qui sont les plus visibles sur votre front-office – au moins pour le thème par défaut.\
La colonne "Emplacement" vous permet de savoir où trouver l'interface permettant de modifier ces aspects de votre boutique. Ce guide de l'utilisateur vous donnera plus de détail sur chaque interface.

#### Langues de la boutique <a href="#premierspasavecprestashop1.6-languesdelaboutique" id="premierspasavecprestashop1.6-languesdelaboutique"></a>

PrestaShop peut fonctionner dans de nombreuses langues, à la fois côté client et côté administration. Dès que plus d'une langue est activée dans le back-office, chaque champ textuel du back-office est accompagné d'une icône de drapeau, qui indique la langue actuelle, et sur lequel vous pouvez cliquer pour insérer le contenu de ce champ dans une autre langue.

![](../../.gitbook/assets/23038242.png)

Par défaut, PrestaShop n'est installé qu'avec deux langues : celle utilisée lors de l'installation, et le français. Vous pouvez facilement en ajouter d'autres : dans le menu "Localisation", choisissez la page "Langues". Celle-ci s'ouvre avec un tableau des langues disponibles.

![](../../.gitbook/assets/23038244.png)

La langue actuellement activée est indiqué avec une coche verte, tandis que les autres ont une croix rouge. Cliquez sur n'importe quelle de ces croix rouges pour activer la langue correspondante.

Vous pouvez activer toutes les langues disponibles si vous estimez que votre boutique en a besoin, mais gardez en mémoire que vous devrez traduire votre contenu pour toutes les langues disponibles : nom du produit, description, tags, nom de catégorie, contenu statique (CMS), réglages de modules, etc.

Vous pouvez facilement importer de nombreuses autres langues en passant par la page "Localisation / Localisation", puis les activer en passant par la page "Localisation / Langues".

#### Informations sur les employés <a href="#premierspasavecprestashop1.6-informationssurlesemployes" id="premierspasavecprestashop1.6-informationssurlesemployes"></a>

Si des personnes vous aident à gérer votre boutique, qu'il s'agisse de votre conjoint, d'amis ou d'employés payés, il vous faut leur créer un compte personnel d'administration, ne serait-ce que pour savoir qui a lancé une action donnée (prise de commande, par exemple). L'autre avantage est que vous pouvez leur créer des profils précis, avec des droits d'accès précis pour les pages d'administration : par exemple, il se peut que vous préfériez limiter l'accès à vos statistiques, vos factures ou vos paiements.\
Vous pouvez créer autant de profils que nécessaire.

Pour créer un compte d'employé", allez dans le menu "Administration", ouvrez la page "Employés", et cliquez sur le bouton "Créer". Donnez-lui un nom, comme "Martin Dupont" ou "Responsable commandes", et enregistrez le compte.\
Un profil peut être utilisé par autant de comptes que nécessaires – mais nous vous recommandons d'en créer un par personne.

Maintenant que l'employé dispose d'un compte personnel, vous pouvez lui assigner un profil avec des permissions spécifiques, réservées aux activités de ce compte. Par défaut, un nouveau profil ne peut pas faire grand-chose. Il vous revient de faire les réglages précis qui correspondent aux besoins quotidiens de ce profil. Cela peut s'avérer laborieux, mais c'est nécessaire.\
Pour assigner des permissions à un compte d'employé, vous devez utiliser l'option "Profil" de la page de création du compte : ce menu vous permet de sélectionner le profil du compte (SuperAdmin, Traducteur, etc.).

![](../../.gitbook/assets/23038246.png)

Vous pouvez modifier les permissions d'un profil de la manière suivante : allez dans la page "Permissions" du menu "Administration", et choisissez le profil que vous voulez modifier. Une longue liste de permissions apparaît alors : modifiez-les comme bon vous semble. Vos modifications sont enregistrées automatiquement.

### Configurer les méthodes de paiement <a href="#premierspasavecprestashop1.6-configurerlesmethodesdepaiement" id="premierspasavecprestashop1.6-configurerlesmethodesdepaiement"></a>

Vous ouvrez une boutique pour gagner de l'argent, et cela ne peut se faire que si vous utilisez au moins un module de paiement. 16 modules sont disponibles dans l'installation par défaut, que vous pouvez installer et configurer (à partir de la catégorie "Paiement" de la page des modules, dans le menu "Modules"), et leur créer des restrictions (dans la page "Paiement" du menu "Modules"). Pour de nombreux modules, vous devrez créer un compte sur le service pour lequel ils ont été conçus.

Le chapitre "Faire fonctionner les modules natifs" vous explique tout sur ces modules dans sa section "Paiement".

Vous pouvez installer d'autres modules en les téléchargeant depuis le site Addons : [http://addons.prestashop.com/fr/4-modules-paiement-prestashop](http://addons.prestashop.com/fr/4-modules-paiement-prestashop).

Le paiement par chèque ou par virement bancaire sont les deux seules méthodes installées par défaut. Si vous choisissez de les conserver, vous **devez** les configurer avec vos informations : ordre du chèque et adresse où l'envoyer, détails bancaires (compte, IBAN, BIC, etc.).

Vous pouvez configurer ces deux méthodes de paiements en passant par les modules "Virement bancaire" et "Paiement par chèque", que vous trouverez la catégorie "Paiement" de la liste de modules.

### Configurer le transport <a href="#premierspasavecprestashop1.6-configurerletransport" id="premierspasavecprestashop1.6-configurerletransport"></a>

Les produits vendus sur votre boutique doivent être expédiés à vos clients – à moins que vous ne vendiez que des produits téléchargeables, auquel cas le menu "Transport" ne vous sera pas d'une grande utilité.

Que vous expédiez vos produits par courrier normal ou que vous disposiez d'un contrat chez un transporteur, vous devez enregistrer cette information dans PrestaShop.

Le chapitre "Gérer le transport" de ce guide vous apprendre tout ce qu'il y a à savoir sur ce menu.

Le retour marchandise n'est pas activé par défaut. Si vous voulez autoriser vos clients à vous renvoyer des produits et à recevoir un bon d'achat ou un remboursement en retour, vous devez activez l'option "Activer les retours" qui se trouve dans la page "Retours produits" du menu "Commandes".

### Choisir votre thème <a href="#premierspasavecprestashop1.6-choisirvotretheme" id="premierspasavecprestashop1.6-choisirvotretheme"></a>

Votre boutique doit disposer de son propre thème pour se distinguer des autres et être reconnaissable au premier coup d'oeil. La dernière chose que vous voulez est que les visiteurs confondent votre boutique avec une autre.

Il y a des nombreux thèmes à acheter sur le site Addons : [http://addons.prestashop.com/fr/3-themes-prestashop](http://addons.prestashop.com/fr/3-themes-prestashop).

Vous pouvez également créer votre propre thème, ou le faire créer par un développeur. Pour savoir comment, rendez-vous sur le Guide de l'Intégrateur PrestaShop.

Une fois votre thème installé, vous devriez en parcourir toutes les pages afin de le connaître par coeur et de pouvoir aider les clients perdus.

Vous pouvez et même devez personnaliser certains aspects du thème, à commencer par le logo dans ses différentes variations (en-tête, e-mail, facture, etc.). Pour ce faire, rendez-vous sur la page "Thèmes" du menu "Préférences".

### Choisir vos modules <a href="#premierspasavecprestashop1.6-choisirvosmodules" id="premierspasavecprestashop1.6-choisirvosmodules"></a>

L'installation par défaut de PrestaShop comprend une centaine de modules. Ils sont très variés : statistiques, bloc du front-office, paiement, expédition... Vous devriez les explorer pleinement, afin de voir lesquels vous souhaitez activer, et lesquels vous préférez garder désactivés.

Lisez les chapitres "Gérer les modules" et "Faire fonctionner les modules natifs" pour en apprendre plus.

Vous trouverez par ailleurs de nombreux modules sur le site Addons : [http://addons.prestashop.com/fr/2-modules-prestashop](http://addons.prestashop.com/fr/2-modules-prestashop).

Chaque fois que vous activez et configurez un module, assurez-vous qu'il fonctionne bien avec le thème que vous avez choisi, dans le cas où ses fonctionnalités ont un impact sur le front-office.

### Créer des produits et des catégories de produits <a href="#premierspasavecprestashop1.6-creerdesproduitsetdescategoriesdeproduits" id="premierspasavecprestashop1.6-creerdesproduitsetdescategoriesdeproduits"></a>

Lisez le chapitre "Ajouter des produits et des catégories de produits".

### Créer du contenu statique <a href="#premierspasavecprestashop1.6-creerducontenustatique" id="premierspasavecprestashop1.6-creerducontenustatique"></a>

Si vous ne l'avez pas déjà fait, prenez le temps d'écrire le contenu de quelques pages CMS, soit pour celles qui sont déjà disponibles dans l'installation par défaut, soit pour celles que vous estimez nécessaire de créer.

Certaines pages existent déjà, mais leur contenu doit être vérifié et revérifié, car ces pages peuvent avoir un impact fort sur le statut légal de votre boutique, entre autres choses.

Les pages par défaut sont "À propos", "Conditions d'utilisation", "Mentions légales", "Livraison", "Paiement sécurisé". Certaines d'entre elles ont du contenu par défaut, que vous devez adapter à vos besoins ; les autres sont vides, et vous devriez y mettre du texte.\
Pour modifier ces pages, allez dans la page "CMS" du menu "Préférences", puis choisissez la page que vous voulez modifier, ou en créez-en de nouvelles.

Vous pouvez créer autant de pages que nécessaire.

### Construire votre menu <a href="#premierspasavecprestashop1.6-construirevotremenu" id="premierspasavecprestashop1.6-construirevotremenu"></a>

Maintenant que vous disposez de catégories de produit et de pages CMS, vous pouvez les ranger dans un ordre logique ou cohérent dans le menu de votre boutique.

Pour ce faire, vous devez passer par le menu "Menu Haut horizontal", qui se trouve dans la catégorie "Fonctionnalités front-office" de la liste de modules. Activez-le si ce n'est pas déjà le cas, puis configurez-le : enlevez les pages ou catégories qui ne vous semblent pas nécessaires, ajoutez-y d'autres pages, et déplacez le contenu jusqu'à être satisfait de votre menu.

### Activez votre boutique <a href="#premierspasavecprestashop1.6-activezvotreboutique" id="premierspasavecprestashop1.6-activezvotreboutique"></a>

Maintenant que tout est fait, vous pouvez enfin lancer publiquement votre boutique.

Allez dans la page "Maintenance" du menu "Préférences", et modifiez deux réglages :

* **Activer la boutique**. Remettez-le à "Oui".
* **IP de maintenance**. Retirez l'adresse IP. Cette modification est facultative : votre boutique marchera même si vous laissez votre IP dans le champ.

Votre boutique devrait maintenant être prête à accueillir ses premiers visiteurs... et prendre ses premières commandes !
