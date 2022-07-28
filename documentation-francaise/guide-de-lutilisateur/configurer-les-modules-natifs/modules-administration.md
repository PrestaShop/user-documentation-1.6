# Modules Administration

/\*\<!\[CDATA\[\*/\
div.rbtoc1597053590228 {padding: 0px;}\
div.rbtoc1597053590228 ul {list-style: disc;margin-left: 0px;}\
div.rbtoc1597053590228 li {margin-left: 0px;padding-left: 0px;}\
\
/\*]]>\*/

* [Modules Administration](modules-administration.md#ModulesAdministration-ModulesAdministration)
  * [1-Click Upgrade - AutoUpgrade](modules-administration.md#ModulesAdministration-1-ClickUpgrade-AutoUpgrade)
  * [Conformité européenne améliorée](modules-administration.md#ModulesAdministration-Conformitéeuropéenneaméliorée)
    * [Libellés](modules-administration.md#ModulesAdministration-Libellés)
    * [Fonctionnalités](modules-administration.md#ModulesAdministration-Fonctionnalités)
    * [Gestion des contenus légaux](modules-administration.md#ModulesAdministration-Gestiondescontenuslégaux)
    * [Inclusion de contenu dans les e-mails](modules-administration.md#ModulesAdministration-Inclusiondecontenudanslese-mails)
  * [Affichage HTML simple](modules-administration.md#ModulesAdministration-AffichageHTMLsimple)
  * [Alertes e-mail](modules-administration.md#ModulesAdministration-Alertese-mail)
  * [CloudCache CDN](modules-administration.md#ModulesAdministration-CloudCacheCDN)
  * [Expertise PrestaShop](modules-administration.md#ModulesAdministration-ExpertisePrestaShop)
  * [Filigrane](modules-administration.md#ModulesAdministration-Filigrane)
  * [Lettre d'informations](modules-administration.md#ModulesAdministration-Lettred%27informations)
  * [Nettoyage de la base de données](modules-administration.md#ModulesAdministration-Nettoyagedelabasededonnées)
  * [XML/SWF Charts](modules-administration.md#ModulesAdministration-XML/SWFCharts)

## 1-Click Upgrade - AutoUpgrade <a href="#modulesadministration-1-clickupgrade-autoupgrade" id="modulesadministration-1-clickupgrade-autoupgrade"></a>

Ce module facilite grandement la mise à jour de PrestaShop vers sa dernière version.

Lisez le chapitre "Mise à jour automatique" du guide de mise à jour de PrestaShop pour en apprendre plus sur ce module : [http://doc.prestashop.com/pages/viewpage.action?pageId=11272345](http://doc.prestashop.com/pages/viewpage.action?pageId=11272345).

## Conformité européenne améliorée <a href="#modulesadministration-conformiteeuropeenneamelioree" id="modulesadministration-conformiteeuropeenneamelioree"></a>

_Nouveauté PrestaShop 1.6.1.0._

Le module "Conformité européenne améliorée" aide les marchands Européens à répondre aux dernières exigences légales en e-commerce.

Ce module est essentiel pour les boutiques européennes.

La plupart de ses options offrent plus de transparence aux clients, avec par exemple :

* Des étiquettes/libellés de prix plus détaillées (prix "À partir de", frais de port et délais, poids du produit, etc.) ;
* Une page de commande avancée ;
* Le contenu légal peut être attaché aux e-mails.

Toutes ses options ne sont pas forcément utiles pour tous les pays, mais elles aident toutes à rendre votre boutique plus conforme face aux lois de l'Europe en termes d'e-commerce.\
Les réglages par défaut sont les réglages recommandés ; vous êtes libre d'activer ou désactiver les options comme bon vous semble.

### Libellés <a href="#modulesadministration-libelles" id="modulesadministration-libelles"></a>

* **Délai de livraison estimé (produits en stock)**. Indique le délai de livraison estimé pour vos produits disponibles. Laissez le champ vide pour le désactiver.
* **Délai de livraison estimé (produits en rupture de stock)**. Indique le délai de livraison estimé pour vos produits en rupture de stock. Laissez le champ vide pour le désactiver.
* **Prix "Au lieu de"**. Quand un produit est en promotion, affiche "Au lieu de" avant le prix de base.
* **Taxes incluses / exclues**. Affiche si les taxes sont incluses ou non, à côté du prix du produit ("HT/TTC").
* **Frais de port inclus / exclus**. Précise si les frais de livraisons sont inclus ou pas, à côté du prix du produit ("Frais de port inclus / Hors frais de port").\
  Si cette option est activée, assurez-vous que les conditions de livraison sont associées à une page CMS ci-dessous ("Gestion des contenus légaux"). Le libellé ajoutera un lien vers cette page.
* **Poids du produit**. Affiche le poids du produit (quand l'information est disponible et que le produit pèse plus de 1 kg).
* **Nombre de décimales du poids**. Choisissez le nombre de décimales à afficher pour le poids du produit (par exemple 1 kg avec 0 décimale ou 1,01 kg avec 2 décimales). Cette valeur doit être positive.
* **Conditions d'annulation dans les CGV**. Ajoute le contenu de la page CMS des conditions d'annulation dans les conditions générales de vente (CGV).\
  Si activé, assurez-vous que les conditions d'annulation sont associées à une page CMS ci-dessous (Gestion des contenu légaux).
* **Conditions d'annulation des produits dématérialisés**. Ajoute une case à cocher obligatoire quand le panier contient un produit dématérialisé. Utilisez cette option pour que vos clients aient conscience qu'il n'est pas possible de retourner un produit dématérialisé.
* **Prix "À partir de" (quand déclinaisons)**. Affiche "à partir de" avant le prix des produits avec déclinaisons.\
  Les prix pouvant varier d'une déclinaison à l'autre, ce libellé indique que le prix final peut être plus élevé.
* **Texte au-dessus du panier**. Permet d'ajouter un texte personnalisé au-dessus du récapitulatif de panier.
* **Texte en bas de panier**. Permet d'ajouter un texte personnalisé en bas du récapitulatif de panier.

### Fonctionnalités <a href="#modulesadministration-fonctionnalites" id="modulesadministration-fonctionnalites"></a>

* **Activer l'option "Envoyer à un ami"**. Assurez-vous d'être en règle avec la législation de votre pays avant de l'activer : les e-mails envoyés par cette option peuvent être considérés comme des e-mails commerciaux non désirés (spam).\
  Quand activé, le module "Envoyer à un ami" permet à vos clients d'envoyer à leurs amis un e-mail avec un lien vers une page produit.
* **Activer l'option "Re-commander"**. Assurez-vous d'être en règle avec la législation de votre pays avant de l'activer : cette option peut être considérée comme de la vente forcée.\
  Quand activée, l'option "e-commander"; permet aux clients de repasser commande en un clic depuis leur historique de commandes.
* **Activer la "Page de commande avancée"**. Pour répondre aux exigences légales européennes les plus récentes, la page de commande avancée affiche des informations supplémentaires (CGV, modes de paiement, etc.), sur une seule et même page.\
  La page de commande avancée affiche les sections suivantes : modes de paiement, récapitulatif d’adresses, acceptation des CGV, récapitulatif du panier, et bouton "Commande avec obligation de paiement".
* **Taxe moyenne pour livraison et emballage**. Quand activé, la taxe pour la livraison et l'emballage sera la moyenne de toutes les taxes qui s'appliquent aux produits du panier.

### Gestion des contenus légaux <a href="#modulesadministration-gestiondescontenuslegaux" id="modulesadministration-gestiondescontenuslegaux"></a>

Plusieurs options de ce module requièrent que le système "sache" ce à quoi servent certaines de vos pages CMS. S'il n'y a pas de page correspondant à une association, vous devez les créer.

### Inclusion de contenu dans les e-mails <a href="#modulesadministration-inclusiondecontenudanslese-mails" id="modulesadministration-inclusiondecontenudanslese-mails"></a>

Avec cette interface, vous pouvez choisir quels documents inclure en bas de n'importe quel e-mail standard envoyé par la boutique – par exemple, le contenu textuel de votre page de CGV peut être inclus avec chaque facture envoyée.

Le contenu est choisi à parti des options dans la section "Gestion des contenus légaux" de ce module. Si aucune option n'est configurée, vous ne pourrez pas choisir le contenu à envoyer avec un e-mail.

## Affichage HTML simple <a href="#modulesadministration-affichagehtmlsimple" id="modulesadministration-affichagehtmlsimple"></a>

Utilisé par le système de statistique de PrestaShop pour afficher les données dans une grille.

## Alertes e-mail <a href="#modulesadministration-alertese-mail" id="modulesadministration-alertese-mail"></a>

PrestaShop vous permet d'informer vos clients par e-mail dans certaines situations, par exemple lorsqu'une nouvelle commande est faite dans votre boutique, ou si un produit est presque en rupture de stock. Les clients peuvent saisir une adresse e-mail à laquelle ils seront contactés lorsque le produit est à nouveau disponible. Cliquez sur "Installer" puis "Configurer" pour configurer le module.

Lorsque vous cochez la case "Disponibilité du produit", un champ apparaît dans la page produit sur votre boutique lorsque le produit est en rupture de stock. Il propose à vos clients de laisser leurs coordonnées afin qu'ils puissent être contactés lorsque vous aurez à nouveau ce produit en stock.

Dans la section "Notifications pour le marchand", vous pouvez spécifier si vous souhaitez être alerté de chaque nouvelle commande. Pour ce faire, cochez la case "Nouvelle commande".\
&#x20;Si vous voulez être alerté lorsqu'un produit atteint un niveau de stock que vous avez défini, sélectionnez "Hors stock" et régler la valeur à laquelle vous souhaitez être alerté.

Les alertes par e-mail peuvent être envoyées à plusieurs destinataires à la fois. Pour ce faire, indiquez chaque adresse e-mail qui recevra la notification (une adresse e-mail par ligne. Pour aller à la ligne, appuyez sur la touche Entrée de votre clavier).

## CloudCache CDN <a href="#modulesadministration-cloudcachecdn" id="modulesadministration-cloudcachecdn"></a>

Accélérez votre boutique avec le Content Delivery Network (CDN) de CloudCache.com

\
Voici les avantages d'avoir un site qui charge plus rapidement :\


* **Meilleur référencement.** Google utilise la vitesse d'affichage de la page comme facteur clé de leur algorithme de tri. Les pages qui se chargent plus rapidement ont une meilleure place dans les moteurs de recherche, ce qui signifie plus de trafic sur votre site et donc plus d'argent pour vous.
* **Augmente votre taux de conversion.** Amazon a découvert qu'un site qui met 100 millisecondes de plus à se charger perd 1% de son revenu. Cette raison seule vous oblige à vous soucier du temps de chargement de votre site.\

* **Traverser les tempêtes de trafic**. Dans le cas où votre site devient célèbre du jour au lendemain (ex. : si votre site est cité à la télévision), vos ventes s'envoleront mais votre serveur peut planter à cause de la charge. Ce module vous aide à balancer la charge de votre site face à un fort trafic.
* **La simplicité des SSL personnalisés**. L'accélération SSL décharge jusqu'à 70% de la puissance de votre serveur.

## Expertise PrestaShop <a href="#modulesadministration-expertiseprestashop" id="modulesadministration-expertiseprestashop"></a>

&#x20;Ce module permet de suivre votre progression dans la configuration de votre boutique et dans la réussite de votre activité, et voir à quel point vous avez grandi et évolué en cours des jours, mois et années. Il est installé par défaut.

Ce module ajoute un système de badges et de points, divisés en trois niveaux, tous faisant partie intégrante du succès d'un site e-commerce :

* **Fonctionnalités**. Votre utilisation de certaines fonctionnalités clé de l'e-commerce, telles que la performance du site, la taille du catalogue, le nombre d'employés ou le SEO.
* **Succès**. Votre complétion de buts précis de l'e-commerce, tels que le nombre de clients, de commandes, ou votre revenu global.
* **International**. Traque votre placement sur les marchés internationaux comme les Amériques, l'Océanie, l'Asie, l'Europe, l'Afrique ou le Maghreb.

&#x20;Plus votre boutique progresse, plus vous gagnez de badges et de points. Il n'y a pas besoin d'envoyer des informations ou de remplir de formulaire. Nous vous savons suffisamment préoccupé par votre boutique, donc tout est fait automatiquement. Utilisez cet outil pour mieux apprécier votre évolution et vous fixer de nouveaux objectifs.

## Filigrane <a href="#modulesadministration-filigrane" id="modulesadministration-filigrane"></a>

Ce module vous permet d'ajouter un filigrane aux images de votre boutique. Cela permet de limiter leur diffusion sur Internet.

Si vous avez l'intention d'exporter vos produits vers Google Shopping, sachez que sur ce service, l'utilisation de texte promotionnel / logos et filigranes sur les images n'est pas autorisée. Vous pouvez seulement y utiliser des images qui n'ont aucun filigrane / logo ajouté.

Vous pouvez en apprendre plus en lisant la documentation de Google Shopping sur le sujet : [https://support.google.com/merchants/answer/2700371?hl=fr](https://support.google.com/merchants/answer/2700371?hl=fr).

La page de configuration vous signale tout de suite quels paramètres sont actuellement manquants.

* **Fichier du filigrane**. L'image choisie doit être au format GIF.
* **Transparence du filigrane (0-100)**. 100 Montant pour une image non transparente, ce qui signifie que votre logo sera très visible, mais il cachera également une partie de l'image entière. Le réglage par défaut, 60, est en général un bon compromis.
* **Alignement horizontal**. Sélectionnez où votre filigrane doit apparaître sur chacune de vos images, ici sur l'axe horizontal.
* **Alignement vertical**. Sélectionnez où votre filigrane doit apparaître sur chacune de vos images, ici sur l'axe vertical.
* **Choisissez les types d'image pour lesquels le filigrane doit s'appliquer.**. Les types d'image auxquels le filigrane doit être appliqué. Vous n'avez vraiment besoin que de choisir les plus grandes tailles, car celles-ci sont les plus susceptibles d'être volées.

Une fois que vous avez enregistré vos paramètres, la configuration est terminée, mais les filigranes ne sont pas encore ajoutés sur les photos de votre boutique. Allez dans le menu "Préférences", puis ouvrez la page "Images". De là, cliquez sur le bouton "Régénérer les miniatures" en bas de la page. PrestaShop traitera toutes vos photos (telles que sélectionnées dans la configuration), et votre image apparaîtra en filigrane sur les photos que vous avez sélectionnées.

## Lettre d'informations <a href="#modulesadministration-lettredinformations" id="modulesadministration-lettredinformations"></a>

Vos clients peuvent vous donner leur adresse e-mail, soit en la saisissant dans le bloc Newsletter situé sur la page d'accueil, soit en cochant la case "Oui" pour s'abonner à la lettre d'information lors de leur inscription. Vous avez besoin de ces adresses e-mail afin de faire du marketing. Cliquez sur "Configurer" pour afficher la page nécessaire.

Lors de leur inscription, vos clients ont deux options liées à la newsletter : la première leur propose de s'abonner à la newsletter, la seconde de recevoir des offres de vos partenaires (opt-in).

La première section vous permet de collecter toutes les adresses e-mail enregistrées par le bloc newsletter sur votre page d'accueil, en cliquant sur le bouton "Exporter fichier .CSV". Une notification apparaîtra, vous demandant de cliquer sur un lien pour télécharger le fichier contenant les adresses.

Quatre éléments d'information seront présents dans ce fichier. L'id du client, son adresse e-mail, le jour de son inscription, et son adresse IP. Si vous chargez ces données avec des logiciels tels que Microsoft Excel, vous pourrez trier les informations comme vous le souhaitez.

La section suivante, appelée "Export des clients", vous permet de filtrer les adresses e-mail de vos clients. Vous pouvez ensuite filtrer les clients par pays d'origine en utilisant la liste déroulante "Pays du client", puis en sélectionnant le pays de votre choix. Le filtrage par pays est particulièrement utile pour l'envoi de newsletters dans la bonne langue et pour adapter vos offres.

Vous pouvez alors prendre en compte plus d'informations lors de l'exportation des adresses e-mail. Utilisez le champ "Inscrits lettre d'info." pour sélectionner l'un des trois éléments suivants:

* Le premier, "Tous les clients", vous permet de sélectionner toutes les adresses e-mail de vos clients qui ouvrent un compte sur votre boutique. C'est-à-dire à la fois ceux qui souhaitent recevoir des informations de votre part, et ceux qui ne le souhaitent pas.
* La seconde, "Inscrits", vous permet de sélectionner uniquement les clients qui veulent recevoir une lettre d'information de votre part.
* Le troisième, "Non-inscrits", vous permet de sélectionner uniquement les clients qui ne veulent pas recevoir une lettre d'information de votre part.

Arrivent ensuite le champ "Inscrits pub", où vous pouvez filtrer les contacts en fonction de leur volonté de recevoir des messages en provenance de vos partenaires publicitaires. Ici également, trois choix sont possibles:

* Le premier, "Tous les clients", vous permet de sélectionner toutes les adresses e-mail de vos clients qui ouvrent un compte sur votre boutique. C'est-à-dire à la fois ceux qui souhaitent recevoir des informations de vos partenaires, et ceux qui ne le souhaitent pas.
* La seconde, "Inscrits", vous permet de sélectionner uniquement les clients qui veulent recevoir une lettre d'information de vos partenaires.
* Le troisième, "Non-inscrits", vous permet de sélectionner uniquement les clients qui ne veulent pas recevoir une lettre d'information de vos partenaires.

Une fois que vous avez filtré les adresses e-mail à exporter, cliquez sur "Exporter un fichier .CSV" pour récupérer toutes les adresses. Comme précédemment, une notification sur un fond vert apparaît, vous demandant de cliquer et télécharger le fichier. Ce fichier contient six types d'informations : l'ID du client, son nom, son prénom, son adresse e-mail, son adresse IP, et la date de l'enregistrement. Vous pouvez ensuite utiliser ces informations pour envoyer vos campagnes de marketing.

## Nettoyage de la base de données <a href="#modulesadministration-nettoyagedelabasededonnees" id="modulesadministration-nettoyagedelabasededonnees"></a>

Ce module est très utile lorsque avez terminé d'explorer PrestaShop pour la première fois, et que vous êtes prêt à mettre en place votre propre contenu.

Vous devez avant cela enlever les données de démonstration qui ont été installées en même temps que PrestaShop : produits, catégories, clients, commandes, etc.

La page de configuration a trois sections :

* **Catalogue.** Cette option supprimera toutes les données de votre catalogue actuel, même les éléments que vous avez ajouté vous-mêmes. Cochez la case et cliquez sur le bouton "Supprimer le catalogue" pour lancer le processus.
* **Commandes et clients**. Cette options supprimera toutes les commandes et les clients, même ceux que vous avez créé vous-même. Cochez la case et cliquez sur le bouton "Supprimer les commandes et clients" pour lancer le processus.
* **Contraintes d'intégrité fonctionnelle**. Un clic sur le bouton "Vérifier et réparer" corrigera votre base de données et s'assurera que tout est bien en place, et tentera de corriger ce qui ne l'est pas.

## XML/SWF Charts <a href="#modulesadministration-xml-swfcharts" id="modulesadministration-xml-swfcharts"></a>

Ce module apporte une bibliothèque graphique qui peut être utilisée pour créer des graphiques de statistiques.
