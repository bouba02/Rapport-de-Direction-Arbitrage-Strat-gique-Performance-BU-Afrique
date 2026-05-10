# Revue de Direction Multi-Filiales — Arbitrage Stratégique BU Afrique | Power BI

> **Vrai client · Expert-comptable · Plusieurs filiales en Afrique · Livré en production**  
> 3 pages · Star Schema · Heatmap · Scatter · Radar · Analyse seuil de rentabilité

🇬🇧 [English version available here](README.md)

---

## Contexte Client

**Secteur :** Cabinet d'expertise comptable  
**Périmètre :** Plusieurs filiales opérant en Afrique — BU consolidée  
**Interlocuteur :** Expert-comptable — présentation en réunion de direction  
**Période :** Mars – Avril 2026  
**Statut :** Livré et utilisé en réunion de direction

> *Les données et visuels du dashboard ne sont pas partagés publiquement
> par respect de la confidentialité client. Ce dépôt documente l'architecture,
> la modélisation et la logique métier.*

---

## Problème Business

L'expert-comptable consolidait les données financières de plusieurs filiales
africaines dans un fichier Excel multi-onglets : illisible en réunion de direction,
aucune comparaison filiale-à-filiale possible, et aucune aide à la décision
pour les arbitrages 2026.

**La direction avait besoin de réponses claires à 4 questions stratégiques :**

| # | Question |
|---|---|
| 1 | **Où gagne-t-on de l'argent ?** |
| 2 | **Où perd-on du cash ?** |
| 3 | **Qui consomme la dette ?** |
| 4 | **Où faut-il arbitrer en 2026 ?** |

**Mission :** Transformer un fichier Excel consolidé multi-filiales en outil
d'arbitrage stratégique interactif, opérationnel dès la première réunion.

---

## Solution Livrée

### Restructuration du Modèle de Données

Transformation du fichier Excel consolidé en Star Schema Power BI :

```
Table de faits
└── FAITS_Financiers     → indicateurs financiers par filiale et période

Table de dimension
└── FILIALES_Dim         → caractéristiques et segmentation des filiales
```

![Modèle en étoile](schema.png)

Architecture optimisée pour le filtrage dynamique par filiale, région et période,
avec comparaison N vs N-1 sur tous les indicateurs.

### KPIs Développés

| Indicateur | Description |
|---|---|
| `CA` | Chiffre d'affaires par filiale et consolidé |
| `EBITDA` | Résultat avant intérêts, impôts, dotations |
| `Résultat Net` | Résultat final après toutes charges |
| `Marge Nette` | Résultat Net / CA — comparaison inter-filiales |
| `Taux de Recouvrement` | Créances recouvrées / CA — suivi liquidité |
| `Exposition Créances` | Encours clients N vs N-1 |
| `Seuil de Rentabilité` | CA minimum pour couvrir les charges fixes |
| `CA Absorbé en Charges Fixes` | % du CA consommé par les charges fixes |

---

## Dashboard — 3 Pages

### Page 1 — Vue Consolidée
KPIs globaux · Waterfall P&L (CA → Résultat Net) · Taux de recouvrement consolidé · Exposition créances N vs N-1

### Page 2 — Performance & Cash par Filiale
- **Heatmap multi-indicateurs** — lecture instantanée de la performance de chaque filiale
- **Scatter CA vs Marge Nette** — positionnement stratégique de chaque filiale
- **Analyse des charges** — graphique à barres exposition créances et CA absorbé
- **Matrice de risque** — classement des filiales par niveau de risque opérationnel

### Page 3 — Arbitrage 2026
- **Radar stratégique** — comparaison multi-dimensionnelle des filiales
- **Analyse seuil de rentabilité vs CA réel** — identification des filiales sous le seuil
- Réponses directes aux 4 questions stratégiques de la direction

---

## Insights Extraits

| Insight | Détail |
|---|---|
| Rentabilité concentrée | Seulement 2 filiales sur le périmètre sont réellement rentables |
| Risque opérationnel critique | Une filiale absorbe **67%** de son CA en charges fixes — revue urgente du modèle |
| Croissance sans trésorerie | Une filiale affiche **+227% de croissance** mais un taux de recouvrement de seulement **62%** |

---

## Impact Métier

| Résultat | Détail |
|---|---|
| Outil opérationnel immédiat | Utilisé dès la première réunion de direction |
| Arbitrages objectivés | Décisions 2026 basées sur des données, pas sur des impressions |
| Lecture inter-filiales | Comparaison directe rendue possible pour la première fois |
| Documentation complète | Toutes les règles de calcul documentées pour une utilisation reproductible |

---

## Stack Technique

- **Power BI Desktop** — développement du rapport
- **DAX** — mesures calculées, comparaisons N vs N-1, seuils dynamiques
- **Power Query / M** — restructuration du fichier Excel consolidé multi-filiales
- **Excel** — source de données consolidée
- **Star Schema** — modélisation dimensionnelle

### Visualisations Avancées
- Waterfall P&L
- Heatmap multi-indicateurs par filiale
- Scatter plot CA vs Marge Nette
- Radar stratégique multi-axes
- Matrice de risque dynamique
- Analyse seuil de rentabilité

---

## Documentation

| Document | Contenu |
|---|---|
| [DAX_MEASURES.md](DAX_MEASURES.md) | Code des mesures DAX et règles de calcul |
| [METHODOLOGY.md](METHODOLOGY.md) | Architecture, restructuration Excel, choix de modélisation |
| [schema.png](schema.png) | Schéma du modèle de données |

---

## Structure du Repository

```
expert-comptable-africa-bu/
├── README.md                  # Version anglaise
├── README_FR.md               # Ce fichier
├── schema.png
└── pbix/
    └── (non partagé — données client confidentielles)
```

---

## Auteur

**Boubacar Nikiema** — Data Analyst & Consultant BI

Spécialisé en dashboards financiers, reporting de gestion et pilotage stratégique
avec Power BI, SQL, Python et Excel. Basé au Maroc, j'interviens auprès
d'entreprises en Afrique et en Europe francophone.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-boubacar--nikiema-blue?logo=linkedin)](https://linkedin.com/in/boubacar-nikiema)
[![YouTube](https://img.shields.io/badge/YouTube-BoubacarDataAnalyst-red?logo=youtube)](https://youtube.com/@BoubacarDataAnalyst)
[![Email](https://img.shields.io/badge/Email-nikiemaboubacar%40gmail.com-gray?logo=gmail)](mailto:nikiemaboubacar@gmail.com)
[![Portfolio](https://img.shields.io/badge/Portfolio-data.ngroupmediadigital.com-green)](https://data.ngroupmediadigital.com)

---

*Mission client réelle · Données confidentielles non partagées · Code : MIT License*
