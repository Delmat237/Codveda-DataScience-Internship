# Level 1 – Task 2: Data Cleaning & Preprocessing  
**Codveda Technologies – Data Science Internship**  
**Azangue Leonel Delmat** | 21/11/2025 | ID: CV/A1/48181  

## Objectif officiel Codveda
> Clean and preprocess a raw dataset to make it suitable for analysis.  
> - Handle missing data (imputation, removal)  
> - Detect and remove outliers  
> - Convert categorical variables (one-hot / label encoding)  
> - Normalize or standardize numerical data  

## Dataset utilisé
**books_dataset.csv** – 1000 livres scrapés hier (Task 1)  
→ Dataset brut réaliste avec vrais problèmes (prix **manquants** simulés, outliers de prix, catégories à encoder, etc.)

## Méthodologie & Justification

| Étape                        | Technique choisie                              | Justification                                                       |
|-----------------------------|-------------------------------------------------|----------------------------------------------------------------------|
| 1. Chargement & overview    | `pandas` + `df.info()`, `df.describe()`         | Identifier rapidement les types et les problèmes                     |
| 2. Valeurs manquantes       | Imputation médiane pour le prix<br>Mode pour catégorie | Prix = numérique → médiane robuste<br>Catégorie = catégorielle      |
| 3. Outliers                 | IQR method (1.5 × IQR) sur le prix              | Méthode standard et robuste aux distributions asymétriques          |
| 4. Encodage catégoriel      | One-Hot Encoding sur `Category`                 | Pas d’ordre naturel → One-Hot est le choix le plus sûr               |
| 5. Rating → numérique       | Déjà numérique (1-5) → rien à faire             | —                                                                    |
| 6. Normalisation            | StandardScaler sur les variables numériques     | Prépare le dataset pour les modèles ML demain (Level 2)              |
| 7. Sauvegarde               | `books_cleaned.csv` + `books_cleaned.pkl`       | Deux formats : lisible + rapide à charger                            |

## Résultats avant/après
| Métrique                  | Avant nettoyage       | Après nettoyage       |
|---------------------------|-----------------------|-----------------------|
| Lignes totales            | 1000                  | 968 (32 outliers supprimés) |
| Valeurs manquantes        | 87 (prix)             | 0                     |
| Catégories uniques        | 49                    | 49 (one-hot → 49 colonnes) |
| Prix max                  | £54.99 → £99.99 (outliers) | £57.20             |

## Structure de la branche
```
level1-data-cleaning/
├── notebooks/02_data_cleaning_books.ipynb   ← Notebook complet + commentaires
├── data/books_dataset.csv                   ← brut (issu Task 1)
├── data/books_cleaned.csv                   ← version finale nettoyée
├── data/books_cleaned.pkl                   ← pour chargement rapide
└── README.md                                ← ce fichier
```

## Prochaines étapes
Ce dataset ultra-propre sera utilisé demain pour **Level 1 Task 3: Exploratory Data Analysis**

#CodvedaJourney #CodvedaExperience #FutureWithCodveda  
#CodvedaAchievements #CodvedaProjects  
#DataScience #DataCleaning #Python #Pandas  

Lien de la branche → https://github.com/Delmat237/Codveda-DataScience-Internship/tree/level1-data-cleaning  

@Codveda
