# 📊 Marketing Campaign Analysis — Customer Data (EDA + Statistical Tests + Power BI)

Analyse exploratoire des données (EDA), tests statistiques et dashboard Power BI sur un dataset de campagnes marketing clients.

## 📁 Structure du projet

```
.
├── notebooks/
│   └── customer_campaign_analysis.ipynb   # EDA + tests statistiques (Python)
├── powerbi/
│   └── campagnes_marketing.pbix            # Dashboard Power BI
├── data/
│   └── (dataset CSV — à ajouter, voir section Données)
├── requirements.txt
└── README.md
```

## 🧠 Contenu du projet

### Étape 1 — Analyse Exploratoire des Données (Python)
- Chargement et exploration du dataset (`shape`, `info`, `describe`)
- Détection des doublons et valeurs manquantes
- Identification des variables continues / discrètes
- Création d'une variable `Total_Spending` (somme des dépenses par catégorie)
- Visualisations : distribution des achats web/magasin, boxplots, histogrammes
- Analyse par pays : revenu moyen, dépenses moyennes
- Relation Income ↔ Total_Spending (scatterplot)

### Étape 2 — Tests Statistiques
- **T-test** : comparaison des dépenses moyennes selon la réponse à la campagne (H0/H1)
- **Chi² d'indépendance** : relation entre le pays et l'acceptation d'une campagne
- **Corrélation de Pearson** : lien entre revenu et dépenses totales
- Matrice de corrélation (heatmap) sur toutes les variables numériques

### Power BI
- Dashboard interactif (`campagnes_marketing.pbix`) sur les campagnes marketing

## 📦 Données

Le notebook utilise un fichier `data-69d3709338fdb705334215.csv` qui n'est pas inclus dans ce repo (souvent trop volumineux ou confidentiel pour GitHub).
➡️ Placez votre CSV dans le dossier `data/` et adaptez le chemin dans la première cellule du notebook si besoin.

## ⚙️ Installation

```bash
git clone https://github.com/<votre-user>/<nom-du-repo>.git
cd <nom-du-repo>
pip install -r requirements.txt
jupyter notebook notebooks/customer_campaign_analysis.ipynb
```

## 🛠️ Technologies

- Python (pandas, seaborn, matplotlib, scipy)
- Jupyter Notebook
- Power BI

## 👤 Auteur

Dahani

## 📄 Licence

Ce projet est fourni à des fins éducatives / portfolio.
