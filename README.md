# Level 1 – Task 3: Exploratory Data Analysis (EDA)  
**Codveda Technologies – Data Science Internship**  
**Azangue Leonel Delmat** | 22/11/2025 | ID: CV/A1/48181  

## Objectif officiel Codveda
> Perform exploratory data analysis to understand the underlying structure and trends in the data.  
> - Visualize the data using histograms, scatter plots, box plots  
> - Compute summary statistics  
> - Identify correlations (correlation matrix)  
> - Generate a report summarizing insights  

## Dataset utilisé
`books_cleaned.csv` → 968 livres nettoyés (issu des tâches 1 & 2)

## Insights majeurs découverts (spoiler du notebook)
- Prix moyen : £29.4 | Médiane : £25.9 → distribution asymétrique  
- 49 catégories → mais 5 catégories représentent 58 % des livres  
- Note moyenne : 3.88/5 → les clients sont plutôt généreux  
- Corrélation forte : livres les plus chers = meilleure note moyenne  
- Les livres “In Stock” ont un prix moyen +12 % plus élevé  
- Top 5 catégories les plus chères : Poetry, Romance, Travel, Classics, Science  

## Visualisations générées
- Distribution des prix (histogram + boxplot)  
- Top 15 catégories par nombre de livres  
- Prix moyen par note (1 à 5)  
- Matrice de corrélation + heatmap  
- Wordcloud des titres les plus fréquents  

## Structure de la branche
```
level1-eda/
├── notebooks/03_eda_books.ipynb           ← Notebook complet + rapport intégré
├── data/books_cleaned.csv                 ← dataset nettoyé
├── results/                               ← 8 graphiques sauvegardés
│   ├── price_distribution.png
│   ├── top_categories.png
│   └── correlation_heatmap.png
└── README.md                              ← ce fichier
```

## Conclusion du rapport
Le dataset est maintenant parfaitement compris.  
Les insights extraits seront directement utilisables pour des modèles de recommandation ou de prédiction de prix demain en Level 2.

**Level 1 complet (3/3) terminé avec mention excellente !**



#CodvedaJourney #CodvedaExperience #FutureWithCodveda  

#CodvedaAchievements #CodvedaProjects  

#DataScience #EDA #Python #Seaborn #Matplotlib  



Lien de la branche → https://github.com/Delmat237/Codveda-DataScience-Internship/tree/level1-eda  



@Codveda
