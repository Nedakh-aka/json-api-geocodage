# JSON, API et géocodage

Projet réalisé dans le cadre de ma formation **Data Analyst à la Wild Code School**.

L'objectif est d'apprendre à manipuler des données JSON, interroger des API REST et exploiter des coordonnées géographiques avec Python.

## Contenu du projet

Le projet est organisé en trois challenges :

### Challenge 1 — Manipulation de JSON imbriqués
- Lecture et exploration de fichiers JSON.
- Normalisation des données avec `pandas.json_normalize()`.
- Calcul et comparaison de moyennes par restaurant et par évaluation.
- Agrégation des données par ville et par type de restaurant.

### Challenge 2 — Interrogation d'une API REST
- Interrogation de l'API Adresse française avec `requests`.
- Gestion des erreurs HTTP et des résultats manquants.
- Extraction des adresses, scores de correspondance et informations géographiques.
- Analyse de la pertinence des résultats dans un DataFrame.

### Challenge 3 — Géocodage et cartographie
- Géocodage de quatre restaurants de Catane avec Nominatim (OpenStreetMap).
- Respect des limites de requêtes du service.
- Création d'une carte interactive avec `folium`.
- Export des résultats géocodés au format CSV.

## Technologies utilisées

- **Python** : traitement des données et appels API.
- **Pandas** : normalisation et analyse des données.
- **Requests** : requêtes HTTP.
- **Folium** : visualisation cartographique.
- **Jupyter Notebook** : exécution et présentation des exercices.

## Structure du projet

```text
json-api-geocodage/
├── data/
│   ├── restaurants.json
│   ├── villes.json
│   └── restaurants_geocodes.csv
├── notebooks/
│   └── quete_json_api.ipynb
├── .gitignore
├── requirements.txt
└── README.md
```

## Installation

Cloner le dépôt :

```bash
git clone https://github.com/Nedakh-aka/json-api-geocodage.git
cd json-api-geocodage
```

Créer et activer un environnement virtuel :

```bash
python -m venv .venv
source .venv/Scripts/activate
```

*La commande d'activation ci-dessus correspond à Git Bash sous Windows.*

Installer les dépendances :

```bash
pip install -r requirements.txt
```

Ouvrir `notebooks/quete_json_api.ipynb` dans VS Code ou Jupyter.

## Résultat

Le projet produit un fichier CSV contenant les informations des restaurants et leurs coordonnées géographiques, ainsi qu'une carte interactive permettant de visualiser leur emplacement et leur note moyenne.

**Note :** le géocodage nécessite une connexion Internet. Les résultats enregistrés dans le CSV peuvent être réutilisés sans interroger à nouveau l'API.