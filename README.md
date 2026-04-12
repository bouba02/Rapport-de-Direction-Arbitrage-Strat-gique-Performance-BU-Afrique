# 📊 Rapport de Direction : Arbitrage Stratégique & Performance BU Afrique
[![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](https://powerbi.microsoft.com)
[![Excel](https://img.shields.io/badge/Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)](https://www.microsoft.com/excel)
[![DAX](https://img.shields.io/badge/DAX-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)](https://dax.guide)
[![Licence](https://img.shields.io/badge/Licence-MIT-green?style=for-the-badge)](LICENSE)

## 🎯 Objectif du Projet
Ce projet consiste en la création d'un outil d'aide à la décision conçu spécifiquement pour un **expert-comptable**. L'objectif est de transformer ses données financières brutes consolidées en un rapport de synthèse interactif pour ses réunions de direction, permettant de répondre à 4 questions stratégiques majeures :

1.  **Où gagne-t-on de l’argent ?** 
2.  **Où perd-t-on du cash ?**
3.  **Qui consomme la dette ?** 
4.  **Où faut-il arbitrer en 2026 ?** 

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
3.  **Page 1 — Vue Consolidée :** KPIs globaux, Waterfall (CA → Résultat Net) et indicateurs de recouvrement.
4.  **Page 2 — Performance & Cash :** Heatmap des indicateurs clés, Graphique à barre des charges, des exposition créances et CA absorbé et matrice de risque par filiale.
5.  **Page 3 — Arbitrage 2026 :** Analyse des seuils de rentabilité vs CA réel pour les recommandations stratégiques, et réponses aux 4 questions principales.
6.  **Export & Documentation :** Guide d'utilisation et spécifications des mesures DAX.

---

## 💡 Insights Stratégiques Extraits
* **Rentabilité :** Nous avons repéré que seulement 2 filiales qui sont rentables du groupe.
* **Risque Opérationnel :** Ainsi une filiale nécessite une revue urgente du modèle car elle absorbe **67%** de son CA en charges fixes.
* **Trésorerie :** Une autre filiale présente une croissance de **+227%** mais un taux de recouvrement critique de seulement **62%**.

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
