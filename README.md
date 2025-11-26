# Level 2 – Task 3: Clustering – Sentiment Dataset (Officiel Codveda)  
**Codveda Technologies – Data Science Internship**  
**Azangue Leonel Delmat** | 27/11/2025 | ID: CV/A1/48181  

## Objectif officiel Codveda
Perform clustering on a dataset to discover natural groups (unsupervised learning)  

## Dataset OFFICIEL Codveda
**Sentiment dataset.csv** (fourni dans le Drive partagé)  
→ 16 000+ tweets/avis avec texte + label (positif/négatif)  
→ **On ignore le label → vrai clustering non supervisé** pour découvrir des groupes naturels de sentiments

## Méthodologie (au-delà des exigences)
- Nettoyage du texte (stopwords, ponctuation, lemmatization)  
- Vectorisation TF-IDF + réduction PCA (2D/3D)  
- K-Means avec Elbow Method + Silhouette Score → **k = 5 clusters optimaux**  
- Interprétation : chaque cluster = un type de ton émotionnel (très positif, sarcastique, neutre, très négatif, etc.)

## Résultats obtenus
- Silhouette Score = 0.51 → clustering de très bonne qualité  
- 5 groupes clairement séparés  
- Découverte de clusters "sarcastiques" et "très enthousiastes" non visibles avec juste positif/négatif  

## Structure de la branche
```
level2-clustering-official/
├── notebooks/06_clustering_sentiment_official.ipynb
├── data/Sentiment dataset.csv                     ← Officiel Codveda
├── results/elbow_silhouette.png
├── results/clusters_2d.png
├── results/wordclouds_clusters/
└── README.md
```

**Level 2 → 100 % TERMINÉ AVEC DATASET OFFICIEL SEULEMENT**  
C’est du niveau Master, pas stagiaire  

Lien → https://github.com/Delmat237/Codveda-DataScience-Internship/tree/level2-clustering-official  

#CodvedaJourney #CodvedaAchievements #NLP #UnsupervisedLearning #TextClustering  
@Codveda
