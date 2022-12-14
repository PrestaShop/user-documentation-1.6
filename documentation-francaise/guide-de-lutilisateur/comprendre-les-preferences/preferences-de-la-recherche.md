# Préférences de la recherche

La page "Recherche" vous permet de configurer les fonctionnalités de recherche de votre boutique.

## Liste d'alias <a href="#preferencesdelarecherche-listedalias" id="preferencesdelarecherche-listedalias"></a>

Quand vos clients lancent une requête sur le moteur de recherche interne de votre boutique, ils peuvent faire des erreurs. Si PrestaShop n'affiche pas les bons résultats, la fonctionnalité "alias" peut s'en occuper. Vous êtes ici en mesure d'enregistrer des mots contenant des erreurs de syntaxe, et de les faire pointer vers les bons produits.

![](../../../.gitbook/assets/23789823.png)

Pour créer un nouvel alias utile, vous devriez d'abord trouver les erreurs de vos clients les plus courantes :

1. Rendez-vous sur l'onglet "Recherches de la boutique" de la page "Statistiques", dans le menu du même nom. Vous pouvez y découvrir les mots saisis par vos clients, dont les plus fréquentes erreurs.
2. Prenez les plus fréquentes, et ajoutez-les à votre liste d'alias, afin de les faire pointer vers les bons produits.
3. Cliquez sur le bouton "Créer" de la page de préférence "Recherche".

Le formulaire de création est très simple : indiquez l'erreur que vous voulez voir corrigée, et le mot correct qui y correspond.

![](../../../.gitbook/assets/23789825.png)

Par exemple, supposons que vos visiteurs utilisent fréquemment "letceur" ou "lecture" plutôt que "lecteur". Vous pouvez créer un alias pour chacune de ces erreurs, et leur faire correspondre "lecteur". Les alias sont en place dès qu'ils sont enregistrés.

Nous vous invitons également à consulter la section de ce guide sur les balises méta de produits et de catégories, afin de mieux comprendre comment afficher des produits en fonction des mots saisis par le client. Rendez-vous sur les chapitres "Ajouter des produits et des catégories de produits" et "Un aperçu du catalogue".

## Indexation <a href="#preferencesdelarecherche-indexation" id="preferencesdelarecherche-indexation"></a>

Cette section fournit des informations sur le nombre de produits qui sont accessibles au moteur de recherche interne à votre boutique, et les compare au nombre de produits présents dans la base de données. Si les valeurs ne correspondent pas, vous devez sélectionner l'option "Ajouter à l'index les produits manquant". Seuls les nouveaux produits seront indexés.

![](../../../.gitbook/assets/23789827.png)

Si vous avez fait de nombreuses modifications à des produits déjà indexés, vous pourriez préférer reconstruire l'intégralité de votre index. Le processus "Reconstruire l'index" prend plus de temps, mais il est exhaustif.

PrestaShop vous donne également une adresse afin de créer une tâche cron permettant de régulièrement reconstruire votre index. Si vous ne savez pas ce que qu'est une tâche cron ou un crontab, contactez votre hébergeur.

## Options de recherche <a href="#preferencesdelarecherche-optionsderecherche" id="preferencesdelarecherche-optionsderecherche"></a>

Cette section vous permet de configurer le comportement du moteur de recherche interne à votre boutique :

![](../../../.gitbook/assets/23789828.png)

* **Recherche Ajax**. Activer cette option fait que le client obtiendra une liste de 10 résultats dès qu'il aura saisi ses premières lettres dans le moteur de recherche, affichés juste sous celui-ci.
* **Recherche instantanée**. Activer cette option fait que le client obtiendra une liste de résultats dès qu'il aura saisi ses premières lettres dans le moteur de recherche, affichés dans la colonne centrale de la boutique. Cette option est désactivée par défaut car de nombreux visiteurs ne sont pas habitués à voir le contenu entier d'une page remplacé par des résultats de recherche sans même avoir à cliquer sur un bouton. De fait, à utiliser avec précaution.
* **Taille de mot minimum**. Vous pouvez choisir le nombre de caractères minimal à partir duquel un mot est enregistré dans l'index de recherche, et donc peut être trouvé par vos clients. Cette fonctionnalité vous permet d'éliminer les mots courts de la recherche, tels que les prépositions ou les articles (le, et, de, etc.).
* **Mots à ne pas indexer**. Vous pouvez choisir les mots qui ne doivent pas être trouvables pour vos clients. Saisissez-les directement dans le champ, séparés par "|".

## Poids <a href="#preferencesdelarecherche-poids" id="preferencesdelarecherche-poids"></a>

PrestaShop vous permet de prioriser certaines données quand une recherche est lancée sur votre boutique.

![](../../../.gitbook/assets/23789829.png)

Comme indiqué dans cette section, le "poids" d'un mot représente son importance et sa pertinence pour le classement des produits lorsqu'un client lance une nouvelle recherche.\
&#x20;Un élément disposant d'un poids égal à 8 aura 4 fois plus de valeur qu'un élément au poids égal à 2.

Par exemple, par défaut "Poids du nom du produit" est à 6, "Poids des tags" est à 4, et "Poids de la description courte" ainsi que "Poids de la description longue" sont à 1. Cela signifie qu'un produit avec "ipod" dans son nom apparaîtra plus haut dans les résultats de recherche qu'un autre produit n'ayant "ipod" que dans ses tags. De son côté, un produit n'ayant "ipod" que dans l'une de ses descriptions aura le classement le plus bas des résultats.

De nombreux facteurs peuvent ainsi se voir assigner un poids : description courte, catégorie, tags, attributs, etc. Vous vous rendrez compte que les résultats peuvent être inversés simplement en changeant le poids de certains champs. L'affinement de ces réglages sera surtout visible sur les catalogues ayant de nombreuses références.

Vos changements sont pris en compte dès qu'ils sont enregistrés.
