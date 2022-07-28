# Règles de gestion des stocks

Vous trouverez ici les règles de gestion appliquées automatiquement dans la gestion des stocks.

Chaque entrée ou sortie de stock doit pouvoir être valorisée. C'est pourquoi chaque produit unitaire entré en stock doit avoir un prix unitaire hors taxes (d'achat ou de production) associé que ce soit par l'intermédiaire d'une commande fournisseur, ou d'une entrée manuelle. Et chaque sortie de produit doit aussi être valorisée.

Il existe pour cela trois méthodes de valorisation principales qu'il faut choisir en fonction de son activité ou des règles en vigueur dans son pays pour chaque entrepôt :

* FIFO (premier entré, premier sorti).
* LIFO (dernier entré, premier sorti).
* CUMP (Coût Unitaire Moyen Pondéré).

Dans le cas des méthodes FIFO et LIFO, chaque produit unitaire dans le stock possède un prix d'achat fixé au moment de son ajout au stock. Ainsi, pour une référence donnée disponible en 100 exemplaires, 40 exemplaires peuvent avoir un prix d'achat X, et 60 un prix d'achat Y. Lors du passage d'une commande, et selon la méthode choisie, on sait quel produit réserver et à quel prix d'achat, ce qui permet de gérer précisément un éventuel retour de commande et remettre les produits en stock avec leurs prix d'achat d'origine.

Le tableau ci-dessous illustre l'utilisation de la méthode LIFO pour valoriser un stock. Dans ce cas, on construit un tableau à deux entrées (prix et quantités par type de mouvement). On ajoute de nouvelles colonnes au fur et à mesure des réceptions faites avec de nouveaux prix.

| Prix            | 4     | 6     | 7   |
| --------------- | ----- | ----- | --- |
| Stock initial   | 1000  |       |     |
| Entrée          |       | 500   |     |
| Sortie          | (700) |       |     |
| Sortie          | (300) | (400) |     |
| Entrée          |       |       | 900 |
| État instantané | 0     | 100   | 900 |

La valeur du stock lors de l'état instantané dans ce cas est de 6900.

Le tableau ci-dessous illustre l'utilisation de la méthode LIFO pour valoriser un stock. Nous reprenons les mêmes entrées et sorties que dans l’exemple précédent. Le principe est identique au cas du FIFO, sauf que lors des sorties, on consomme prioritairement les dernières unités entrées.

| Prix            | 4     | 6     | 7   |
| --------------- | ----- | ----- | --- |
| Stock initial   | 1000  |       |     |
| Entrée          |       | 500   |     |
| Sortie          | (200) | (500) |     |
| Sortie          | (700) |       |     |
| Entrée          |       |       | 900 |
| État instantané | 100   | 0     | 900 |

La valeur du stock lors de l'état instantané dans ce cas est de 6700.

La troisième méthode couramment utilisée pour valoriser un stock est le Coût Unitaire Moyen Pondéré. Le calcul du CUMP se fait après chaque entrée dans le stock.

Pour un produit donné, le calcul du CUMP se fait avec la formule :

CUMP = (QS \* CUMP précédent + QA \* CU) / (QS + QA)\
&#x20;Sauf si QS est négative ou nulle, auquel cas CUMP = CU.

Avec :

* QS = Quantité actuellement en stock, ou stock initial.
* QA = Quantité à ajouter en stock.
* CU = Coût Unitaire (prix d'achat HT ou coût de production).

Le tableau ci-dessous illustre l'évolution du CUMP en prenant l'exemple d'un produit initialement en 20 exemplaires en stock, et acheté à un prix unitaire de 2. Les nouvelles entrées/sorties seront valorisés de la façon suivante :

|               | Entrées | PU entrées | Sorties | PU sorties | CUMP | Valeur du stock |
| ------------- | ------- | ---------- | ------- | ---------- | ---- | --------------- |
| Stock Initial | 20      | 2          |         |            | 2    | 40              |
| Date X        |         |            | 12      | 2          | 2    | 16              |
| Date Y        | 20      | 3.4        |         |            | 3\*  | 84              |
| Date Z        |         |            | 10      | 3          | 3    | 54              |

\* Détail du calcul : ((8 quantités restantes en stock \* 2) + (20 quantités à ajouter \*3,4)) / 28 quantités au total = 3.

À la date Y, on a donc recalculé le CUMP en fonction du nombre de produits ajoutés au stock et de leur nouvelle valeur unitaire. L'ensemble des produits en stock a donc une valeur unitaire réaffectée en fonction du nouveau CUMP.
