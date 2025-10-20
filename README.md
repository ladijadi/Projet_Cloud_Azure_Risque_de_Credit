# 🌐 Projet Cloud – Analyse du Risque de Crédit avec Azure et Power BI

## 📘 Description du projet
Ce projet a pour objectif de **concevoir un pipeline analytique complet** pour l’analyse du risque de crédit, en combinant les outils **Python, Azure et Power BI**.  
Il s’inscrit dans le cadre du module *Cloud Computing et Data Management*, et démontre la capacité à intégrer un **flux de données de bout en bout**, depuis la préparation locale jusqu’à la visualisation interactive dans le cloud.

---

## 🎯 Objectif
> Mettre en place un pipeline simple permettant **d’explorer, stocker et visualiser** des données à grande échelle via **Azure Blob Storage**, **Azure SQL Database**, et **Power BI**.

Le dataset étudié provient de la fusion de deux sources :
- **UCI Credit Card Dataset** (Kaggle)
- **Credit Risk Dataset** (Kaggle)

Ces données ont été préalablement **nettoyées et enrichies dans Alteryx**, puis intégrées et visualisées dans un environnement Cloud Azure.
---
## ☁️ Étapes principales

### 🔹 Nettoyage et exploration des données dans un notebook Python
- Gestion des valeurs manquantes, des outliers et enrichissement des variables  
- Analyse descriptive et visualisations avec **matplotlib** et **seaborn**

### 🔹 Stockage cloud
- Export du dataset nettoyé vers **Azure Blob Storage**

### 🔹 Chargement dans Azure SQL Database
- Configuration du pipeline avec **Azure Data Factory**

### 🔹 Connexion Power BI → Azure SQL
- Importation de la table **`Dataset_Risque_de_Credit_Clean`**  
- Création de visuels interactifs et d’indicateurs de performance (**KPI**)

---

## 📊 Résultats
- **Dataset final :** `Dataset_Risque_de_Credit_Clean` *(10M lignes, 26 colonnes)*  
- **Tableau de bord Power BI :** indicateurs de risque (score paiement, taux de défaut, endettement, etc.)  
- **Visualisations interactives :** par tranche d’âge, revenu, montant de prêt et statut de paiement

---

## 📎 Auteur
👩‍💻 **Khady DIAGNE**  
Master 2 – Science des Données  
Université de Lorraine – IDMC  
🔗 [LinkedIn](https://www.linkedin.com/in/khadydiagne/)

## 🧱 Architecture du projet

```text
Python (Notebook)
    │
    ├── Préparation & Nettoyage du Dataset
    │       └── pandas, numpy, seaborn, Matplotlib
    │
    ├── Envoi vers Azure Blob Storage
    │       └── azure-storage-blob SDK
    │
    ├── Chargement dans Azure SQL Database
    │       └── Azure Data Factory (ADF)
    │
    └── Visualisation interactive
            └── Power BI connecté à Azure SQL


