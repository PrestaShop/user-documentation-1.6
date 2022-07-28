# Préférences de l'administration

La page d'administration "Préférences" contient des options et réglages concernant la manière dont PrestaShop lui-même fonctionne. Elle contient quatre sections.

## Général <a href="#preferencesdeladministration-general" id="preferencesdeladministration-general"></a>

Cette section comprend quatre réglages :

![](../../../.gitbook/assets/23789901.png)

* **Vérifier automatiquement les mises à jour de modules**. Vous pouvez demander à PrestaShop de régulièrement vérifier s'il existe de nouvelles versions de vos modules sur le site Addons. Si c'est le cas, la page "Modules" affichera un bouton "Mettre à jour !".
* **Vérifier l'adresse IP du cookie**. Il s'agit d'une mesure de sécurité supplémentaire : vous pouvez dire à PrestaShop de vérifier que l'utilisateur vient bien de l'IP stockée dans le cookie de son navigateur.
* **Durée de vie du cookie front-office**. Par défaut, un cookie de PrestaShop dure 480 heures (20 jours). Vous pouvez réduire sa longévité si vous estimez que la sécurité de votre boutique en dépend.
* **Durée de vie du cookie back-office**. Par défaut, un cookie de PrestaShop dure 480 heures (20 jours). Vous pouvez réduire sa longévité si vous estimez que la sécurité de votre boutique en dépend.

## Quota de téléchargement <a href="#preferencesdeladministration-quotadetelechargement" id="preferencesdeladministration-quotadetelechargement"></a>

Cette page vous aide à définir la taille autorisée de fichiers mis en ligne par votre propre équipe – pas la limite imposée à vos clients.

![](../../../.gitbook/assets/23789902.png)

Trois options sont présentes, la première étant très générale et les deux suivantes plus spécifiques :

* **Poids maximum des fichiers joints**. La valeur par défaut est prise directement des réglages de votre serveur, mais vous pouvez la baisser si besoin est.
* **Taille maximale d'un produit téléchargeable**. Si vous vendez des produits dématérialisés (services, réservations, fichiers téléchargeables), ce réglage vous permet de limiter la taille des fichiers que votre équipe peut mettre en ligne – et donc, la taille du produit final. Prévoyez bien votre usage, afin de ne pas bloquer un membre de votre équipe qui doit mettre en ligne un fichier plus lourd que prévu.
* **Taille maximum des images des produits**. De la même manière, vous pouvez limiter la taille des images que vous ou votre équipe pouvez mettre en ligne sur votre boutique. Cela peut servir de rappel pratique à votre équipe, les poussant à réduire le poids d'une image, étant donné qu'il est rarement utile d'utiliser des images de plus de 600x600 pixels (ce qui correspond environ à 200 ko une fois correctement compressé). Allez sur la page de préférences "Images" pour voir les différentes tailles configurées dans votre installation de PrestaShop. Autre avantage : vous utilisez ainsi moins de bande passante, et moins de temps processeur (étant donné que PrestaShop redimensionne les images et crée des miniatures, entre autres formats).

## Aide <a href="#preferencesdeladministration-aide" id="preferencesdeladministration-aide"></a>

Afin de vous aider dans votre quotidien sous PrestaShop, l'équipe de développement a ajouté de nombreuses aides dans l'interface.

![](../../../.gitbook/assets/23789903.png)

Vous pouvez les afficher à l'aide de ces deux options :

* **Bulles d'aide du back-office**. Cela affichera des sections d'aide jaunes sous les champs les plus complexes.
* **Masquer les conseils d'optimisation**. Cela affichera une section de conseils de configuration sur la page d'accueil du back-office.

## Notifications <a href="#preferencesdeladministration-notifications" id="preferencesdeladministration-notifications"></a>

Les notifications sont de petites bulles numérotées, situées tout en haut de n'importe quelle page de l'administration, juste à côté du nom de la boutique. Elles affichent le nombre de nouveaux éléments depuis la dernière fois que vous les avez cliquées.

![](../../../.gitbook/assets/23789904.png)

Vous pouvez choisir de ne pas en recevoir pour certains types de contenus :

* **Affiche les notifications pour les nouvelles commandes**. En cliquant sur cette notification, l'interface affichera le nombre de commandes récentes, leurs montants et le nom des clients. De là, vous pouvez soit ouvrir la page individuelle de chaque commande, ou ouvrir la page "Commandes" pour obtenir la liste complète.
* **Affiche les notifications pour les nouveaux clients**. En cliquant sur cette notification, l'interface affichera les noms des utilisateurs inscrits depuis votre dernière vérification. De là, vous pouvez soit ouvrir la page individuelle de chaque client, ou ouvrir la page "Clients" pour obtenir la liste complète.
* **Affiche les notifications pour les nouveaux messages**. En cliquant sur cette notification, l'interface affichera les e-mails des personnes qui vous ont envoyé un message à l'aide du formulaire de contact de votre boutique. De là, vous pouvez soit ouvrir un message individuel, ou ouvrir la page "SAV" pour la liste complète.
