# fake-project
# Prévision des Stocks avec des Séries Temporelles

## Description du projet/ The problem
Dans ce projet, l'objectif est de prévoir les niveaux de stock d'un produit à partir de données historiques. L'approche utilise des techniques d'analyse de séries temporelles pour prédire les besoins futurs en stock et aider à la gestion de l'approvisionnement.

# How does it work ?
## 1. Acquisition de données
Pour ce projet, les données de stock ont été obtenues à partir de **fichiers Excel** contenant des informations sur les ventes passées. Ces fichiers sont régulièrement mis à jour par l'équipe de gestion des stocks.

- **SQL** : Les données de vente peuvent également être extraites d'une base de données relationnelle à l'aide de requêtes SQL pour obtenir des informations supplémentaires sur les ventes.
- **Importation de fichiers Excel** : Les fichiers Excel sont importés dans le projet pour une analyse approfondie à l'aide de la bibliothèque `pandas` en Python.

## 2. Préparation des données
Les données de stock brutes ont nécessité un nettoyage et une transformation avant d'être prêtes pour l'analyse :

- **Nettoyage et manipulation des données** : 
  - Traitement des valeurs manquantes dans les colonnes des ventes.
  - Conversion des dates au format correct.
  - Gestion des valeurs aberrantes pour s'assurer que les prévisions ne sont pas faussées.
  
- **Techniques avancées** :
  - **Transformations** : Les données ont été ajustées pour s'assurer qu'elles étaient stationnaires, une condition importante pour l'analyse des séries temporelles.
  - **Machine learning** : Un modèle de régression a été utilisé pour détecter des tendances et des patterns dans les données. En complément, des modèles ARIMA (AutoRegressive Integrated Moving Average) ont été utilisés pour les prévisions.

## 3. Analyse des données
L'analyse des données a été réalisée en plusieurs étapes pour identifier les tendances et les modèles dans les séries temporelles :

- **Méthodes statistiques** : 
  - Calculs de moyennes mobiles et d'écart-type pour identifier les tendances à court et à long terme.
  - Application de tests statistiques pour déterminer si les séries temporelles sont stationnaires.
  
- **Régression** :
  - Un modèle de régression linéaire a été utilisé pour estimer les tendances de stock en fonction des ventes passées.
  
- **Analyse de séries temporelles** : 
  - Modèles ARIMA ont été employés pour prévoir les besoins futurs en stock en utilisant les ventes passées comme référence. Ces modèles ont permis d'obtenir des prévisions mensuelles du stock nécessaire.

## 4. Visualisation
Les résultats de l'analyse et des prévisions ont été visualisés à l'aide de plusieurs outils et techniques pour une meilleure compréhension des tendances et des besoins futurs :

<img width="1252" alt="Capture d’écran 2024-12-20 à 08 41 20" src="https://github.com/user-attachments/assets/63d0d60e-c80d-421c-874c-e070b040c6ba" />

- **Graphiques** :
  - Des graphiques de séries temporelles ont été générés pour illustrer les tendances historiques des niveaux de stock.
  - Des prévisions futures ont été affichées pour visualiser l'impact des tendances sur les besoins futurs en stock.

- **Tableaux de bord** :
  - Des **tableaux de bord interactifs** ont été créés avec **Streamlit** pour permettre aux utilisateurs de visualiser les prévisions de stock et d'interagir avec les données.
  - Des graphiques interactifs ont été réalisés avec **Matplotlib** pour afficher les tendances et ajuster les prévisions en fonction de différents paramètres.

## Technologies utilisées
- **Python** : Langage principal pour l'analyse des données.
- **Pandas** : Pour le nettoyage et la manipulation des données.
- **Statsmodels / ARIMA** : Pour les modèles de séries temporelles et les prévisions.
- **Matplotlib** : Pour la visualisation des données et des prévisions.
- **Streamlit** : Pour créer des tableaux de bord interactifs.

## Résultats et Conclusion
Les prévisions de stock réalisées grâce aux modèles ARIMA ont permis d'anticiper les besoins futurs en stock et d'optimiser la gestion des approvisionnements. Ce projet démontre l'importance de l'analyse des séries temporelles dans la gestion de la chaîne d'approvisionnement.

