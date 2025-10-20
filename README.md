# 🌐 Projet Cloud – Analyse du Risque de Crédit avec Azure et Power BI

## 📘 Description du projet
Ce projet a pour objectif de **concevoir un pipeline analytique complet** pour l’analyse du risque de crédit, en combinant les outils **Python, Azure et Power BI**.  
Il s’inscrit dans le cadre du module *Cloud Computing et Data Management*, et démontre la capacité à intégrer un **flux de données de bout en bout**, depuis la préparation locale jusqu’à la visualisation interactive dans le cloud.

---

## 🎯 Objectif
> Mettre en place un pipeline simple permettant **d’explorer, stocker et visualiser** des données à grande échelle via **Azure Blob Storage**, **Azure SQL Database**, et **Power BI**.

Le dataset étudié provient de la fusion de deux sources :
- **UCI Credit Card Dataset**
- **Credit Risk Dataset** (Kaggle)

Ces données ont été préalablement **nettoyées et enrichies dans Alteryx**, puis intégrées et visualisées dans un environnement Cloud Azure.

---

## 🧱 Architecture du projet

```text
Python (Notebook)
    │
    ├── Préparation & Nettoyage du Dataset
    │       └── pandas, numpy
    │
    ├── Envoi vers Azure Blob Storage
    │       └── azure-storage-blob SDK
    │
    ├── Chargement dans Azure SQL Database
    │       └── Azure Data Factory (ADF)
    │
    └── Visualisation interactive
            └── Power BI connecté à Azure SQL
