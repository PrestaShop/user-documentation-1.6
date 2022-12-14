# Commandes

La page "Commandes" vous permet d'accéder à toutes les informations relatives aux achats sur votre boutique. Toutes les transactions sont disponibles ici, rangées par date (par défaut, de la plus récente à la plus ancienne).

Vous pouvez filtrer les résultats et facilement trouver les commandes que vous recherchez en utilisant les champs ci-dessus. Par exemple, pour identifier les commandes de M. Durand, tapez "Durand" dans le champ "Client" puis cliquez sur "Filtrer".

VOUS NE POUVEZ PAS SUPPRIMER UNE COMMANDE. En Europe, il est interdit de permettre la suppression d'informations de paiement, de facturation ou de commande. C'est pourquoi l'implémentation d'un bouton "Supprimer" pour les commandes rendrait PrestaShop illégal en Europe.

Pour supprimer correctement la commande par défaut, installez le module "Nettoyage de la base de données" (qui est disponible dans l'installation par défaut depuis la version 1.5.4), ouvrez son écran de configuration et cochez la case "Commandes et clients" avec de cliquer sur le bouton "Supprimer les commandes et clients".

Vous pouvez exporter une liste de vos commandes en cliquant sur le bouton "Export" situé en haut.\
Vous ne pouvez pas importer de commandes.

## Créer une commande <a href="#commandes-creerunecommande" id="commandes-creerunecommande"></a>

L'une des grandes fonctionnalités de PrestaShop est la possibilité de créer une commande directement depuis le back-office. Cela peut par exemple se révéler extrêmement utile quand un client veut acheter un produit mais n'y parvient pas, et il vous faut prendre la main et faire la commande tandis que vous êtes en contact avec le client, par téléphone ou par e-mail.

En cliquant sur le bouton "Ajouter", une page s'ouvre, avec un seul champ textuel, nommé "Rechercher un client". Lorsque vous créez une nouvelle commande via le back-office, votre première tâche consiste à associer cette commande à un client. Saisissez les premières lettres de son nom, prénom ou adresse e-mail, et PrestaShop vous affichera les comptes correspondants.

Si le client pour lequel vous créez la commande n'a même pas encore de compte sur votre boutique, vous pouvez en créer un à la volée : cliquez sur le bouton "Ajouter un nouveau client" pour ouvrir une fenêtre avec les principaux détails à remplir. Une fois le compte enregistré, il devient aussitôt le compte associé à la commande.

Notez bien que vous devrez également enregistrer les adresses du client – un bouton "Ajouter une nouvelle adresse" est disponible en bas de la page, dans la section "Adresses".

Cliquez sur le bouton "Choisir" du bon client, et l'intégralité du formulaire de commande apparaît. Tous les ajouts de produits se feront dans sa section principale, "Panier". Vous pouvez également choisir d'utiliser l'une des précédentes commandes du client, ou l'un de ses paniers abandonnés.

Le champ "Rechercher un produit" vous permet de faire une recherche dynamique sur les produits à ajouter : saisissez les premières lettres du nom du produit, et PrestaShop affichera une liste déroulante avec les produits correspondants. Choisissez le produit, sélectionnez la quantité, et cliquez sur le bouton "Ajouter au panier". Si le produit est disponible en plusieurs déclinaisons, vous pouvez bien sûr choisir celle désirée grâce à la liste déroulante qui apparaît dans ce cas.\
&#x20;Notez que PrestaShop vous indique le stock restant pour un produit donné, ce qui vous permet de faire savoir au client que vous êtes en rupture de stock pour ce produit dès le formulaire de commande.

Cette page vous permet de voir les paniers et commandes précédent(e)s de ce client, s'il y en a. S'il se trouve que vous deviez gérer un panier que le client n'arrive pas à valider, vous pouvez utiliser ce panier pour cette commande en cliquant sur l'action "Utiliser".

Si besoin est, vous pouvez également octroyer un bon d'achat ou une règle de panier pour cette commande, et même en créer une à la volée en cliquant sur le bouton "Ajouter un bon d'achat".

Enfin, vous devez préciser à quelle adresse la commande doit être envoyée (et possiblement facturée). Ici encore, vous pouvez créer de nouvelles adresses à la volée à l'aide du bouton "Ajouter une nouvelle adresse".

## Voir le détail des commandes <a href="#commandes-voirledetaildescommandes" id="commandes-voirledetaildescommandes"></a>

Afin de traiter les commandes que vous recevez, vous devez avoir accès aux informations qu'elles contiennent.\
&#x20;Cliquez sur la ligne contenant la commande, ou cliquez sur le bouton à la droite de la commande.

La fiche détaillant la commande occupe une pleine page.

En haut de la page se trouve un rapide résumé de la commande : date de validation, nombre de discussion avec le service client à propos de cette commande, nombre de produits dans la commande, et montant total.

Les détails de la commande vous donnent accès à de nombreuses informations :

* À gauche, les informations de commande :\

  * L'état et à l'historique de la commande
  * Aux informations relatives au transport : poids total de la commande, transporteur choisi par le client.
* À droite, les informations sur le client :
  * Historique d'achats
  * Adresses de livraison et de facturation (avec une carte)
* La méthode de paiement utilisée, le coût des produits, le coût du transport.
* Divers détails sur les produits commandés.

Dans la section "Adresse de livraison" de la page, vous pouvez voir une icône "G" : elle vous permet de localiser l'adresse sur Google Maps.

## Modifier la commande <a href="#commandes-modifierlacommande" id="commandes-modifierlacommande"></a>

Les commandes ne sont pas gravées dans le marbre. Il existe de nombreuses raisons pour lesquelles vous pourriez vouloir modifier une commande avant de lancer la récupération des produits, leur emballage et leur envoi à leur nouveau propriétaire : l'un des produits est en fait déstocké, le client a changé d'avis, etc.

### Ajouter un produit <a href="#commandes-ajouterunproduit" id="commandes-ajouterunproduit"></a>

En bas de liste des produits, vous pouvez trouver un bouton "Ajouter un produit", qui ajoute un champ à la commande

En ajoutant un produit, la liste des produits se voit ajouter une ligne avec une poignée de champs. Le premier champ est en fait un moteur de recherche : saisissez les premières lettres d'un produit pour voir apparaître les produits correspondants. Sélectionnez celui que vous souhaitez ajouter, et les champs grisés deviennent disponibles.\
&#x20;Si le produit dispose de déclinaisons, vous pouvez sélectionner la vôtre dans la liste déroulante qui apparaît sous le nom : le prix par unité changera en conséquence.\
&#x20;Réglez la quantité du produit, puis cliquez sur le bouton "Ajouter le produit" : c'est fait.

Vous ne pouvez pas ajouter plus de quantité de produit qu'il n'y a de quantité disponible.

### Enlever un produit <a href="#commandes-enleverunproduit" id="commandes-enleverunproduit"></a>

Pour annuler un produit, rendez-vous dans la liste de produits et, au choix, soit supprimer le produit en cliquant sur l'action "Supprimer", soit en cliquant sur l'action "Modifier" si vous souhaitez simplement enlever de la quantité de produit.

Vous pouvez modifier la quantité de plusieurs produits à la fois.\
&#x20;Si la quantité d'un produit atteint 0, il est enlevé directement de la commande.\
&#x20;Vous ne pouvez pas enlever plus de quantité que celle déjà en place dans la commande.\
&#x20;Cliquez sur l'icône de croix rouge pour annuler votre modification.

## Modifier les détails de la commande <a href="#commandes-modifierlesdetailsdelacommande" id="commandes-modifierlesdetailsdelacommande"></a>

De nombreuses sections de la commande peuvent être modifiées, vous permettant de les mettre à jour ou de corriger les données fournis par le client.

### État de la commande <a href="#commandes-etatdelacommande" id="commandes-etatdelacommande"></a>

La première liste déroulante de la page de commande vous permet de changer son état. C'est un aspect très important du processus de suivi d'une commande, car chaque étape débloquera des fonctionnalités et documentations pour la commande.

Vous pouvez choisir parmi les états suivants :

* Annulé.
* En attente de réapprovisionnement.
* En attente du paiement par chèque.
* En attente du paiement par PayPal.
* En attente du paiement par virement bancaire.
* En cours de livraison.
* Erreur de paiement.
* Livré.
* Paiement à distance accepté.
* Paiement accepté.
* Préparation en cours.
* Remboursé.

Afin d'avoir un meilleur aperçu des évolutions de la commande, chaque changement d'état est enregistré, et le journal apparaît juste en-dessous de la liste déroulante. De fait, vous devriez ne changer un état que s'il a été clairement confirmé : n'indiquez pas qu'une commande a atteint l'état "Livré" alors que vous venez d'envoyer le colis, utilisez plutôt "En cours de livraison" ; n'utilisez pas "Préparation en cours" si vous n'avez fait que jeter un oeil rapide à la commande, etc.

### Boutons d'action <a href="#commandes-boutonsdaction" id="commandes-boutonsdaction"></a>

Les boutons d'action de la barre supérieure dépendent de l'état de la commande. Par exemple, une fois que la commande est marquée comme livrée, les boutons "Ajouter un produit" et "Enlever des produits" sont remplacés par deux nouveaux boutons : "Retourner un produit" et "Remboursement partiel".

Le retour produit n'est pas activé par défaut. Pour l'activer, allez dans la page "Retours produit" du menu "Commandes", et activez l'option se trouvant en bas de la page. Ce réglage s'appliquera à tous les produits et toutes les commandes.

* **Retourner les produits**. Ne doit être qu'à partir du moment où un client vous a effectivement renvoyé des produits : une fois que le paquet a été reçu, vous devez marquer les produits comme retournés directement dans la page de la commande. Cliquez sur le bouton "Retourner les produits" et une nouvelle colonne apparaîtra dans le tableau des produits, intitulée "Retour". Cochez la case du ou des produits concernés, indiquez la quantité retournée, et cliquez sur le bouton "Retourner les produits" en bas du tableau.
* **Remboursement partiel**. Ne doit être utilisé que quand vous souhaitez rembourser une partie de la commande, et non la commande entière, quelle que soit la raison – ce peut être parce qu'un client vous a renvoyé un produit, ou simplement pour faire un geste commercial pour un produit endommagé que le client a décidé de garder malgré tout. Cliquez sur le bouton "Remboursement partiel" et une nouvelle colonne apparaîtra dans le tableau des produits, intitulée "Remboursement partiel". Indiquez le montant et la quantité pour chacun des produits affectés, choisissez l'une des options situées en bas de la liste (voir ci-dessous) et cliquez sur le bouton "Remboursement partiel" en bas du tableau.

Quand vous marquez des produits comme ayant été retournés ou à rembourser, quatre options sont disponibles sous le tableau des produits :

* **Réinjecter**. Une fois coché, PrestaShop considère que le produit renvoyé est remis en vente, et augmentera alors le stock de ce produit. Ne cliquez pas cette option si un produit a été renvoyé car il était cassé...
* **Générer un avoir**. Une fois coché, un avoir sera créé, correspondant au montant des produits sélectionnés. Un avoir est l'indication que vous reconnaissez qu'un produit a été retourné et qu'un remboursement a été mis en place. Le client peut utiliser cet avoir pour son prochain achat.
*   **Bon de réduction**. Une fois coché, un bon de réduction sera créé, correspondant au montant des produits sélectionnés. Un bon de réduction prend la forme d'un code de réduction que le client peut saisir lors du processus de commande.\
    Vous pouvez modifier les bons existants du client en affichant la page du client : depuis la page de la commande actuelle, cliquez sur le lien sous le nom du client dans la section "Information client" ; une fois sur la page du client, allez dans la section "Bons". Vous pouvez modifier chaque bon en cliquant sur leur icône "Modifier".

    Depuis PrestaShop 1.5, les bons de réduction font partie d'une nouvelle fonctionnalité : les "règles de paniers". Elles peuvent être créées et modifiées depuis la page "Règles paniers", dans le menu "Promotions". Le processus de création d'une règle panier est expliqué dans le chapitre suivant, "Mettre en place des promotions".
* **Rembourser les frais d'envoi**. Vous pouvez aussi choisir de rembourser les frais d'expédition, ce qui est toujours apprécié.

La différence entre un avoir, un bon de réduction et une règle panier

Un avoir est avant tout une preuve écrite qu'un produit a été retourné. La plupart du temps, le client peut s'en servir comme d'un bon de réduction

Un bon de réduction est un code promotionnel qui n'a pas à être lié à un retour marchandise ou à un remboursement, et peut prendre plus de formes qu'un simple avoir :

* une réduction sur une commande (en pourcentage).
* une réduction sur une commande (un montant précis).
* la livraison gratuite.

Vous pouvez appliquer un bon de réduction à tous vos clients, ou un groupe de clients, ou à un seul client ; vous pouvez également lui donner une date d'expiration.

Une règle de panier est une version améliorée du bon de réduction : en plus de faire ce que pouvait faire un bon de rédaction dans PrestaShop 1.4, le système règles paniers introduit avec PrestaShop 1.5 vous permet de :

* Donner un nom à la réduction.
* Autoriser le client à n'utiliser qu'une partie de la réduction.
* Mettre en place des priorités entre règles paniers.
* Indiquer la compatibilité entre règles paniers.
* Faire en sorte que la réduction ne fonctionne qu'avec certains transporteurs.
* Faire en sorte que la réduction ne fonctionne qu'avec une sélection de produits et/ou de catégories et/ou de marques et/ou de fournisseurs et/ou d'attributs... ou tous en même temps si nécessaire !
* Faire en sorte que la réduction comprenne la livraison gratuite et/ou une réduction sur la commande et/ou un produit gratuit... ou tous en même temps si nécessaire !

### Documents <a href="#commandes-documents" id="commandes-documents"></a>

Vous pouvez obtenir de nombreux documents PDF depuis la page de la commande. Une fois rendus disponibles, ils sont listés dans la section "Documents" de la page.

Par défaut, vous pouvez télécharger la commande elle-même au format PDF, en cliquant sur le bouton "Imprimer la commande" en haut à droite.

Vous pouvez récupérer la facture de la commande en cliquant sur le bouton "Générer la facture" de la section "Documents". La facture peut également être générée une fois que vous avez passé la commande à l'état "Paiement accepté".\
Une fois généré, le bouton "Afficher la facture" apparaît sous la barre principale.

Vous pouvez facilement personnaliser l'apparence de la facture : les modèles de fichiers PDF sont situés dans le dossier `/pdf`. Ces fichiers `.tpl` sont en fait des fichiers HTML contenant des balises Smarty pour les données dynamiques. Vous pouvez modifier l'apparence de la facture en modifiant le fichier `invoice.tpl`.

Une fois que vous avez mis la commande à l'état "Préparation en cours", un bon de livraison en PDF est généré, que vous pouvez ensuite télécharger depuis la section "Documents".

### Transport <a href="#commandes-transport" id="commandes-transport"></a>

Les détails de livraison de la commande en cours peuvent être en partie modifiés. Plus précisément, vous pouvez modifier le numéro de suivi : dans la section "Transport", cliquez sur l'icône d'édition de la colonne "Numéro de suivi", et saisissez votre nouveau numéro.

### Adresse de livraison <a href="#commandes-adressedelivraison" id="commandes-adressedelivraison"></a>

La section "Adresse de livraison" vous permet de modifier l'adresse de destination du colis que votre équipe s'apprête à envoyer. Vous pouvez soit utiliser la liste déroulante pour choisir une autre des adresses que le client a déjà enregistré dans votre boutique, ou vous pouvez utiliser l'icône "Modifier" pour corriger l'adresse actuellement utilisée.

Si vous avez besoin d'envoyer un colis à une adresse qui n'est pas encore enregistrée dans PrestaShop, vous devez d'abord la créer. Pour ce faire, rendez-vous dans le menu "Clients", ouvrez la page "Adresses", et cliquez sur le bouton "Créer". N'oubliez pas de mettre la bonne adresse e-mail du client, car c'est de cette manière que PrestaShop saura associer la nouvelle adresse avec votre client existant ! Ceci fait, retournez dans la page de la commande, et changez l'adresse à l'aide de la liste déroulante.

Notez l'icône "G" : elle vous permet de localiser l'adresse de destination sur Google Maps.

### Adresse de facturation <a href="#commandes-adressedefacturation" id="commandes-adressedefacturation"></a>

La section "Adresse de facturation" vous permet de modifier l'adresse de règlement de la commande. De la même manière que pour l'adresse de livraison, vous pouvez soit utiliser la liste déroulante pour choisir une autre des adresses que le client a déjà enregistré dans votre boutique, ou vous pouvez utiliser l'icône "Modifier" pour corriger l'adresse actuellement utilisée.

Si vous avez besoin que le règlement soit associé à une adresse qui n'est pas encore enregistrée dans PrestaShop, vous devez d'abord la créer. Pour ce faire, rendez-vous dans le menu "Clients", ouvrez la page "Adresses", et cliquez sur le bouton "Créer". N'oubliez pas de mettre la bonne adresse e-mail du client, car c'est de cette manière que PrestaShop saura associer la nouvelle adresse avec votre client existant ! Ceci fait, retournez dans la page de la commande, et changez l'adresse à l'aide de la liste déroulante.

### Réduction <a href="#commandes-reduction" id="commandes-reduction"></a>

Dans la section "Produits", en-dessous de la liste des produits, vous pouvez trouver un tableau vide, avec un bouton "Ajouter une réduction". Cela crée une simple réduction, pas aussi élaborée qu'avec le système règles paniers/bon d'achat, mais reste cependant utile.

En cliquant sur le bouton, un nouveau formulaire s'ouvre, avec les éléments suivants :

* **Nom**. Donnez un nom à cette réduction. Il sera lisible par le client.
* **Type**. Choisissez un type de réduction : "pourcentage", "montant" ou "livraison offerte".
* **Valeur**. Pour les types "pourcentage" ou "montant", vous devez indiquer la valeur de la réduction.
* **Facture**. Sélectionnez la facture à laquelle cette réduction sera appliquée. S'il y a plus d'une facture, vous pouvez cocher une case afin d'appliquer la réduction à toutes les factures.

La réduction sera appliquée au total avant l'application des coûts d'expédition.

## Attacher un commentaire à la commande <a href="#commandes-attacheruncommentairealacommande" id="commandes-attacheruncommentairealacommande"></a>

Avec la section "Nouveau message", à droite de la page, vous pouvez laisser un commentaire à destination de votre équipe.

Vous pouvez également envoyer ce message à votre client, afin de lui donner des informations relatives à la commande, à un retard, une surprise, ou pour le tenir informé des offres et promotions en cours. C'est là un aspect essentiel de la relation client.

Deux liens sont disponibles :

* **Cliquez ici pour ajouter un commentaire ou envoyer un message au client**.
  * Vous pouvez ajouter votre message simplement en remplissant le champ texte et en cliquant sur "Envoyer". Le message sera intégré à la base SAV du client, accessible depuis soit la page du client, soit depuis la page du SAV. Le message sera également envoyé à l'adresse e-mail du client si vous en avez fait le choix.
  * Vous pouvez enregistrer des messages pré-écrits et les réutiliser autant de fois que nécessaire, ce qui vous économise du temps de rédaction. Pour envoyer l'un de ces messages, sélectionnez-le dans la liste déroulante. Vous pouvez ensuite y ajouter plus de détails si nécessaire.\
    &#x20;Vous pouvez créer autant de message pré-écrits que vous le souhaitez à l'aide de l'outil de la page "Message prédéfinis" de la page "Commandes".
* **Cliquez ici pour voir tous les messages**. Ce lien mène à la page du Service Après-Vente, disponible dans le menu "Clients". Cette page est expliquée en détails dans le chapitre "Gérer les clients" de ce guide.
