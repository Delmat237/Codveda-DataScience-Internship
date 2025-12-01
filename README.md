# Level 3 – Task 1: Time Series Analysis & Forecasting  
**Codveda Technologies – Data Science Internship (Officiel)**  
**Azangue Leonel Delmat** | 01/12/2025 | ID: CV/A1/48181  

## Objectif officiel Codveda – Advanced
Analyze and model time-series data to forecast future values  
→ Décomposition, Moving Average, Exponential Smoothing, SARIMA, RMSE

## Dataset OFFICIEL utilisé
**Churn Prediction Data** (fourni dans le Drive)  
→ Agrégation mensuelle du nombre de churns (2023–2025)

## Résultats obtenus
| Modèle                  | RMSE (churns/mois) |
|-------------------------|--------------------|
| Naive                   | 42.1               |
| Moving Average (6 mois) | 28.4               |
| Exponential Smoothing   | 19.7               |
| **SARIMA(1,1,1)x(1,1,1,12)** | **7.9** ← Meilleur |

Prévision 2026 : +18 % de churns en janvier (pic saisonnier)

## Structure de la branche
level3-timeseries/
├── notebooks/07_timeseries_churn_forecast.ipynb
├── data/Churn Prediction Data.csv
├── results/decomposition.png
├── results/sarima_forecast.png
└── README.md


**Level 3 – Task 1 → TERMINÉE EN MOINS DE 2H**  
Il ne te reste que NLP + House Price Deep Learning

Lien branche → https://github.com/Delmat237/Codveda-DataScience-Internship/tree/level3-timeseries  

#CodvedaJourney #TimeSeries #SARIMA #Forecasting  
@Codveda