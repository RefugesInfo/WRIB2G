## Application FirefoxOS de www.refuges.info

### Comment lancer cette application

Cette application utilise des requêtes AJAX entre hôtes (ce qui est bloqué par les navigateurs), voici les solutions qui s'ofrent à vous pour l'utiliser :

 * Utiliser la version hébergée sur le serveur [refuges.info/mobile](http://leo.refuges.info/mobile/)
 * Sur Firefox, installez [ForceCORS](https://addons.mozilla.org/fr/firefox/addon/forcecors) et activez-le (dans la barre des modules), puis [téléchargez l'application](https://github.com/OpenSourceWay/WRIB2G/archive/master.zip), décompressez le dossier et ouvrez index.html avec Firefox.
 * Sur Firefox, Firefox OS, Tablettes ou smartphones android, assurez-vous d'avoir installé la version officielle **prochainement** disponible dans [MarketPlace](https://marketplace.firefox.com/app/refuges/)

### Modifications faites pour héberger cette application sur refuges.info

Voici une liste des modifications effectuées quand on héberge cette application sur le serveur de WRI :

 * Renommer `js/index.js.online` en `js/index.js` (changement des liens)
 * Renommer `online.htaccess` en `.htaccess` (ajout du bon content-type)
 * Renommer `manifest.webapp.online` en `manifest.webapp` (passage de host en packaged)

*Le dossier dans lequel doit se trouver l'application doit être http://HOST/mobile/ ou il faut changer le `manifest.webapp`*

### À faire (propsez vous aussi !) :

 * Remplacer les liens vers d'autres points bbcode pour utiliser `displayPoint()`
 * Gérer les préférences utilisateur via un cookies (fond de carte)
 * Ajouter un support permalink avec une ancre vers un id de point pour afficher directement un point

### Contenu du innerHTML non complilé :

    <a class="retour" href="#" onclick="displayBlock('carte');">Retour carte</a>
    <span id="titrePoint"></span>
    <div id="fichePoint"><span id="idPoint"></span><span id="typePoint"></span></div>
    <p id="coordPoint"></p>
    <p id="proprioPoint"></p>
    <p id="accesPoint"></p>
    <p id="rmqPoint"></p>
    <p id="infoscompPoint"><b>Informations complémentaires :</b><br />
    	<span id="couverturePoint"></span>
    	<span id="eauPoint"></span>
    	<span id="boisPoint"></span>
    	<span id="latrinePoint"></span>
    	<span id="manquemurPoint"></span>
    	<span id="poelePoint"></span>
    	<span id="chemineePoint"></span>
    	<span id="clefPoint"></span>
    	<span id="matelasPoint"></span>
    	<span id="ravitaillementeauPoint"></span>
    	<span id="sitewebPoint"></span></p>
    <p id="pointsprochesPoint"><b>Points proches :</b><br />
    	<span id="pp0Point"></span>
    	<span id="pp1Point"></span>
    	<span id="pp2Point"></span></p>
    <div id="commentairesPoint"><p><b>Commentaires :</b></p>
    	<div id="com0Point"></div>
    	<div id="com1Point"></div>
    	<div id="com2Point"></div>
    	<div id="com3Point"></div>
    	<div id="com4Point"></div></div>
    <p class="sautdeligne"></p>