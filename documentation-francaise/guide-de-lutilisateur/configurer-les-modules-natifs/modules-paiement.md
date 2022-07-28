# Modules Paiement

Avec PrestaShop, vous pouvez accepter les transactions de vos clients à l'aide de plusieurs modes de paiement, tels que les chèques, virement bancaire, les espèces à la livraison, et certains modules partenaires tels que HiPay, Moneybookers, PayPal et autres. Ils sont déjà inclus dans votre boutique et sont prêts à l'usage. Cependant, il est nécessaire de les configurer.

PrestaShop dispose de trois modules de paiement de base, que vous pouvez utiliser directement, sans devoir vous enregistrer auprès du service tiers :

* Virement bancaire
* Règlement à la livraison
* Chèque

En outre, plusieurs modules pour les services tiers de paiement sont disponibles par défaut dans votre installation de PrestaShop. Ces ont été mis au point par des partenaires de PrestaShop, en étroite collaboration avec les développeurs de PrestaShop. Tous peuvent être utilisés en toute confiance.Tous peuvent être utilisés en toute sécurité, et vous trouverez une documentation qui leur est propre dans la page de configuration de chaque module.

Notez que vous pouvez trouver de nombreux autres modules de paiement sur Addons : [http://addons.prestashop.com/fr/4-modules-paiement-prestashop](http://addons.prestashop.com/fr/4-modules-paiement-prestashop).

## Authorize.net AIM <a href="#modulespaiement-authorize.netaim" id="modulespaiement-authorize.netaim"></a>

Le module AIM Authorize.net permet à votre boutique d'accepter les paiements par carte de crédit.

Vous devez avoir un compte Authorize.net pour utiliser ce module. Vous pouvez accéder au site en cliquant sur le logo Authorize.net dans la page de configuration du module (à droite de la page).\
&#x20;Ensuite, configurez le module avec votre identifiant et votre clé. Indiquez si vous êtes en mode test ou en mode de production, sélectionnez les types de cartes que vous voulez que votre boutique accepte, et enfin, indiquez quelle devrait être l'état de commande PrestaShop correspondant à l'état "En attente de vérification" d'Authorize (par défaut : "Erreur de paiement").

Une fois que les paramètres sont en place, vos clients verront l'option "Authorize.net AIM" apparaître sur le front-office de la boutique, dans le bloc des méthodes de paiement disponibles.

## Chèque <a href="#modulespaiement-cheque" id="modulespaiement-cheque"></a>

Ce module permet à vos clients de payer en vous envoyant un chèque.

Pour configurer le paiement par chèque, ouvrez la page de configuration du module et indiquez l'ordre auquel votre client doit faire le chèque - la plupart du temps, votre nom ou celui de votre société, et votre adresse.\
&#x20;Cette information apparaîtra alors à l'utilisateur à la fin du processus de commande, après avoir cliqué sur l'option "Paiement par chèque", et avoir validé par un clic sur le "Je confirme ma commande".

Notez que lors de la réception du paiement par chèque, vous **devez** changer manuellement l'état de paiement de la commande pour le passer à "Paiement accepté" dans votre back-office. C'est bien différent des commandes par carte de crédit, pour lesquelles le paiement est validé automatiquement. Vous pouvez trouver la commande et changer son statut dans la page "Commandes" du menu "Commandes".

## Comptant à la livraison <a href="#modulespaiement-comptantalalivraison" id="modulespaiement-comptantalalivraison"></a>

Ce module permet à vos clients de vous dire qu'ils souhaitent payer le produit directement à celui qui le livrera chez eux. La transaction pourrait se faire en magasin, ou vous pourriez avoir vos propres employés qui livrent le produit à vos clients. C'est surtout utile pour les livraisons locales.

## Hipay <a href="#modulespaiement-hipay" id="modulespaiement-hipay"></a>

Le module Hipay permet à votre boutique d'accepter les paiements par carte de crédit.

Vous devez avoir un compte Hipay pour utiliser ce module.\
&#x20;Ensuite, configurez le module avec votre numéro de compte, votre mot de passe marchand, et votre ID de site.\
&#x20;Enfin, vous pouvez choisir l'âge minimum autorisé, et restreindre le module à certaines zones géographique.

Une fois que les paramètres sont en place, vos clients verront l'option "Hipay" apparaître sur le front-office de la boutique, dans le bloc des méthodes de paiement disponibles.

## Kwixo <a href="#modulespaiement-kwixo" id="modulespaiement-kwixo"></a>

Le module Kwixo permet à votre boutique d'accepter les paiements grâce au service de paiement Kwixo. Kwixo fait partie de FIA-Net, le tiers de confiance de l'e-commerce français, et de deux grandes banques françaises, le Crédit Agricole et LCL. Les clients ont besoin d'avoir un compte Kwixo, et d'avoir enregistré une carte de crédit sur leur service.

Vous devez avoir un compte Kwixo pour utiliser ce module. Vous pouvez accéder au formulaire d'inscription en cliquant sur le lien dans la page de configuration.\
&#x20;Ensuite, configurez le module avec votre ID marchand, votre clé de cryptage, et indiquez si vous souhaitez travailler en mode Test pour l'instant, le type de paiement que vous souhaitez accepter, et votre délai de livraison.\
&#x20;À partir de là, compléter les informations de configuration en indiquant vos principaux types de produits dans la section "Informations sur les produits vendus sur votre boutique" , et vos types de support dans la section "Configuration du transporteur".

Une fois que les paramètres sont en place, vos clients verront l'option "Kwixo" apparaitre sur le front-office de votre boutique, dans la section des méthodes de paiement disponibles.

En tant que commerçant, vous avez accès à un back-office Kwixo spécifique à l'adresse située dans la section "Gérez vos paiements dans votre interface d'administration Kwixo".

## Ogone <a href="#modulespaiement-ogone" id="modulespaiement-ogone"></a>

Le module Ogone permet à votre boutique d'accepter les paiements par carte de crédit.

Vous devez avoir un compte Ogone pour utiliser ce module. Vous pouvez accéder au formulaire d'inscription en cliquant sur le bouton "Créer votre compte d'essai gratuit!" dans la page de configuration.\
&#x20;Ensuite, configurer le module avec votre PSPID, votre signature SHA-in, votre signature SHA-out, et enfin choisissez si vous voulez utiliser le module en mode test ou en mode production.

Une fois que les paramètres sont en place, vos clients verront l'option "Ogone" apparaître sur le front-office de la boutique, dans le bloc des méthodes de paiement disponibles.

## PayPal <a href="#modulespaiement-paypal" id="modulespaiement-paypal"></a>

Le module PayPal permet à votre boutique d'accepter les paiements par carte de crédit ou via le service de paiement PayPal.

Vous devez avoir un compte PayPal pour utiliser ce module. Vous pouvez accéder au formulaire d'inscription en cliquant sur le bouton "Ouvrez un compte PayPal" dans la page de configuration.\
&#x20;Ensuite, configurez le module puis entrez votre nom d'utilisateur de l'API, votre mot de passe API et votre signature API. Vous devez également vous assurer que les autres paramètres correspondent à vos besoins.

Une fois que les paramètres sont en place, vos clients verront l'option "PayPal" apparaître sur le front-office de la boutique, dans le bloc des méthodes de paiement disponibles.

## Skrill <a href="#modulespaiement-skrill" id="modulespaiement-skrill"></a>

Le module Skrill Moneybookers permet à votre boutique d'accepter les paiements par carte de crédit.

Vous devez disposer d'un compte Moneybookers pour utiliser ce module. Vous pouvez accéder au formulaire d'inscription en cliquant sur l'image dans la section "Ouverture de compte".\
Ensuite, cliquez sur "J'ai déjà un compte Moneybookers" pour continuer la configuration du module.

Une fois que les paramètres sont en place, vos clients verront l'option "Skrill Moneybookers" apparaître sur le front-office de la boutique, dans le bloc des méthodes de paiement disponibles.

## Syspay <a href="#modulespaiement-syspay" id="modulespaiement-syspay"></a>

Syspay révolutionne le paiement dans le monde de l’e-commerce et propose à ses clients une Plate-forme d’encaissement omni-channel. Sur le web, en magasin, en relais-colis, à domicile ou sur la route, quelle que soit votre activité, le paiement est possible et est considéré comme « on-line », il bénéficie ainsi de tous les avantages de la plateforme Syspay !

## Virement bancaire <a href="#modulespaiement-virementbancaire" id="modulespaiement-virementbancaire"></a>

Ce module permet à vos clients de payer en utilisant un virement bancaire.

Pour que le module accepte les virements bancaires, vous devez remplir l'adresse de la banque utilisée par votre boutique. Pour cela, allez dans la page de configuration du module.

Une fois que les paramètres sont en place, vos clients verront l'option "Payer par virement bancaire" apparaître sur le front-office de la boutique, dans le bloc des méthodes de paiement disponibles. Après que le client l'ait choisi et ait indiqué son choix de monnaie, vos coordonnées bancaires apparaissent.\
&#x20;Notez que lors de la réception par virement bancaire du client, vous **devez** changer manuellement l'état de paiement de la commande pour le passer à "Paiement accepté" dans votre back-office. C'est bien différent des commandes par carte de crédit, pour lesquelles le paiement est validé automatiquement. Vous pouvez trouver la commande et changer son statut dans la page "Commandes" du menu "Commandes".
