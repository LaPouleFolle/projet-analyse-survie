# Analyse de survie : durée de maintien au pouvoir des dirigeants politiques

## Présentation du projet

Dans le cadre de mon projet d'analyse de survie, je m'intéresse à la durée de maintien au pouvoir des dirigeants politiques et aux facteurs qui accélèrent leur chute. 

J'ai choisi d'adopter une approche en deux temps :
1. **Une analyse globale** sur l'ensemble des dirigeants de ma base de données afin de poser le contexte général.
2. **Un focus sur l'Afrique depuis les indépendances**, pour identifier plus précisément les déterminants qui accélèrent la sortie irrégulière du pouvoir sur le continent.

## Données utilisées

* **`h_data.csv`** : base globale recensant les mandats de dirigeants politiques (dates d'entrée et de sortie, durée du mandat en années, type de fonction exercée, mode d'accession au pouvoir, motif de départ et indicatrice de chute irrégulière).
* **Base Afrique** *(à venir)* : jeu de données complémentaire dédié au focus sur les dirigeants africains.

## Méthodologie

Pour mener cette étude sur des données censurées à droite, je mets en œuvre les méthodes vues en cours :
* Nettoyage des données et calcul du taux de censure ;
* Estimation non-paramétrique de la fonction de survie (**Kaplan-Meier**) ;
* Comparaison de groupes (**test du log-rank**) ;
* Modélisation multivariée (**modèle à risques proportionnels de Cox**) ;
* Ouverture vers les **risques concurrents** (départ irrégulier vs départ régulier ou décès naturel).

## Outils et organisation du dépôt

Je réalise l'ensemble de ce travail sous **R** via **RStudio sur Onyxia**, en rédigeant mon rapport au format **Quarto (`.qmd`)** compilé en **PDF**.

* `data/` : jeux de données bruts
* `rapport_survie.qmd` : fichier source contenant mon analyse et mes scripts R
* `README.md` : présentation du projet
