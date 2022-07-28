# Dépannage

**Contenu**

* [Dépannage](depannage.md#Dépannage-Dépannage)
  * [Activer l'affichage des erreurs en cas de pages blanches inattendues et répétées](depannage.md#Dépannage-Activerl%27affichagedeserreursencasdepagesblanchesinattenduesetrépétées)
  * [Hébergement chez 1&1 : résoudre les problèmes de mémoire](depannage.md#Dépannage-Hébergementchez1&1:résoudrelesproblèmesdemémoire)
  * [Il est impossible de se connecter](depannage.md#Dépannage-Ilestimpossibledeseconnecter)
  * [Regénérer le mot de passe manuellement](depannage.md#Dépannage-Regénérerlemotdepassemanuellement)
  * [PrestaShop ne m'envoie pas mon nouveau mot de passe](depannage.md#Dépannage-PrestaShopnem%27envoiepasmonnouveaumotdepasse)
  * [Se connecter après avoir effacé un pack de langue par erreur](depannage.md#Dépannage-Seconnecteraprèsavoireffacéunpackdelangueparerreur)

## Dépannage <a href="#depannage-depannage" id="depannage-depannage"></a>

### Activer l'affichage des erreurs en cas de pages blanches inattendues et répétées <a href="#depannage-activerlaffichagedeserreursencasdepagesblanchesinattenduesetrepetees" id="depannage-activerlaffichagedeserreursencasdepagesblanchesinattenduesetrepetees"></a>

Si le front-office ou le back-office de votre boutique se met à afficher une page blanche ou incomplète régulièrement sans donner de message d'erreur, il est nécessaire d'activer l'affichage des erreurs PHP pour comprendre le problème.

Pour ce faire, vous devez ouvrir le fichier `/config/defines.inc.php` de votre installation de PrestaShop, et modifier la ligne suivante :

```
define('_PS_MODE_DEV_', false);
```

...afin qu'elle ressemble à ceci :

```
define('_PS_MODE_DEV_', true);
```

Parcourez ensuite votre boutique afin de revoir cette page blanche, qui devrait cette fois s'accompagner de messages d'erreur, qui devraient vous aider à résoudre le problème.

Une fois que le problème a été résolu, remettez la ligne du fichier `/config/defines.inc.php` telle qu'elle était avant, avec la constante `_PS_MODE_DEV_` réglée à `false`.

### Hébergement chez 1&1 : résoudre les problèmes de mémoire <a href="#depannage-hebergementchez1-and-1-resoudrelesproblemesdememoire" id="depannage-hebergementchez1-and-1-resoudrelesproblemesdememoire"></a>

Certains utilisateurs peuvent rencontrer des soucis d'allocation mémoire, en particulier lorsque le back-office tente d'afficher des images qui sont assez grosses sur le disque (plus de 800 ko). Sachez que même si vous augmentez manuellement la limite de mémoire pour la passer à 128 Mo, certains hébergeurs web, tel que 1&1, conserve la limite à 32 Mo. Lisez cette FAQ de 1&1 : [http://faq.1and1.fr/scripts/php/5.html](http://faq.1and1.fr/scripts/php/5.html).

Il n'y a que deux solutions à ce problème, et elles sont toutes les deux radicales :

* Baissez la taille de vos images en pixels, et donc leur taille sur le disque. Cela aura l'autre avantage d'améliorer les performances globales.
* Passez chez un autre hébergeur qui donne la possibilité d'augmenter la mémoire allouée.

### Il est impossible de se connecter <a href="#depannage-ilestimpossibledeseconnecter" id="depannage-ilestimpossibledeseconnecter"></a>

Dans certaines situations, PrestaShop peut ne plus reconnaître les identifiants d'un utilisateur, ce qui rend la connexion impossible autant au front-office qu'au back-office. L'utilisateur est simplement renvoyé vers l'écran de connexion. Les retours reçus tendent à indiquer que ce problème arrive surtout avec le navigateur IE10.

Il s'agit très certainement d'un problème avec les cookies de votre boutique : lorsque l'utilisateur se déconnecte et se reconnecte souvent de la boutique, les clés de cryptage du cookie peuvent se mélange.

Dans tous les cas, une manière simple de régler ce problème et enfin pouvoir à nouveau se connecter consiste à vider le cache du navigateur et à supprimer ses cookies. Voici une page expliquant cela en fonction du navigateur : [https://support.google.com/mail/answer/32050?hl=fr](https://support.google.com/mail/answer/32050?hl=fr).

### Regénérer le mot de passe manuellement <a href="#depannage-regenererlemotdepassemanuellement" id="depannage-regenererlemotdepassemanuellement"></a>

Dans certains cas, rien n'arrive lorsque vous faites une demande de renouvellement de votre mot de passer. Il peut y avoir plusieurs causes à cela, mais le plus important reste de pouvoir vous connecter à nouveau à votre compte.

Le processus nécessite que vous accédiez à votre base de données, par exemple à l'aide de phpMyAdmin.

Voici la procédure à suivre :

1. Ouvrez le fichier `settings.inc.php`, que vous trouverez dans le dossier `/config` à la racine de votre installation de PrestaShop. Trouvez la ligne contenant "`_COOKIE_KEY`\_". Copiez le contenu de sa valeur (sans les apostrophes) : il s'agit du MD5 de votre mot de passe actuel.
2. Vous devez maintenant générer un nouveau hash MD5 de votre mot de passe :\

   1. Ouvrez le site [http://www.md5.fr/](http://www.md5.fr/)
   2. Collez le contenu de la valeur "`_COOKIE_KEY`\_", et saisissez votre nouveau mot de passe juste après. Par exemple, xykxB41JrEacRIoZxDioPNRmKeuO3ixCLygNxBAkeOkAHf2YUVESuT9jMONMOTDEPASSE, où la valeur se termine par T9j, et le nouveau mot de passe est MONMOTDEPASSE (cela peut être n'importe quel mot de passe).
   3. Cliquez sur le bouton "Convertir en MD5" : cela produira un hash MD5 du contenu du champ texte. Copiez-le.
3. Vous devez maintenant mettre ce hash dans votre base de données :
   1. Ouvrez votre base de données dans phpMyAdmin. Si vous ne savez pas comment accéder à phpMyAdmin, demandez à votre webmaster ou votre hébergeur.
   2. Ouvrez la table `pw_employee`, trouvez la table correspondant à votre compte (il doit contenir votre prénom, nom et adresse e-mail), et cliquez sur le bouton "Modifier".
   3. Trouvez le champ `passwd`, et copiez-y le hash MD5 que vous venez de générer.
4. Connectez-vous à votre back-office avec votre identifiant et votre nouveau mot de passe tel qu'utilisé ci-dessus (MONMOTDEPASSE ). Cela suffira à générer un nouvelle clé pour le cookie de votre navigateur.

Si cela ne marche toujours pas, utilisez phpMyAdmin pour accéder à la table `ps_shop_url` et vérifier la valeur de la boutique principale, dont l'`id` doit être 1. Elle doit contenir le chemin de la boutique. :

* Si votre boutique est à la racine du serveur, cette variable devrait contenir "`/`".
* Si votre boutique est dans un sous-dossier, la variable devrait y pointer. Par exemple, si votre boutique est à l'adresse "[http://www.mywebsite/shop/](http://www.mywebsite/shop/)", la variable devrait contenir "/shop/".

Si rien de tout cela ne marche, contactez le support de PrestaShop [http://support.prestashop.com/fr/](http://support.prestashop.com/fr/).

### PrestaShop ne m'envoie pas mon nouveau mot de passe <a href="#depannage-prestashopnemenvoiepasmonnouveaumotdepasse" id="depannage-prestashopnemenvoiepasmonnouveaumotdepasse"></a>

La demande de regénération du mot de passe ne fonctionne que si le serveur SMTP a bien été configuré, afin que PrestaShop puisse vous envoyez des e-mails.

Deux solutions se présentent à vous :

1. **Configurer votre serveur SMTP pour envoyer des e-mails :**\

   1. Renseignez-vous auprès de votre hébergeur afin d'obtenir vos informations de connexion SMTP.
   2. Ouvrez la page "E-mails" du menu "Paramètres avancés" de votre back-office (que ce soit vous ou un autre administrateur encore capable de se connecter).
   3. Sélectionnez l'option "Utiliser mes propres paramètres SMTP". Un formulaire apparaîtra : remplissez-le à l'aide des informations données par votre hébergeur.
   4. Enregistrez vos modifications.
   5. Refaites une demande de mot de passe. Vous devriez le recevoir.
2. **Suivez ces étapes** :
   1. Choisissez un nouveau mot de passe. Pour cet exemple, ce sera "\$$$lapin$159\$$$".
   2. À l'aide de votre client FTP, ouvrez le fichier `login.php` de votre installation de PrestaShop, situé dans le dossier d'administration en ligne (dont le nom dépend de votre installation).\
      En bas de ce fichier, ajoutez la ligne suivante :\
      &#x20;`echo md5( PSQL( _COOKIE_KEY_ . 'nouveaupassword' ) );`\
      Donc, avec notre mot de passe d'exemple :\
      &#x20;`echo md5( PSQL( _COOKIE_KEY_ . '$$$lapin$159$$$' ) );`\
      N'oubliez pas de mettre votre nouveau mot de passe !
3. Rendez-vous sur l'écran de connexion de votre back-office, comme si vous souhaitiez vous connecter, et copier le texte qui apparaît en bas de la page (par exemple, a0ee884b507dd4624ce51968cfbb19a9).
4. Rendez-vous dans la base de données de PrestaShop, par exemple à l'aide de phpMyAdmin. Dans la table `ps_employee`, remplacez la valeur existante de la colonne `passwd` de l'employé dont vous souhaitez changer le mot de passe, en y mettant la valeur obtenue à l'étape précédente. Enregistrez vos modifications.
5. Vous pouvez maintenant vous connecter avec l'identifiant et mot de passe.

### Se connecter après avoir effacé un pack de langue par erreur <a href="#depannage-seconnecterapresavoireffaceunpackdelangueparerreur" id="depannage-seconnecterapresavoireffaceunpackdelangueparerreur"></a>

Dans le cas où vous avez effacé un pack de langue de votre boutique, vous pourriez avoir des problèmes pour vous reconnecter à votre back-office.

Voici comment résoudre ce problème avec le français en langue par défaut :

1. Rendez-vous dans phpMyAdmin. Si vous ne pouvez pas y accéder, demandez à votre hébergeur de suivre ce processus pour vous.
2. Sélectionnez la base de données de votre boutique, et sélectionnez la table `ps_lang`.
3. Cliquez sur le bouton "Insérer" en haut de l'écran, et créez une nouvelle entrée avec ces valeurs :\

   * `id_lang` -> 1
   * `name` -> Français (France)
   * `active` -> 1
   * `iso_code` -> fr
   * `language_code` -> fr
   * `date_format_lite` -> Y-m-d
   * `date_format_full` -> Y-m-d H:i:s
   * `is_rtl` -> 0
4. Exécutez la requête.

Vous devriez pouvoir à nouveau vous connecter.
