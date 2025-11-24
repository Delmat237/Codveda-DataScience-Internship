# Level 2 – Task 1: Predictive Modeling – Regression  
**Codveda Technologies – Data Science Internship** 
**Azangue Leonel Delmat** | 23/11/2025 | ID: CV/A1/48181  

## Objectif officiel Codveda
Build and evaluate a regression model to predict a continuous variable (e.g., house prices)  
• Train several models + compare performance  
• Evaluate using MSE, RMSE, R²  
• Experiment with multiple algorithms  

## Dataset utilisé (Corrigé)
**Boston Housing Prices** (506 échantillons, 14 colonnes, data/4) house Prediction Data Set.csv)  
Target → MEDV (valeur médiane des maisons)

## Résultats obtenus (Meilleur score : Gradient Boosting)
| Modèle (Final) | RMSE | MAE | R² |
|----------------------------|---------|------|--------------|
| Linear Regression | 4.9286 | 3.1891 | 0.6688 |
| Decision Tree | 3.2274 | 2.3941 | 0.8580 |
| Random Forest | 2.9172 | 2.0413 | 0.8840 |
| **Gradient Boosting Optimisé** | **2.4918** | **1.9122** | **0.9153** |
| Random Forest Optimisé | 2.9172 | 2.0413 | 0.8840 |

---

## Points forts ajoutés (au-delà des exigences)
- **Identification et correction** des erreurs de chargement de fichier (pas d'en-tête, séparateur d'espaces).
- **Gradient Boosting** identifié et optimisé comme le **meilleur modèle** de loin ($R^2 = 0.9153$).
- **GridSearchCV** sur Gradient Boosting pour valider la robustesse des paramètres.
- Visualisation Prediction vs Actual + Feature Importance pour le **meilleur modèle (GB)**.
- Tout reproductible (random_state=42).

## Structure de la branche
```
level2-regression/
├── notebooks/04_regression_california_housing.ipynb
├── data/ house Prediction Data Set.csv
├── results/feature_importance.png
├── results/prediction_vs_actual.png
└── README.md
```

**Level 2 commence en force – Random Forest R² = 0.835 garanti**

Lien branche → https://github.com/Delmat237/Codveda-DataScience-Internship/tree/level2-regression  

#CodvedaJourney #CodvedaAchievements #MachineLearning #Regression  
@Codveda
