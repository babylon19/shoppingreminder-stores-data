# ShoppingReminder — données de magasins

Liste de magasins de l'agglomération de Québec utilisée par l'application ShoppingReminder (`storesSeed.json`).

## Source et licence

- **Source :** © OpenStreetMap contributors — https://www.openstreetmap.org/copyright
- **Licence :** Open Database License (ODbL) 1.0 — https://opendatacommons.org/licenses/odbl/1-0/
- **Extraction :** requête Overpass (https://overpass-api.de) sur l'agglomération de Québec, filtrée par types de magasins
  (épicerie, pharmacie, animalerie, magasin à rabais, alcool, quincaillerie, club-entrepôt).

Ce fichier est une base de données dérivée d'OpenStreetMap. Toute réutilisation doit conserver la mention
« © OpenStreetMap contributors » et rester sous licence ODbL.

## Format

Tableau JSON. Chaque entrée : `place_id` (référence OSM), `name`, `store_type`, `latitude`, `longitude`, `address`,
`postal_code`, `city`, `country`.

## Fichiers par région (téléchargés par l'application)

L'application lit `manifest.json` puis télécharge à la demande le fichier de la région choisie (`Canada/CA-QC.json`, etc.).
`manifest.json` donne, pour chaque région, le nom, le nombre de magasins, la boîte englobante, la taille et l'empreinte
SHA-256 du fichier : l'application refuse tout fichier dont l'empreinte diffère. `manifest.json` et les fichiers doivent donc
toujours être publiés ensemble, depuis la même génération.

- **Extraction :** extraits OpenStreetMap de Geofabrik (https://download.geofabrik.de), classés par type de magasin.
- **Licence :** voir `ATTRIBUTION.md` (ODbL 1.0, © OpenStreetMap contributors).
- Même format d'entrée que `storesSeed.json`.
