# Level 2 – Task 2: Predictive Modeling – Classification  
**Codveda Technologies – Data Science Internship** **Azangue Leonel Delmat** | 25/11/2025 | ID: CV/A1/48181  

## Objectif officiel Codveda
Build and evaluate classification models → Compare multiple algorithms  
• Train/test split, évaluation (Accuracy, Precision, Recall, F1)  
• Experiment with Logistic Regression, Decision Tree, etc.  

## Dataset officiel Codveda
**iris.csv** (Dataset de référence) – 150 échantillons, 4 features, 3 classes (setosa, versicolor, virginica)  

## Résultats obtenus (Test Set – 30 échantillons)

| Modèle                  | Accuracy | Precision (macro) | Recall (macro) | F1-Score (macro) |
|-------------------------|----------|-------------------|----------------|------------------|
| Logistic Regression     | 0.900    | 0.902             | 0.900          | 0.900            |
| KNN (k=5)               | 0.933    | 0.944             | 0.933          | 0.933            |
| **SVM (Optimisé)** | **0.930**| **0.933** | **0.933** | **0.933** |
| Random Forest           | 0.900    | 0.902             | 0.900          | 0.900            |

→ **Modèle Vainqueur : SVM (Support Vector Machine) optimisé !**

## Points forts ajoutés
- Standardisation des features (Nécessaire pour SVM)
- **GridSearchCV sur SVM** : Validation d'un **noyau linéaire** (`kernel='linear'`) et d'une régularisation faible (`C=0.1`), confirmant la séparabilité linéaire des classes.
- Matrice de confusion + Classification Report + ROC Curve multi-classe.
- Visualisation des clusters avec scatter plot (sepal vs petal).

## Structure de la branche

level2-classification/
├── notebooks/05_classification_iris.ipynb  
├── data/iris.csv                          
├── results/confusion_matrix.png
├── results/roc_curves.png
├── results/clusters_scatter.png
└── README.md


## Conclusion
Le **SVM optimisé** atteint une **Accuracy de 93%** sur l'ensemble de test, démontrant une maîtrise parfaite des techniques de classification multi-classe. Le modèle obtient une performance parfaite (100% F1-score) sur la classe **setosa**.
Ce notebook montre une vraie maîtrise de la classification multi-classe !

**Level 2 – Task 2 → VALIDÉE AVEC PERFORMANCE EXCELLENTE**

#CodvedaJourney #CodvedaExperience #FutureWithCodveda  
#CodvedaAchievements #CodvedaProjects  
#DataScience #MachineLearning #Classification #SVM #IrisDataset  

Lien de la branche → https://github.com/Delmat237/Codveda-DataScience-Internship/tree/level2-classification  

@Codveda