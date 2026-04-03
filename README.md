# 🏦 Projet d’Analyse des Transactions Bancaires

## 📌 Description

Ce projet consiste à analyser un dataset de transactions bancaires afin de :

* Comprendre la structure des données
* Nettoyer et préparer les données
* Détecter les valeurs aberrantes (anomalies)
* Produire des analyses statistiques et visuelles

L'objectif est d'améliorer la qualité des données et d’extraire des insights utiles pour la prise de décision.

---

## 📂 Dataset

Le dataset utilisé est :

* `bank.csv`

Il contient des informations sur les transactions bancaires telles que :

* Montant des transactions
* Score de crédit client
* Agence / région
* Statut des transactions

---

## ⚙️ Technologies utilisées

* Python 🐍
* Pandas (manipulation des données)
* NumPy (calculs numériques)
* Matplotlib & Seaborn (visualisation)

---

## 🔍 Étapes du projet

### 1. 📥 Importation des données

* Chargement du dataset avec `pandas`
* Affichage des premières lignes
* Vérification des dimensions et types de colonnes

### 2. 📊 Analyse exploratoire (EDA)

* Statistiques descriptives (`describe()`)
* Identification des variables numériques et catégorielles
* Analyse des distributions

### 3. 🧹 Nettoyage des données

* Traitement des valeurs manquantes :

  * Remplacement par la moyenne / médiane (numérique)
  * Remplacement par le mode (catégoriel)
* Correction des types de données

### 4. 🚨 Détection des anomalies

Deux méthodes utilisées :

#### ✔️ Méthode IQR (Interquartile Range)

* Détection des valeurs extrêmes
* Identification des transactions anormales

#### ✔️ Méthode Z-score

* Détection des valeurs très éloignées de la moyenne

👉 Une colonne `is_anomaly` peut être ajoutée pour marquer les anomalies.

---

## 📈 Visualisation

* Histogrammes des variables
* Boxplots pour détecter les outliers
* Graphiques de distribution

---

## 🧠 Décisions prises

* Conservation ou suppression des anomalies selon leur impact
* Remplacement des valeurs manquantes pour éviter la perte de données
* Ajout d’indicateurs pour suivre la qualité des données

---

## ▶️ Exécution du projet

1. Installer les dépendances :

```bash
pip install pandas matplotlib seaborn numpy
```

2. Lancer le notebook :

```bash
jupyter notebook projet_bank.ipynb
```

---

## 📊 Résultats attendus

* Dataset propre et exploitable
* Identification des transactions suspectes
* Meilleure compréhension des comportements financiers

---

## 🚀 Améliorations possibles

* Intégration d’un modèle de Machine Learning pour détecter les fraudes
* Création d’un dashboard interactif avec Streamlit
* Automatisation du pipeline de nettoyage

---

## 👤 Auteur

Projet réalisé par : **Nouhaila Sabbar**

---

## 📎 Remarque

Ce projet peut être intégré dans :

* un projet Data Science
* un système de détection de fraude bancaire
* un dashboard d’analyse financière

---
