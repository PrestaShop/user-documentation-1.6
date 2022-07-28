# Modules Transporteur et logistique

## Affiliation - Accès boutique <a href="#modulestransporteuretlogistique-affiliation-accesboutique" id="modulestransporteuretlogistique-affiliation-accesboutique"></a>

Ce module apporte à PrestaShop une solution d'affiliation intégré, qui permet à vos affiliés d'accéder à leurs propres statistiques.

L'outil de programme d'affiliation est situé dans la page "Sites affluents " du menu "Statistiques". Une fois que vous avez installé le module "Affiliation - Accès boutique", ces filiales peuvent accéder à leurs statistiques en allant à l'adresse [http://www.exemple.com/modules/trackingfront/stats.php](http://www.exemple.com/modules/trackingfront/stats.php).

Pour créer un nouvel affilié, cliquez sur le bouton "Créer", et dans le formulaire de création, ajoutez le nom d'utilisateur et le mot de passe du compte d'affiliation, puis spécifiez la commission qu'ils reçoivent par clic, par commande ou par pourcentage du chiffre d'affaires.

Cliquez sur l'en-tête de la section "Aide" pour afficher des instructions sur la façon de configurer l'URL de provenance.

La section "Informations techniques - Mode expert" vous permet d'utiliser des expressions régulières au lieu d'URL en texte clair.

## Date de livraison <a href="#modulestransporteuretlogistique-datedelivraison" id="modulestransporteuretlogistique-datedelivraison"></a>

Ce module affiche une date approximative de livraison durant le processus de commande.

La page de configuration comporte deux sections:

* **Configuration de transporteur**. Le module s'appuie sur les indications de vos transporteurs. Vous devez donc ajouter des règles pour chacun de vos transporteurs, en cliquant sur le lien "Ajouter une nouvelle règle de transporteur".
* Plus d'options :
  * **Temps supplémentaire lorsqu'un produit est hors stock**. Donnez une estimation du temps qu'il faudra pour que votre équipe re-stocke ses produits. Ce n'est vraiment utile que si les clients peuvent commander les produits hors-stock (l'option se trouve dans la page de préférence "Produits", dans la section "Stock produits").
  * **Temps supplémentaire pour la préparation des commandes**. Donnez une estimation du temps qu'il faudra pour que votre équipe prépare une commande.
  * **Option pour la préparation**. Si votre équipe d'emballage travaille également le week-end, indiquez-le, car le module le prend en compte.
  * **Format de la date**. Le format dans lequel la date de livraison prévue est affichée. Il utilise le format de la fonction `date()` de PHP : chaque lettre a un sens, comme expliqué dans le lien indiqué. La valeur par défaut, "l j F Y", signifie que la date sera affichée dans le format "Samedi 21 Janvier 2012". Il y a beaucoup plus de lettres que vous pouvez utiliser pour créer le format de date qui vous convient.

Il est facile d'ajouter une nouvelle règle transporteur :

* **Transporteur**. Choisissez le transporteur pour lequel vous souhaitez ajouter la règle.
* **Livraison entre**. Réglez le délai dans lequel le transporteur choisi annonce pouvoir livrer des produits. Vous devez recueillir cette information auprès du transporteur lui-même.
* **Option de livraison**. Certains transporteurs livrent également les jours de week-end. N'oubliez pas de l'indiquer le cas échéant.

Vous devez créer autant de règles transporteur que nécessaire.

## Estimation des livraisons <a href="#modulestransporteuretlogistique-estimationdeslivraisons" id="modulestransporteuretlogistique-estimationdeslivraisons"></a>

Ce module permet au client de comparer les transporteurs avant de poursuivre le processus de commande.

Ce module est très simple : il suffit de l'installer pour pouvoir afficher son option sur votre front-office.

Tous les transporteurs disponibles doivent avoir leurs tarifs réglés correctement. Cela se fait en bas de la page "Transport", dans la section "Frais par transporteurs, zones et tranches".

La page de configuration du module a une seule option, "Méthode de rafraîchissement de la liste des transporteurs". Cela vous permet d'afficher un transporteur, soit uniquement quand toutes les informations sont en place, ou dès que possible.

## Kiala avancé <a href="#modulestransporteuretlogistique-kialaavance" id="modulestransporteuretlogistique-kialaavance"></a>

Ce module permet à vos clients de faire livrer leurs colis dans un point de collecte Kiala. Les points Kiala sont largement disponibles en France, ainsi que dans certains autres pays européens.

Vous devez disposer d'un compte Kiala afin de pouvoir utiliser ce module. Vous pouvez accéder au formulaire d'inscription ici : [http://www.kiala.com/](http://www.kiala.com/).\
&#x20;Ensuite, configurez le module avec toutes les informations sur vous et votre boutique dans le formulaire de la section "Statut du module Kiala".\
&#x20;La section "Réglages par pays", située plus bas, vous permet d'indiquer les pays où vous voulez rendre disponible la livraison Kiala pour vos clients.\
&#x20;Enfin, la section "Réglages avancés de Kiala" ajoute quelques options supplémentaires:

* **Dossier d'export**. Le dossier local dans lequel le module enregistrera ses exportations, contenant une foule de renseignements utiles.
* **Préfixe pour les numéros des commandes**. Vous pouvez avoir un préfixe spécifique à votre boutique, ce qui donne un aspect plus personnalisé pour vos clients.
* **Exporter à chaque commande ?**. Vous préférerez peut-être avoir plusieurs fichiers d'exportation spécifiques à la commande plutôt qu'un seul grand fichier.
* **Critère de suivi des paquets ?**. Le colis doit-il être suivi en fonction du client ou en fonction de la commande? Si vous n'êtes pas sûr, garder le réglage "par commande".

Une fois que les paramètres sont en place, vos clients verront l'option "Kiala" apparaître sur le front-office de votre boutique, dans la section des modes de livraison disponibles.

## Mondial Relay <a href="#modulestransporteuretlogistique-mondialrelay" id="modulestransporteuretlogistique-mondialrelay"></a>

Ce module vous permet d'afficher le prix de livraison dans les points Mondial Relay. Ce service est disponible en France, au Luxembourg, en Espagne et en Belgique.

Vous devez avoir un compte Mondial Relay pour utiliser ce service. Vous pouvez accéder au formulaire d'inscription ici : [http://www.mondialrelay.com/](http://www.mondialrelay.com/).\
&#x20;Puis, à partir de la page de configuration du module, cliquez sur l'icône "Détails du compte" et saisissez les informations nécessaires, comme indiqué par Mondial Relay : Enseigne Webservice, Code Marque, Clé Webservice, Langue des étiquettes et Coefficient de Poids. La Langue des étiquettes peut utiliser uniquement les langues qui sont activées sur votre boutique ; vous pouvez activer d'autres langues sur la page "Langues" du menu "Localisation". Cliquez sur "Mettre à jour le compte" afin de connecter votre boutique au webservice Mondial Relay, et à partir de là, suivez les instructions du module dans l'écran "Transporteur" et "Paramètres avancés".

Une fois que les paramètres sont en place, vos clients verront l'option "Mondial Relay" apparaître sur le front-office de votre boutique, dans la section des modes de livraison disponibles.

## So Colissimo <a href="#modulestransporteuretlogistique-socolissimo" id="modulestransporteuretlogistique-socolissimo"></a>

Ce module vous permet d'afficher les tarifs des livraisons via SoColissimo, un service de La Poste, le service postal historique de la France. Ce service est disponible principalement en France.

Vous devez avoir un compte SoColissimo pour utiliser ce module. Cela se fait en appelant La Poste à partir d'un téléphone français, en utilisant le numéro suivant : **3634**.\
&#x20;Ensuite, configurez le module avec vos informations SoColissimo : Identifiant FO, clé de cryptage, temps de préparation, surcoût, URL FO, Fancybox, supervision et adresse de vérification.\
&#x20;Une documentation complète est disponible (en français) sous forme de fichier PDF, que vous pouvez trouver sous le lien "Documentation" de la page de configuration.

Afin de finaliser l'installation, copiez / collez les deux dernières URL dans votre back-office SoColissimo.

Une fois que les paramètres sont en place, vos clients verront l'option "SoColissimo" apparaître sur le front-office de votre boutique, dans la section des modes de livraison disponibles.

## TNT Express <a href="#modulestransporteuretlogistique-tntexpress" id="modulestransporteuretlogistique-tntexpress"></a>

Ce module vous permet d'afficher le prix de livraison via TNT Express. Ce service est disponible dans le monde entier.

Vous devez avoir un compte TNT pour utiliser ce module. Vous pouvez accéder au formulaire d'inscription ici : [http://www.tnt.fr/](http://www.tnt.fr/).\
&#x20;Ensuite, configurez le module avec votre Identifiant TNT, votre mot de passe et votre numéro de compte, le tout dans l'onglet "Paramètres du compte".\
&#x20;A partir de là, vous pouvez continuer de configurer le module en utilisant les onglets "Adresse d'expédition" et "Mode de livraison". Ce dernier onglet vous permet d'être très précis sur le service de livraison que vous souhaitez proposer à vos clients, ainsi que tout supplément que vous pourriez réclamer en fonction du prix du colis.\
&#x20;Une fois que les paramètres sont en place, vos clients verront l'option "Buyster" apparaître sur le front-office de votre boutique, dans la section des modes de livraison disponibles.
