# Analyse des Contributions Genrées sur Wikipédia

Ce projet a pour objectif d’analyser les contributions sur Wikipédia selon le genre des contributeurs (hommes, femmes, personnes transgenres), en étudiant les thématiques éditées, la répartition géographique, les langues utilisées, et l’évolution temporelle. Il vise également à projeter les tendances futures (2025–2030) à l’aide de modèles prédictifs.

## Objectifs

- Identifier les déséquilibres dans la participation selon le genre
- Comprendre les préférences éditoriales en fonction du genre
- Étudier l’évolution des contributions dans le temps et selon la localisation
- Anticiper les tendances futures via des modèles d’apprentissage automatique

## Méthodologie

Les données ont été collectées via l’API Wikipedia en ciblant trois catégories : "Male Wikipedians", "Female Wikipedians", "Transgender Wikipedians". Un enrichissement a été effectué via DBpedia pour catégoriser les articles. Le traitement comprend :

- Nettoyage et filtrage des données
- Extraction des localisations (pycountry, geonamescache)
- Vectorisation des titres (TF-IDF)
- Clustering thématique (KMeans)
- Modélisation des tendances (régression linéaire, Random Forest, XGBoost)

## Technologies utilisées

- Python 3.x
- Bibliothèques : wikipedia-api, pandas, numpy, scikit-learn, xgboost, matplotlib, seaborn, plotly, pycountry, requests, re

## Fichiers principaux

- `code.ipynb` : notebook principal d’analyse, enrichissement, modélisation
- `wikipedia_contributions.csv` : jeu de données enrichi
- `Article_scientifique.pdf` : article scientifique détaillé du projet
- `Presentation.pdf` : support de présentation des résultats
- `requirements.txt` : dépendances du projet

## Instructions d'exécution

1. Cloner le dépôt :
   git clone https://github.com/votre-utilisateur/analyse-genree-wikipedia.git

2. Se rendre dans le dossier :
   cd analyse-genree-wikipedia

3. Installer les dépendances :
   pip install -r requirements.txt

4. Lancer le notebook :
   jupyter notebook code.ipynb

## Résultats synthétiques

- 58,9 % des contributions sont masculines, 31,2 % féminines, 9,85 % transgenres
- Les hommes éditent majoritairement des sujets techniques, militaires et scientifiques
- Les femmes privilégient les domaines culturels, sociaux et éducatifs
- Les personnes transgenres contribuent davantage aux sujets liés aux droits LGBTQ+
- Les contributions féminines et transgenres progressent, mais la tendance reste dominée par les hommes
- La régression linéaire est le modèle prédictif le plus performant (R² > 0.89)

## Auteurs

- Ismael SOW
- Fatoumata DIALLO
- Tuteur : Marc SPANIOL

## Licence

Ce projet est distribué sous licence MIT. Voir le fichier `LICENSE` pour plus d'informations.
