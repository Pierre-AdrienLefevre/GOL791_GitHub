# Analyse des Routes et Visualisation

Ce projet se concentre sur l'analyse et la visualisation des données de routes, en utilisant des bibliothèques telles que `pandas`, `folium`, et `matplotlib`. Il vient du Amazon Last Mile Routing Challenge (2021).
Il est destiné au cours GOL791 à l'Ecole de Techologie Superieure, Montréal, Canada.

## Contenu

- `route_data.parquet` : Contient les données des routes.
- `actual_sequences.parquet` : Contient les séquences réelles des arrêts.
- `Analyse_Exploratoire.ipynb` : Le notebook Jupyter contenant le code pour charger, traiter, analyser les données, et créer des visualisations.

## Bibliothèques Utilisées

- `pandas` : Pour la manipulation des données.
- `folium` : Pour la création de cartes interactives.
- `matplotlib` : Pour la création de graphiques.
- `seaborn` : Pour la visualisation des données.
- `osmnx` : Pour l'analyse et la visualisation des réseaux de transport.
- `shapely` : Pour la manipulation des géométries.
- `pyarrow` : Pour lire les fichiers parquet.

## Instructions d'Installation

1. Clonez le dépôt :
    ```sh
    git clone https://github.com/votre-utilisateur/votre-repo.git
    cd votre-repo
    ```

2. Installez les dépendances :
    ```sh
    pip install pandas folium matplotlib seaborn osmnx shapely
    ```

3. Exécutez le notebook :
    ```sh
    jupyter notebook main.ipynb
    ```

## Exemple d'Utilisation

### Chargement et Affichage des Données

```python
import pandas as pd

route_data_df = pd.read_csv(r"DataBase/route_data.csv")
actual_sequences_df = pd.read_csv(r"DataBase/actual_sequences.csv")

print(route_data_df.head())
print(actual_sequences_df.head())
