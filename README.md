# Level 1 – Task 1: Data Collection & Web Scraping  
**Codveda Technologies – Data Science Internship**  
**Azangue Leonel Delmat** | 20/11/2025 | ID: CV/A1/48181  

## Objectif de la tâche (extrait officiel Codveda)
> **Description**: Collect data from a website using web scraping techniques.  
> - Identify a target website and inspect its structure  
> - Use BeautifulSoup and requests libraries to scrape data from web pages  
> - Store the scraped data in a structured format (CSV, JSON)  
> - Handle common challenges such as pagination and dynamic content  
> Tools: Python, BeautifulSoup, requests, pandas  

## Site cible choisi
**http://books.toscrape.com**  
→ Site d’entraînement public et 100 % légal pour le scraping  
→ 1000 livres répartis sur 50 pages → parfait pour tester la pagination  
→ Structure HTML très claire (pas de JavaScript lourd) → BeautifulSoup suffit  

## Méthodologie choisie & Justification

| Étape                     | Outil / Technique utilisée                     | Justification                                                                 |
|---------------------------|--------------------------------------------------|--------------------------------------------------------------------------------|
| 1. Inspection du site     | DevTools Chrome (Elements + Network)             | Comprendre rapidement la structure et les classes CSS utilisées              |
| 2. Requêtes HTTP          | `requests` + header User-Agent                   | Éviter d’être bloqué + simuler un vrai navigateur                            |
| 3. Parsing HTML           | `BeautifulSoup` (parser 'html.parser')           | Le plus simple, rapide et suffisant ici (pas de JS)                          |
| 4. Gestion de la pagination | Boucle sur 50 pages avec `page-{i}.html`        | Pagination statique → très fiable, pas besoin de Selenium                   |
| 5. Extraction des données  | Sélecteurs CSS précis (`article.product_pod`)    | Robuste même si le site évolue légèrement                                   |
| 6. Récupération catégorie | Une requête supplémentaire sur la page détail    | Nécessaire car catégorie non présente dans la liste → enrichissement données |
| 7. Politeness & Robustesse| `time.sleep(random 0.5-1.5s)` + `try/except`    | Respect du serveur + gestion des erreurs réseau                              |
| 8. Progression            | `tqdm`                                           | Visualisation claire pendant l’exécution (1000 livres → ~8 min)              |
| 9. Sauvegarde             | CSV + JSON via pandas                            | Deux formats demandés + facile à réutiliser pour les tâches suivantes       |

## Résultats obtenus
- **1000 livres** scrapés avec succès  
- Colonnes: `Title`, `Price (£)`, `Rating`, `In Stock`, `Category`, `URL`  
- Fichiers générés dans `/data`:
  - `books_dataset.csv` (1000 lignes)
  - `books_dataset.json`

## Structure de la branche