# Analyse des Genres sur Wikipedia

## Description

Ce projet vise à analyser la répartition et l'évolution des contributions sur Wikipedia en fonction du genre des contributeurs (hommes, femmes, personnes transgenres). Wikipedia, en tant que plateforme ouverte, aspire à représenter la société dans sa diversité. Cependant, des différences notables persistent dans la participation en fonction du genre et des dimensions spatio-temporelles. Ce projet cherche à comprendre ces écarts, en explorant les contributions des utilisateurs selon le genre, la localisation géographique et les sujets modifiés. L'objectif est de révéler les tendances dans les contributions à Wikipedia à travers différentes langues et régions.

Pour atteindre cet objectif, le projet utilise des bibliothèques Python telles que **wikipedia-api** pour accéder aux informations des contributeurs, **Pandas** pour structurer et analyser les données, **Requests** pour les appels à l'API Wikipedia, et **Re** pour extraire des informations à partir du contenu des pages.

## Fonctionnalités

- **Collecte des Données** : Utilisation de l'API Wikipedia pour récupérer les informations des contributeurs par genre à partir de catégories spécifiques telles que "Female Wikipedians", "Male Wikipedians" et "Transgender Wikipedians".
- **Extraction de la Localisation** : Extraction des informations de localisation à partir des pages utilisateur de Wikipedia en utilisant des expressions régulières pour détecter les mentions géographiques.
- **Analyse des Contributions** : Collecte des contributions des utilisateurs par genre, langue, et région, pour évaluer la participation de chaque genre sur Wikipedia.
- **Visualisation des Résultats** : Les données collectées sont agrégées et visualisées pour comprendre les tendances en matière de participation et de localisation des contributeurs.

## Prérequis

- Python 3.x
- Bibliothèques Python : wikipedia-api, Pandas, Requests, Re

## Installation et Lancement

1. Clonez ce dépôt sur votre machine locale :
   ```sh
   git clone <URL-du-dépôt>
   ```
2. Accédez au dossier du projet :
   ```sh
   cd chemin/vers/le/projet
   ```
3. Installez les dépendances requises :
   ```sh
   pip install -r requirements.txt
   ```
4. Exécutez le script principal pour lancer la collecte des données et l'analyse :
   ```sh
   python gender_analysis_wikipedia.py
   ```

## Objectifs du Projet

1. **Création d'une Collection de Données** : Collecter des données à partir de Wikipedia concernant les contributeurs par genre, localisation, et langue.
2. **Prétraitement des Données** : Identifier et structurer les aspects tels que le genre, la localisation, les sujets et les langues.
3. **Agrégation des Données** : Analyser les données collectées en fonction des dimensions identifiées (genre, localisation, sujets).
4. **Visualisation des Résultats** : Fournir une représentation visuelle des contributions par genre, localisation, et sujets modifiés.

## Structure du Projet

- **gender_analysis_wikipedia.py** : Script principal pour la collecte et l'analyse des données Wikipedia.
- **wikipedia_contributions_with_geography5.csv** : Fichier CSV généré contenant les contributions avec les informations de localisation et de genre.
- **requirements.txt** : Liste des bibliothèques nécessaires pour exécuter le projet.

## Collaborateurs

- Arafat Feical Idriss
- Ismael Sow

## Licence

Ce projet est sous licence MIT. Voir le fichier `LICENSE` pour plus de détails.

