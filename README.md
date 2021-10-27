# README #

Dépôt du cours [swirl](https://swirlstats.com/) de l'ENSTBB

Ce cours n'a pas pour objectif d'apprendre la statistiques, il se focalise sur l'apprentissage de l'utilisation de R/RStudio, de son fonctionnement et de ses mécanismes programmatique.

L'objectif est de comprendre comment R fonctionne pour pouvoir l'utiliser correctement/efficacement/intelligement pour faire de la statistiques.

Cours traduit et adapté du cours [R_programming_E](https://github.com/swirldev/R_Programming_E) lui-même issu du MOOC Coursera **R-programming** de l'équipe biostatistics du *John Hopkins School of Public Health*.

Un grand merci à eux pour le travail accompli et la publication en open-source.

# Installation #

1. Installer R/RStudio (R version 4.* recommandée)
1. Ouvrir R/Rstudio
1. Mettre le focus (curseur actif) sur la console:
    - dans R, vous n'avez qu'une console, donc pas de problème
    - dans Rstudio, la console est censée être en bas à gauche. Si vous ne la voyez pas, cliquez sur View(Affichage) > Panes (Panneau) > Zoom Console

![Rstudio console position](images/RStudioConsole.png)

Image source : [sthda - Running Rstudio and  setting up your working directory](http://www.sthda.com/english/wiki/running-rstudio-and-setting-up-your-working-directory-easy-r-programming)

5. Taper les commandes suivantes:

```r
install.packages("swirl")
#si besoin, installer les dépendances requises
library(swirl)
```

il vous faut maintenant installer le cours:

```r
install_course_github("jsansen", "beginrswirlified", "main") 
```

Vous êtes maintenant normalement prêt à démarrer le cours, il ne vous reste plus qu'à lancer le package.

```r
library(swirl) //(normalement déjà fait précédemment pour installer le cours mais a reproduire si vous éteignez R/RStudio)
swirl()
# répondre aux quelques questions posées et sélectionner le cours.
```
# Pour les éditeurs
suivre les indications disponibles sur le site de [swirlify](http://swirlstats.com/swirlify/writing.html)

# Remaining lessons TODO #

**TODO : réorganisation des modules**

1. R_101
1. **CORRECTIONS** Fichiers_et_espace_de_travail
1. Suites
1. Vecteurs
1. Sous-ensembles
1. Matrices_et_Dataframes
1. Logique
1. **TODO** : indexation de données (voir section concernée ci dessous)
1. **TODO** : Données et typages  (voir section concernée ci dessous)
1. Data_first_encounter
1. Valeurs_manquantes
1. Fonctions
1. Lapply_sapply
1. Vapply_tapply
1. **TODO** : structures de manipulation générales (voir section concernée ci dessous)
1. Lois_simulation
1. Graphiques_basiques
1. **TODO** : bibliothèques externes (voir section concernée ci dessous)


## les bibliothèques externes ##

Trouver, installer, charger rechercher et utiliser une bibliothèque ext.

## Données et typage ##

- différents types de base
    - character
    - numeric (real or decimal)
    - integer
    - logical
    - complex

structures de bases:
    - vecteurs
        - atomiques (monotypes)
        - listes (types multiples)
    - listes
    - Matrices
    - dataframes
    - facteurs

- différence vecteur/matrice/listes/array/dataframe
- conversions (cast)

## Indexation de données ##
Exercices pratiques

- accès à des données dans des vecteurs
- accès à des données dans des listes
- accès à des données dans des matrices
- accès à des données dans des dataframes

> acces aux lignes, accès aux colonnes, utilisation de which, etc

> nécéssite de le montrer après vecteurs, sequences, matrices df et logique

## Importation de données ##

Extension de fichier, separateur, décimal, header, autres formats

## les fonctions de manipulation générales ##

for/while/repeat loops

(en complément à la *apply family de R)

# source d'information externes #

- [Rstudio - Oreilly : how-to-write-fast-for-loops-in-r](https://rstudio-education.github.io/hopr/speed.html#how-to-write-fast-for-loops-in-r)
- [O'reilly- R for data sciences](https://r4ds.had.co.nz/introduction.html)

# Contenu du cours #

## R101 ##
Comme son nom l'indique, ce cours est à faire en premier et donne la base de R.

* Opérations simples
* Variables
* Création et opération de vecteurs

## Fichiers et espaces de travail ##

Içi, nous chercherons a travailler sur la notion d'espace de travail et la manipulation des fichiers. Cela est primordial à la bonne compréhension de la façon dont travaille R et comment il interprète votre système, comment lui faire ouvrir un fichier et naviguer dans votre espace de fichiers (votre ordinateur).
**TODO** corriger erreur de conception (retour dans le dossier test_dir après setwd(..), très perturbant pour les étudiants
**TODO** retirer la section file.path (peu utile et perturbant pour les étudiants + explication mal adaptée)
## Suites ##

Ici on voit la création de suites et les variants de création.

## Vecteurs ##

Ici on parle de vecteurs numérique(un peu), vecteur booléen et de manipulation de vecteurs de (chaînes de )caractères, methode paste etc.

### ~TODO~

- ~ajouter une partie sur les listes~
    - ~combinaisons de vecteurs de types et longueurs différentes~
    - ~comment les créer~
    - ~point rapide sur comment y accéder (avec ou sans nommage)~

## Valeurs manquantes ##

## Sous-ensembles ##

## Matrices_et_Dataframes ##

## Logique ##

## Fonctions ##

## Lapply_sapply ##

## Vapply_tapply ##

## Data_first_encounter ##

## Lois_simulation ##

## Graphiques_basiques ##
