# En cas de problème

* [En cas de problème](en-cas-de-probleme.md#Encasdeproblème-Encasdeproblème)
  * [Les pages d'administration s'affiche bizarrement](en-cas-de-probleme.md#Encasdeproblème-Lespagesd%27administrations%27affichebizarrement)
  * [La pages des module n'est pas mise à jour](en-cas-de-probleme.md#Encasdeproblème-Lapagesdesmodulen%27estpasmiseàjour)
  * [Le thème par défaut ne fonctionne plus](en-cas-de-probleme.md#Encasdeproblème-Lethèmepardéfautnefonctionneplus)
  * [Certains modules ne fonctionnent pas](en-cas-de-probleme.md#Encasdeproblème-Certainsmodulesnefonctionnentpas)
  * [Incompatible module](en-cas-de-probleme.md#Encasdeproblème-Incompatiblemodule)
  * [La mise en page des produits phares est mauvaise](en-cas-de-probleme.md#Encasdeproblème-Lamiseenpagedesproduitspharesestmauvaise)
  * [Remettre votre ancienne base de données](en-cas-de-probleme.md#Encasdeproblème-Remettrevotreanciennebasededonnées)
  * [Support PrestaShop](en-cas-de-probleme.md#Encasdeproblème-SupportPrestaShop)

## Les pages d'administration s'affiche bizarrement <a href="#encasdeprobleme-lespagesdadministrationsaffichebizarrement" id="encasdeprobleme-lespagesdadministrationsaffichebizarrement"></a>

Lors du premier chargement après la mise à jour, les pages d'administration peuvent sembler complètement cassées : parce que votre navigateur conserve en mémoire cache certaines fichiers, il est probable qu'il utilise encore les anciens fichiers CSS et JavaScript au lieu des nouveaux.

Vous devez recharger les pages plusieurs fois, ou même vider le cache de votre navigateur, afin d'obtenir l'interface correcte. Lisez comment vider votre cache ici : [http://support.google.com/accounts/bin/answer.py?hl=fr\&hlrm=en\&answer=32050](http://support.google.com/accounts/bin/answer.py?hl=fr\&hlrm=en\&answer=32050).

## La pages des module n'est pas mise à jour <a href="#encasdeprobleme-lapagesdesmodulenestpasmiseajour" id="encasdeprobleme-lapagesdesmodulenestpasmiseajour"></a>

Pour régler le problème, rechargez la page plusieurs fois, à l'aide de la touche F5.

## Le thème par défaut ne fonctionne plus <a href="#encasdeprobleme-lethemepardefautnefonctionneplus" id="encasdeprobleme-lethemepardefautnefonctionneplus"></a>

Le nom du thème par défaut a été changé de "prestashop" en "default". Si vous utilisez le thème par défaut, renommez le dossier du thème de "prestashop" à "default", et tout devrait remarcher.

## Certains modules ne fonctionnent pas <a href="#encasdeprobleme-certainsmodulesnefonctionnentpas" id="encasdeprobleme-certainsmodulesnefonctionnentpas"></a>

Si un module installé ne donne pas les résultats attendus, essayez de les désinstaller, puis de le réinstaller.

## Incompatible module <a href="#encasdeprobleme-incompatiblemodule" id="encasdeprobleme-incompatiblemodule"></a>

Dans certaines cas, un module peut ne pas être compatibles avec la dernière version de PrestaShop. Vous devriez alors contacter le développeur ou sa société, afin de lui demander comment corriger le problème.

## La mise en page des produits phares est mauvaise <a href="#encasdeprobleme-lamiseenpagedesproduitspharesestmauvaise" id="encasdeprobleme-lamiseenpagedesproduitspharesestmauvaise"></a>

Si votre page d'accueil est cassé du fait du block Produits Phares, qui place ses éléments sur une seule colonne, alors il vous faut réinstaller le module "Produits phares sur la page d'accueil" (de la catégorie "Fonctionnalités Front-office").

## Remettre votre ancienne base de données <a href="#encasdeprobleme-remettrevotreanciennebasededonnees" id="encasdeprobleme-remettrevotreanciennebasededonnees"></a>

La remise en place de l'ancienne base de données n'est à faire qu'en dernier recours.

Si votre mise à jour s'est mal déroulée et que vous n'avez pas d'autre solution que de revenir à la version précédente de votre base de données, il a deux manières d'y parvenir :

* Demandez à votre hébergeur de le faire pour vous.\
  &#x20;N'oubliez pas de leur fournir la sauvegarde de base de données que vous avez à la première étape du processus de mise à jour !

...ou...

* Importez vos données sauvegardées en passant par phpMyAdmin\
  &#x20;Votre hébergeur vous propose certainement un outil de gestion de base de données, comme phpMyAdmin, qui dispose de fonction d'export et d'import.\
  &#x20;Si votre base de données est trop volumineuse, il se peut que vous receviez un message d'erreur. Il se peut dans ce cas que vous ayez à demander de l'aide à votre hébergeur, par exemple pour changer la taille maximale d'envoi.

Les fichiers SQL que vous avez sauvegardés avec l'outil interne de PrestaShop sont accessibles dans le dossier `/admin/backups`.\
&#x20;Vous pouvez également télécharger les fichiers SQL de vos données depuis votre back-office. Dans la page "Sauvegarde BDD" du menu "Paramètres avancés", sélectionnez votre dernière sauvegarde et téléchargez-la en cliquant sur son lien. Cela devrait prendre entre 1 à 20 minutes à télécharger.

## Support PrestaShop <a href="#encasdeprobleme-supportprestashop" id="encasdeprobleme-supportprestashop"></a>

Pour toute **demande de support** ou **d'aide à la mise en place de votre site**, contactez-nous et découvrez nos offres.

Notre équipe de support se met à votre disposition pour tous les problèmes techniques liés à la mise à jour de votre boutique PrestaShop :

* Par e-mail : [support@prestashop.com](mailto:support@prestashop.com)
* Par téléphone : +33.1 40 18 30 04 (9h00 à 18h00, heure de Paris)
* [http://support.prestashop.com](http://support.prestashop.com)
* Et bien entendu, le formidable forum communautaire : [http://www.prestashop.com/forums/](http://www.prestashop.com/forums/)
