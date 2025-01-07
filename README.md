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

## Objectif

L'objectif est de construire différents modèles de Deep Learning capablent de labelliser automatiquement le type de coup réalisé à partir des variables d'accélération et de gyroscope. Nous comparons ensuite les résultats des différents modèles. 

