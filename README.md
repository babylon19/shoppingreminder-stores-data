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
