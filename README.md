```markdown
# TP_Musée — Base de Données (PostgreSQL) 🏛️📊  
**Modélisation • Implémentation • Analyse de données**

---

## 🎯 Présentation du projet

Ce projet **TP_Musée** est une étude complète de conception et d’exploitation d’une base de données relationnelle dédiée à la gestion d’activités culturelles d’un musée.  

Il met en œuvre l’ensemble du cycle d’un projet de données :

> **Analyse → Modélisation → Implémentation → Intégration des données → Requêtes analytiques**

Ce travail démontre des compétences clés en :

- Modélisation de données (MCD / MER)  
- Conception de bases relationnelles  
- Manipulation avancée de SQL  
- Nettoyage et structuration de données (CSV → PostgreSQL)  
- Analyse par requêtes (jointures, agrégations, vues analytiques)

---

## 📁 Contenu du dépôt

```

TP_musee/
│
├── Create_Tables.sql      # Création du schéma PostgreSQL
├── Requêtes.sql           # Requêtes analytiques et métiers
├── Rapport projet BDD.odt # Analyse et modélisation du projet
│
├── accessibilite.csv
├── agenda.csv
├── avoir.csv
├── correspondre.csv
├── derouler.csv
├── evenement.csv
├── lien.csv
├── lieu.csv
├── territoire.csv
│
└── README.md

````

---

## 🧠 Problématique métier

Le musée souhaite :

- organiser ses **événements culturels**,  
- gérer les **lieux et territoires**,  
- suivre l’**accessibilité**,  
- analyser la fréquentation et la programmation,  
- relier événements, lieux et thématiques de façon structurée.

La base permet notamment de répondre à des questions telles que :

- Quels événements ont lieu dans tel territoire ?  
- Quels lieux sont accessibles aux personnes à mobilité réduite ?  
- Quels types d’événements sont les plus fréquents ?  
- Quels liens existent entre événements et lieux ?

---

## 🛠️ Compétences mises en œuvre

### ✔️ Modélisation de données  
- Identification des entités (événement, lieu, territoire, agenda, accessibilité…)  
- Définition des relations (1-N, N-N)  
- Normalisation des tables  

### ✔️ Implémentation PostgreSQL  
- Création de tables avec clés primaires et étrangères  
- Contraintes d’intégrité  
- Indexation et relations  

### ✔️ Intégration des données  
- Importation de fichiers CSV dans PostgreSQL  
- Structuration et nettoyage des données  

### ✔️ Analyse SQL  
Exemples de types de requêtes réalisées :

- Jointures multiples  
- Agrégations (`COUNT`, `GROUP BY`)  
- Filtres avancés  
- Requêtes analytiques pour décision  

---

## 🚀 Installation et utilisation

### Prérequis  
- PostgreSQL installé  
- pgAdmin ou psql  

### Étapes

1. Cloner le projet :

```bash
git clone https://github.com/kossi-ctrl/TP_musee.git
cd TP_musee
````

2. Créer la base et charger le schéma :

```sql
CREATE DATABASE tp_musee;
\c tp_musee;
\i Create_Tables.sql;
```

3. Importer les CSV dans PostgreSQL :

```sql
COPY lieu FROM 'lieu.csv' DELIMITER ';' CSV HEADER;
COPY evenement FROM 'evenement.csv' DELIMITER ';' CSV HEADER;
-- etc.
```

4. Exécuter les requêtes dans `Requêtes.sql` pour analyser les données.

---

## 🧰 Technologies utilisées

* **PostgreSQL**
* **SQL avancé**
* **Modélisation MER / UML**
* **CSV**
* **Git & GitHub**

---

## 👤 Auteur

**Kossi-Ctrl**
📍 Étudiant / Analyste de données en formation
🔗 [https://github.com/kossi-ctrl](https://github.com/kossi-ctrl)

---

## 📌 À propos (Portfolio)

Ce projet illustre ma capacité à :

* comprendre un problème métier,
* le traduire en modèle de données,
* construire une base robuste,
* et produire des analyses pertinentes via SQL.

Il constitue une pièce centrale de mon portfolio en **Data Engineering & Analyse de données**.

---

## 📜 Licence  

Projet réalisé dans le cadre du  
👉 [Centre d’Études Supérieures de la Renaissance — Université de Tours](https://www.cesr.tours.fr)

© Novembre 2025 — Daniel, Thamra & Kossi  

Sous licence :  
👉 **[Creative Commons CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.fr)**


```
```
