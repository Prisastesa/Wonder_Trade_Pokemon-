#  Projet Wonder Trade : Analyse de la Générosité des Échanges Pokémon

##  Contexte Académique
Ce projet est réalisé dans le cadre de la **L2 MIASHS** (Mathématiques et Informatique Appliquées aux Sciences Humaines et Sociales) à l'Université Montpellier Paul Valéry. Il valide les compétences de deux Unités d'Enseignement (UE) :
* **Bases de Données (BD)** : Modélisation, requêtage SQL complexe et gestion de base de données.
* **Science des Données 2 (SD)** : Analyse statistique, inférence et modélisation sous R.


##  Problématique
**"Les caractéristiques des Pokémon et des dresseurs influencent-ils la qualité des échanges au sein du système Wonder Trade ?"**

Nous cherchons à déterminer si ce système de troc est utilisé comme un espace de partage généreux ou comme un "vide-ordures" pour Pokémon indésirables, en analysant l'impact de l'identité des dresseurs sur la valeur des Pokémon envoyés.


##  Méthodologie Statistique & Technique

###  Analyse de Données (Inférence)
Contrairement à une analyse basée uniquement sur des moyennes (qui masquent la réalité des extrêmes), ce projet privilégie l'étude des **distributions** :
* **Étude des Distributions** : Utilisation de Boxplots et de densités pour observer la dispersion des niveaux et des statistiques de combat.
* **Test du Khi-deux ($\chi^2$)** : Analyse de la dépendance entre variables qualitatives (ex: Genre du dresseur vs Type de Pokémon).
* **ANOVA** : Comparaison des distributions de variables numériques entre plusieurs groupes (ex: Niveau moyen par pays d'origine).
* **Corrélation de Pearson** : Mesure de la force du lien entre la difficulté de capture et la fréquence d'échange.
* **Régression Linéaire** : Modélisation prédictive pour estimer la "valeur" d'un Pokémon en fonction de ses caractéristiques techniques.
* **Clustering K-means (Optionnel)** : Identification de profils types d'échanges (Pokémon "poubelles" vs Pokémon "stratégiques").

###  Architecture des Données
* **Base de données** : MySQL (phpMyAdmin).
* **Requêtage** : Utilisation requetes avancé.

---

##  Équipe & Répartition des Rôles
Le projet est géré sous une organisation GitHub. La répartition suit un modèle **Responsable (Lead) / Co-responsable (Support)** pour assurer une collaboration fluide sur tous les aspects du projet.

| Membre | Rôle Principal (Lead) | Support (Co-responsable) |
| :--- | :--- | :--- |
| **Sara** (@SaraFenina) | **Git Master** & Régression Linéaire | Architecture BD (MCD/MOD) |
| **Stéphanie** (@Stephanie-goat) | Import/Prétraitement & **ANOVA** | Mise en forme RMarkdown & Slides |
| **Prisca** (@ambinintsoaprisca) | SQL Avancé & **ggplot2** (Distributions) | Clustering (K-means) |
| **Sarah** (@Sarhaivie) | Tests Stat (**Khi-2 / Corrélation**) | Analyse métier des requêtes |

---

##  Structure du Répertoire
* `/data` : Données brutes et traitées (CSV).
* `/sql` : Scripts de création des tables et requêtes d'analyse.
* `.Rmd` contenant le code de l'analyse statistique et les graphiques.
* `/docs` : Rapport final PDF et support de présentation (Slides).

---
