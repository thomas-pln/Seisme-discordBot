# Seisme-DiscordBot
Bot discord proposant d'afficher les événements sismiques dans une région donné avec des coordonnées.


## Fichiers :
* app.js -> code du bot
* config.json -> fichier de configuration (requis), modifiable directement sur discord (recommandé ✔) ou directement sur le fichier (⚠)
* ./data/data.json -> contient les événements de la requête précédente (requis),
en cas de problème remplacer tout le contenu par:
```json
{"features":[],"type":"FeatureCollection"}
```

* Ajouter un fichier `.env` tel que :
```
TOKEN = [token Discord]
USERNAME = [username geoNames]
```

## Librairies requises :
* discord.js: 13.1.0 (minimum) -> ``nmp install discord.js``
* request -> ``nmp install request``
* dotenv -> ``nmp install dotenv``



Pour lister les commandes disponibles : ``!quake help``

Les données proviennent de la BDD de http://www.franceseisme.fr/

Autres liens :
* https://api.franceseisme.fr/fdsnws/event/1/ (base de l'API)
* https://renass.unistra.fr/
* http://www.geonames.org/
