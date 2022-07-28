# Concepts généraux

## Concepts généraux <a href="#conceptsgeneraux-conceptsgeneraux" id="conceptsgeneraux-conceptsgeneraux"></a>

Afin d'éviter toute confusion avec la gestion des stocks de la version 1.4, il convient de présenter deux concepts distincts : les stocks physiques et les quantités de produits disponibles à la vente.

### Les quantités de produits disponibles à la vente <a href="#conceptsgeneraux-lesquantitesdeproduitsdisponiblesalavente" id="conceptsgeneraux-lesquantitesdeproduitsdisponiblesalavente"></a>

Cela correspond à la gestion des stocks dans PrestaShop 1.4.x. Il s'agit des quantités qui sont affichées en boutique pour chaque produit et déclinaison de produit. C'est cette quantité qui définit si le produit peut être commandé ou non (sauf si l'option "Autoriser la commande de produits hors stock" est activée). Cette quantité peut être définie manuellement pour chaque produit et déclinaison de produit.

Depuis PrestaShop 1.5.x, cette quantité peut être automatiquement déterminée en fonction du stock physique du produit concerné. Dans le cas d'une utilisation multiboutique, la quantité doit être définie pour chaque boutique.

Par conséquent, ce qui était appelé "stock" dans PrestaShop 1.4.x est maintenant appelé "quantités de produits disponibles à la vente" depuis  PrestaShop 1.5.x.

### Les stocks de produits (stockés physiquement) <a href="#conceptsgeneraux-lesstocksdeproduits-stockesphysiquement" id="conceptsgeneraux-lesstocksdeproduits-stockesphysiquement"></a>

Cela correspond à la gestion des produits réellement stockés dans un ou plusieurs lieux de stockage ou entrepôts. C'est ce nouveau concept qui est appelé "stock" lors de son introduction dans PrestaShop 1.5.x

Cette nouvelle gestion de stocks inclus les mouvements de stocks, la valorisation du stock, les transferts de stocks entre entrepôts, l'intégration avec le mode multiboutique et la gestion de commandes aux fournisseurs.

Elle permet aussi de prendre en compte la notion de stock réel. A un instant T, un produit peut être disponible dans le stock physique mais plus disponible à la vente du fait de commandes clients en attente d'expédition. Ce même produit peut aussi faire l'objet d'une commande fournisseur en cours de livraison, et donc pas encore comptabilisée dans le stock physique.

Le stock réel est donc constitué du stock physiquement présent dans un entrepôt, auquel on ajoute les quantités en cours de commande aux fournisseurs, et duquel on retranche les quantités commandées par les clients pour lesquelles les commandes n'ont pas encore été expédiées.

## Utilisation de la nouvelle gestion des stocks <a href="#conceptsgeneraux-utilisationdelanouvellegestiondesstocks" id="conceptsgeneraux-utilisationdelanouvellegestiondesstocks"></a>

### Est-ce obligatoire d'utiliser la nouvelle gestion des stocks ? <a href="#conceptsgeneraux-est-ceobligatoiredutiliserlanouvellegestiondesstocks" id="conceptsgeneraux-est-ceobligatoiredutiliserlanouvellegestiondesstocks"></a>

Il n'est pas obligatoire d'utiliser la nouvelle gestion des stocks, de la même façon qu'il n'est pas obligatoire d'utiliser la gestion des quantités disponibles à la vente.

L'activation de la gestion des quantités disponibles à la vente et de la gestion des stocks se fait dans la page de préférences "Produits". Descendez jusqu'à la section "Stocks produit" et mettez "Oui" pour les deux options de gestion du stock. Vous devrez d'abord activer la gestion des stocks avant de pouvoir activer la gestion avancée des stocks.

L'activation de la gestion avancée des stocks, et d'une façon générale la gestion de votre stock et de vos entrepôts, est indépendante de la fonctionnalité multiboutique. Par conséquent, quelle que soit la boutique en cours d'administration dans le back-office de PrestaShop, lorsque vous vous trouvez dans le menu "Stock", vous gérer toujours votre stock de façon globale.

### Comment faire pour ne rien changer à ce que j'avais avec PrestaShop 1.4.x/1.5.x ? <a href="#conceptsgeneraux-commentfairepournerienchangeracequejavaisavecprestashop1.4.x-1.5.x" id="conceptsgeneraux-commentfairepournerienchangeracequejavaisavecprestashop1.4.x-1.5.x"></a>

Si vous ne souhaitez pas bénéficier de la gestion avancée des stocks de PrestaShop 1.5 et êtes pleinement satisfait du fonctionnement "classique" de la gestion des quantités de vos produits, il vous suffit d'activer la gestion des quantités de produits et de ne pas activer la gestion avancée des stocks : rendez-vous dans la page de préférences "Produits", descendez jusqu'à la section "Stocks produit" et mettez "Oui" pour l'option "Activer la gestion des stocks" en laissant l'option "Activer la gestion des stocks avancée" à "Non".

La gestion des quantités disponibles à la vente de vos produits est désormais centralisée dans l'onglet "Quantités" de la fiche produit : créez un nouveau produit ou modifiez un produit existant, et l'onglet apparaît parmi tous les autres, à gauche de l'écran.

### La nouvelle gestion des stocks s'applique-t-elle à mon cas ? <a href="#conceptsgeneraux-lanouvellegestiondesstockssapplique-t-elleamoncas" id="conceptsgeneraux-lanouvellegestiondesstockssapplique-t-elleamoncas"></a>

La nouvelle gestion des stocks permet de gérer un stock de produits de façon avancée. Cette fonctionnalité s'applique à votre activité si :

* Vous gérez un stock des produits en vente sur votre (vos) boutique(s).
* Vous utilisez au moins un lieu de stockage (entrepôt) que vous gérez vous-même.
* Vous commandez tout ou partie de vos produits à un ou plusieurs fournisseurs.
* Vous avez besoin de statistiques sur l'état de votre stock et de votre (vos) entrepôt(s).

Cette fonctionnalité ne s'applique pas à votre activité si :

* Vous ne gérez pas les stocks des produits en vente sur votre boutique.
* Vous possédez déjà un système de gestion de stock dont vous souhaitez poursuivre l'utilisation sans rien changer.
