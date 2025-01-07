# Classification des Coups de Tennis avec Deep Learning

Ce projet vise à classifier différents types de coups de tennis à partir de données d'accélération et de gyroscope enregistrées avec un accéléromètre positionné sur le manche d'une raquette.

## Description du Jeu de Données

Le jeu de données contient des mesures d'accélération et de gyroscope pour différents types de coups de tennis. Chaque coup est représenté par 100 lignes de données, comprenant :

- **6 variables prédictives** :
  - `AccX`, `AccY`, `AccZ` : Composantes d'accélération.
  - `GyrX`, `GyrY`, `GyrZ` : Composantes du gyroscope.
- **1 variable cible (Labels)** :
  - `0` : Service
  - `1` : Coup droit de fond
  - `2` : Revers de fond
  - `3` : Coup droit de volée
  - `4` : Revers de volée

Après prétraitement, les données sont transformées comme suit :
- **X** : Tableau 3D de dimensions `(2013, 100, 6)` représentant 2013 coups, chacun décrit par 100 frames de 6 variables.
- **y** : Vecteur unidimensionnel de taille `(2013,)` contenant les labels associés.

## Objectif

L'objectif est de construire différents modèles de Deep Learning capablent de labelliser automatiquement le type de coup réalisé à partir des variables d'accélération et de gyroscope. Nous comparons ensuite les résultats des différents modèles. 

