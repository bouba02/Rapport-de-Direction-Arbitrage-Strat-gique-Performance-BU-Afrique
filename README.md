# 📊 Rapport de Direction : Arbitrage Stratégique & Performance BU Afrique
[![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](https://powerbi.microsoft.com)
[![Excel](https://img.shields.io/badge/Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)](https://www.microsoft.com/excel)
[![DAX](https://img.shields.io/badge/DAX-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)](https://dax.guide)
[![Licence](https://img.shields.io/badge/Licence-MIT-green?style=for-the-badge)](LICENSE)

## 🎯 Objectif du Projet
Ce projet consiste en la création d'un outil d'aide à la décision conçu spécifiquement pour un **expert-comptable**. L'objectif est de transformer ses données financières brutes consolidées en un rapport de synthèse interactif pour ses réunions de direction, permettant de répondre à 4 questions stratégiques majeures :

1.  [cite_start]**Où gagne-t-on de l’argent ?** [cite: 241, 242]
2.  [cite_start]**Où perd-t-on du cash ?** [cite: 238]
3.  [cite_start]**Qui consomme la dette ?** [cite: 234]
4.  [cite_start]**Où faut-il arbitrer en 2026 ?** [cite: 231]

---

## 🏗️ Architecture du Modèle de Données
Le projet repose sur une restructuration complète des données comptables en un **Modèle en Étoile (Star Schema)**. Cette architecture garantit une performance optimale des calculs DAX et une flexibilité totale pour le filtrage par filiale ou région.

### Visualisation du Modèle :
![Modèle en Étoile Power BI](schema.png)

> **Note technique :** Le modèle sépare clairement les données de faits (`FAITS_Financiers`) des dimensions contextuelles (`FILIALES_Dim`).

---

## 🛠️ Plan de Réalisation Étape par Étape

1.  **Préparation des données :** Restructuration du fichier Excel consolidé en table plate exploitable.
2.  **Maquettage UI/UX :** Création d'un prototype haute fidélité aux couleurs corporate.
3.  [cite_start]**Page 1 — Vue Consolidée :** KPIs globaux, Waterfall (CA → Résultat Net) et indicateurs de recouvrement[cite: 21, 55].
4.  [cite_start]**Page 2 — Performance & Cash :** Heatmap des indicateurs clés, Graphique à barre des charges, des exposition créances et CA absorbé et matrice de risque par filiale[cite: 161, 162].
5.  [cite_start]**Page 3 — Arbitrage 2026 :** Analyse des seuils de rentabilité vs CA réel pour les recommandations stratégiques, et réponses aux 4 questions principales.[cite: 189, 190, 231].
6.  **Export & Documentation :** Guide d'utilisation et spécifications des mesures DAX.

---

## 💡 Insights Stratégiques Extraits
* [cite_start]**Rentabilité :** Nous avons repéré que seulement 2 filiales qui sont rentables du groupe[cite: 243].
* [cite_start]**Risque Opérationnel :** Ainsi une filiale nécessite une revue urgente du modèle car elle absorbe **67%** de son CA en charges fixes[cite: 231, 238].
* [cite_start]**Trésorerie :** Une autre filiale présente une croissance de **+227%** mais un taux de recouvrement critique de seulement **62%**[cite: 239].

---
## 🛠️ Outils & technologies

- Power BI  
- Power Query (M)  
- DAX  
- Excel (source de données) 



---

## 👤 Auteur

**Boubacar Nikiema**  
Data Analyst | Consultant BI  

📧 nikiemaboubacar@gmail.com  
📱 +212 676 86 1686  

---

## 🤝 Me contacter

Vous souhaitez :

- Automatiser votre reporting financier  
- Mettre en place un pilotage par la donnée  
- Transformer vos données en levier stratégique  

👉 N’hésitez pas à me contacter.
