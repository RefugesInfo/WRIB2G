## Application FirefoxOS de www.refuges.info

### Comment lancer cette application

Cette application utilise des requêtes AJAX entre hôtes (ce qui est bloqué par les navigateurs), voici les solutions qui s'ofrent à vous pour l'utiliser :

 * Utiliser la version hébergée sur le serveur refuges.info/mobile
 * Sur Firefox, installez [ForceCORS](https://addons.mozilla.org/fr/firefox/addon/forcecors) et activez-le (dans la barre des modules)
 * Sur FirefoxOS, assurez-vous d'avoir installé la version officielle **prochainement** disponible dans MarketPlace

### Modifications faites pour héberger cette application sur refuges.info

Voici une liste des modifications effectuées quand on héberge cette application sur le serveur de WRI :

 * Renommer `js/index.js.online` en `js/index.js`
 * Renommer `online.htaccess` en `.htaccess`
 * Renommer `manifest.webapp.online` en `manifest.webapp`

*Le dossier dans lequel doit se trouver l'application doit être http://HOST/mobile/ ou il faut changer le `manifest.webapp`*