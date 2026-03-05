#  Traitement des Données Manquantes par Régression Linéaire (From Scratch)

## Description
Ce projet implémente manuellement la régression linéaire multiple via la formule 
analytique pour imputer des valeurs manquantes dans un jeu de données salarial.
Aucune bibliothèque ML n'est utilisée — uniquement NumPy pour les calculs matriciels.

## Auteure
**Chaymae YASSINE**

## Structure du projet
missing-data-regression/
│
├── regression_from_scratch.ipynb    # Notebook principal
├── README.md                        # Documentation du projet
└── images/                          # Graphiques générés
    ├── experience_vs_salaire.png
    └── age_vs_salaire.png

## Instructions d'exécution
1. Cloner le repo ou télécharger le fichier `.ipynb`
2. Ouvrir dans Jupyter Notebook ou Google Colab
3. Exécuter toutes les cellules dans l'ordre

## Contexte et Problématique
Un jeu de données de 50 personnes contient des salaires manquants (8 valeurs sur 50).
L'objectif est d'imputer ces valeurs manquantes en utilisant une régression linéaire 
implémentée from scratch, sans bibliothèques ML.

## Méthodologie
### 1. Génération et exploration des données
- Création d'un dataset de 50 personnes (âge, expérience, salaire)
- Suppression aléatoire de 8 valeurs de salaire
- Analyse des valeurs manquantes (nombre et pourcentage)

### 2. Implémentation de la régression linéaire (from scratch)
- Séparation des données complètes (train) et incomplètes (test)
- Implémentation manuelle via la formule analytique :

$$\beta = (X^T X)^{-1} X^T y$$

- Aucune bibliothèque ML utilisée — uniquement NumPy

### 3. Imputation des valeurs manquantes
- Prédiction des salaires manquants avec les coefficients calculés
- Remplacement des valeurs manquantes par les prédictions
- Vérification de l'absence de valeurs manquantes après imputation

### 4. Visualisation des résultats
- Droite de régression : Expérience vs Salaire
- Droite de régression : Âge vs Salaire
- Équation finale affichée : Salaire = β₀ + β₁ × Âge + β₂ × Expérience

## Résultats
- 8 valeurs manquantes imputées avec succès
- 0 valeurs manquantes restantes après imputation
- Relation positive entre expérience/âge et salaire confirmée visuellement

## Limites
- Jeu de données simulé (pas de données réelles)
- Taille réduite (50 observations)
- Absence de métriques d'évaluation (RMSE, MAE, R²)
- Relation supposée linéaire entre les variables

##  Technologies
Python · NumPy · Pandas · Matplotlib
