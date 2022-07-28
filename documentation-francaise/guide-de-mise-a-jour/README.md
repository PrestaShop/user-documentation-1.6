# Guide de mise à jour

**Contenu**

* [Guide de mise à jour](./#Guidedemiseàjour-Guidedemiseàjour)
  * [Support PrestaShop](./#Guidedemiseàjour-SupportPrestaShop)
  * [Vérifier les prérequis pour la nouvelle version](./#Guidedemiseàjour-Vérifierlesprérequispourlanouvelleversion)
  * [Mettre à jour depuis une version antérieure à la 1.4](./#Guidedemiseàjour-Mettreàjourdepuisuneversionantérieureàla1.4)

## Guide de mise à jour <a href="#guidedemiseajour-guidedemiseajour" id="guidedemiseajour-guidedemiseajour"></a>

De nouvelles versions de PrestaShop sortent régulièrement. Certaines sont importantes, d'autres mineurs, mais toutes apportent leur lot d'innovations, d'améliorations et de corrections. Il est donc fortement conseillé de régulièrement mettre votre installation à jour.

Vous avez deux possibilités pour mettre à jour :

* [Mise à jour automatique](mise-a-jour-automatique.md).
* [Mise à jour manuelle](mise-a-jour-manuelle.md).

La mise à jour automatique utilise simplement le module gratuit [1-Click Upgrade](http://addons.prestashop.com/fr/outils-administration-modules-prestashop/5496-1-click-upgrade-autoupgrade.html).

La mise à jour manuelle est aujourd'hui déconseillée, mais nous conservons sa documentation pour des raisons historiques – et pour les utilisateurs qui ne peuvent pas utiliser la mise à jour automatique.

Le processus de mise à jour touche à tous les fichiers et dossiers de votre installation de PrestaShop. Cela comprend tous les fichiers fondamentaux de PrestaShop, tous les modules par défaut et le thème par défaut. Si vous avez modifié ces fichiers, vos modifications seront perdues.

Bien faite, la mise à jour décrite dans ces pages ne devrait pas prendre plus d'une demi-heure. Ne passez pas une étape dans le seul but de gagner du temps, car toutes sont cruciales.

* [Mise à jour automatique](mise-a-jour-automatique.md)
* [Mise à jour manuelle](mise-a-jour-manuelle.md)
* [Faire une sauvegarde et la restaurer](faire-une-sauvegarde-et-la-restaurer.md)
* [En cas de problème](en-cas-de-probleme.md)

### Support PrestaShop <a href="#guidedemiseajour-supportprestashop" id="guidedemiseajour-supportprestashop"></a>

Pour toute **demande de support** ou **d'aide à la mise en place de votre site**, contactez-nous et découvrez nos offres.

* Par e-mail : utilisez le formulaire de contact à l'adresse [https://www.prestashop.com/fr/support](https://www.prestashop.com/fr/support)
* Par téléphone ([de 9h00 à 18h00, heure de Paris](http://www.timeanddate.com/worldclock/france/paris)):
  * 01 40 18 30 04 si vous avez besoin de conseils sur PrestaShop (gratuit)
  * 08 90 03 23 20 si vous avez des questions sur l'utilisation de notre solution (0.80€ / min)
* Découvrez nos offres de support : [http://addons.prestashop.com/fr/388-support](http://addons.prestashop.com/fr/388-support)
* Et bien entendu, le formidable forum d'entraide communautaire : [http://www.prestashop.com/forums/](http://www.prestashop.com/forums/)

### Vérifier les prérequis pour la nouvelle version <a href="#guidedemiseajour-verifierlesprerequispourlanouvelleversion" id="guidedemiseajour-verifierlesprerequispourlanouvelleversion"></a>

Avant de vous lancer dans l'installation de la dernière version de PrestaShop, vérifiez bien que la configuration de votre serveur correspond ou dépasse les prérequis minimaux pour cette version, qui sont indiqués sur cette page : [http://www.prestashop.com/fr/configuration-requise](http://www.prestashop.com/fr/configuration-requise).

Par exemple, assurez-vous que votre hébergeur vous propose effectivement les versions nécessaires de PHP et MySQL. Le cas échéant, demandez-lui de mettre à jour la configuration du serveur. Si ne connaissez pas les versions de PHP et MySQL que vous utilisez, demandez-les-lui.

S'il se trouve que votre hébergeur ne veut ou ne peut pas mettre à niveau votre configuration serveur, il est sans doute temps de trouver un meilleur hébergeur. Ne vous lancez PAS dans une mise à jour à moins de disposer au moins des versions minimales requises.

### Mettre à jour depuis une version antérieure à la 1.4 <a href="#guidedemiseajour-mettreajourdepuisuneversionanterieureala1.4" id="guidedemiseajour-mettreajourdepuisuneversionanterieureala1.4"></a>

Les anciennes versions de PrestaShop ne sont pas aussi simple à mettre que les dernières versions : le code y est très différent, de nombreux fichiers ont été déplacés, d'autres ont été créés et certains ont été supprimés. De fait, le risque est grand de voir s'afficher nombre d'erreurs si le saut de version est trop brutal.

Vous êtes par ailleurs limité à la mise à jour manuelle : le module de mise à jour automatique ne fonctionne qu'à partir de la version 1.4 de PrestaShop.

Vous devriez de fait faire d'autant plus attention à chaque étape de la mise à jour. Plus la version est ancienne, plus les détails sont importants : sauvegardes, fichiers personnalisés, thème modifié, etc.
