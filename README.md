# 📊 Analyse de l'évolution du profil sociodémographique des étudiants Data OpenClassrooms avec Snowflake & dbt

## 🎯 Objectif

Construire un pipeline analytique moderne permettant d'intégrer, transformer et analyser les données sociodémographiques des étudiants Data OpenClassrooms, puis les comparer aux statistiques nationales de l'INSEE.

## 📌 Contexte

Projet réalisé dans le cadre de la formation **Data Analyst OpenClassrooms**.

L'objectif est de mettre en œuvre une architecture analytique reposant sur **Snowflake** et **dbt** afin de produire des indicateurs fiables sur les profils des étudiants Data OpenClassrooms entre 2022 et 2025.

## ❓ Problématique

Comment exploiter les données internes OpenClassrooms et les données publiques de l'INSEE afin de mieux comprendre le profil des apprenants et identifier les opportunités de développement de l'offre de formation ?

## 📂 Sources de données

### Données OpenClassrooms

* 4 010 étudiants Data
* Période : 2022 à 2025
* Genre
* Région
* Tranche d'âge
* Parcours

### Données INSEE

* Population active française
* Répartition régionale
* Répartition par âge
* Répartition par genre

## 🏗️ Architecture du projet

Le pipeline suit une architecture **Modern Data Stack** :

```text
Sources
    ↓
Staging
    ↓
Intermediate
    ↓
Marts
    ↓
Export & Visualisation
```

### Sources

* Données OpenClassrooms
* Données INSEE

### Staging

* Nettoyage des données
* Déduplication
* Contrôle qualité
* Normalisation des variables

### Intermediate

* Agrégation des étudiants
* Harmonisation des régions
* Standardisation des segments démographiques

### Marts

* Création des tables analytiques finales
* Jointure OpenClassrooms + INSEE
* Calcul des indicateurs métier

## 🔍 Contrôle qualité

Mise en place de tests dbt :

* not_null
* unique
* accepted_values

Plus de 40 tests automatisés ont été exécutés pour garantir la qualité des données.

## 📊 Analyses réalisées

### Profil des étudiants OpenClassrooms

* Répartition par genre
* Répartition par région
* Répartition par tranche d'âge
* Évolution des effectifs

### Comparaison avec la population nationale

* Analyse des écarts hommes/femmes
* Analyse territoriale
* Analyse démographique
* Identification des segments sous-représentés

## 📈 Principaux résultats

### Profil type de l'étudiant Data OpenClassrooms

* Homme
* Âgé de 30 à 34 ans
* Résidant principalement en Île-de-France

### Évolution des effectifs

* Baisse des effectifs entre 2022 et 2024
* Reprise observée en 2025

### Répartition géographique

* Forte concentration en Île-de-France
* Plusieurs régions restent sous-représentées

### Diversité

* Progression de la part des femmes entre 2022 et 2025
* Parité encore non atteinte

## 💡 Recommandations

* Renforcer le recrutement en régions
* Développer les actions en faveur de la diversité
* Attirer davantage de profils en formation initiale
* Poursuivre l'exploitation des données démographiques pour adapter l'offre de formation

## 🧰 Technologies utilisées

* Snowflake
* dbt Cloud
* SQL
* CSV
* Data Modeling
* Data Quality Testing

## 📁 Structure du projet

```text
models/
│
├── staging/
├── intermediate/
├── marts/

tests/
│
├── schema.yml

data/
│
├── social.csv
├── insee_pop.csv

exports/
│
├── mart_final_export.csv

README.md
```

## ✅ Compétences développées

* SQL avancé
* Snowflake
* dbt
* Data Modeling
* Data Quality
* Data Warehouse
* ETL / ELT
* Analyse sociodémographique
* Storytelling de données
* Gouvernance des données

## 🔒 RGPD

* Données pseudonymisées
* Aucun nom ou email conservé
* Agrégation des données avant restitution
* Respect des principes de minimisation des données

## 👨‍💻 Auteur

**Mohamed Zaidi**
