# @etalab/decoupage-administratif

Données concernant le découpage administratif français, au format JSON.

- Communes
- Arrondissements
- Départements
- Régions
- EPCI (à fiscalité propre)

## Installation

```bash
# npm
npm install @etalab/decoupage-administratif

# yarn
yarn add @etalab/decoupage-administratif
```

## Utilisation

### Node

```js
const communes = require('@etalab/decoupage-administratif/data/communes.json')
const departements = require('@etalab/decoupage-administratif/data/departements.json')
const regions = require('@etalab/decoupage-administratif/data/regions.json')
const arrondissements = require('@etalab/decoupage-administratif/data/arrondissements.json')
const epci = require('@etalab/decoupage-administratif/data/epci.json')
```

### via des URLs

Pour la dernière version

- Communes https://unpkg.com/@etalab/decoupage-administratif/data/communes.json
- Départements https://unpkg.com/@etalab/decoupage-administratif/data/departements.json
- Régions https://unpkg.com/@etalab/decoupage-administratif/data/regions.json
- Arrondissements https://unpkg.com/@etalab/decoupage-administratif/data/arrondissements.json
- EPCI https://unpkg.com/@etalab/decoupage-administratif/data/epci.json

Il est possible de rajouter une version. Pour les EPCI 2021, par exemple https://unpkg.com/@etalab/decoupage-administratif@1.1.1/data/epci.json (voir le lien millésime et version de packages)

## Millésimes et versions de package

Vous avez besoin de données selon une année? Voici un tableau récapitulatif pour choisir:

| Année | Version du package                        | NPM                                               | Yarn                                               |
|-------|-------------------------------------------|---------------------------------------------------|----------------------------------------------------|
| 2022  | 2.2.0                                     | `npm install @etalab/decoupage-administratif@2.2.0` | `yarn install @etalab/decoupage-administratif@2.2.0` |
| 2021  | 1.1.1                                     | `npm install @etalab/decoupage-administratif@1.1.1` | `yarn install @etalab/decoupage-administratif@1.1.1` |
| 2020  | Non disponible, sauf EPCI 2020 avec 0.8.0 | `npm install @etalab/decoupage-administratif@0.8`   | `yarn install @etalab/decoupage-administratif@0.8`   |
| 2019  | 0.7                                       | `npm install @etalab/decoupage-administratif@0.7`   | `yarn install @etalab/decoupage-administratif@0.7`   |

## Sources

* [Code Officiel Géographique](https://insee.fr/fr/information/2560452) de l'INSEE
* [Liste des EPCI à fiscalité propre](https://www.collectivites-locales.gouv.fr/institutions/liste-et-composition-des-epci-fiscalite-propre) de la DGCL ([url exacte](https://www.collectivites-locales.gouv.fr/files/Accueil/DESL/2022/epcicom2022.xlsx))
* [Population légale](https://www.insee.fr/fr/statistiques/6011070?sommaire=6011075) de l'INSEE + [population Mayotte INSEE 2017](https://www.insee.fr/fr/statistiques/3291775?sommaire=2120838)
* [Liste des codes postaux](https://www.data.gouv.fr/fr/datasets/base-officielle-des-codes-postaux/) issue des données La Poste. Antérieurement, sous licence ODBL, maintenant en LO
* [Correspondances communes code SIREN et code INSEE](https://www.banatic.interieur.gouv.fr/V5/fichiers-en-telechargement/fichiers-telech.php) Menu gauche "Table de correspondance code SIREN / Code Insee des communes" ([url exacte](https://www.banatic.interieur.gouv.fr/V5/ressources/documents/document_reference/TableCorrespondanceSirenInsee.zip))

## Licence

Données : [Licence Ouverte](https://www.etalab.gouv.fr/licence-ouverte-open-licence)\
Code : MIT
