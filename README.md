# Projet d'Évaluation des Options Température

Ce projet évalue la juste valeur des options de température, à la fois sous une approche Monte Carlo et une approche similaire à Black-Scholes sous la mesure risque-neutre. Il calcule la valeur des options call et put basées sur les "heating degree days" (HDD), en tenant compte de la volatilité et des paramètres du marché pour des contrats d'hiver.

## Description du Projet

Le projet permet de modéliser les options basées sur les températures, en particulier les options de température appelées "Winter Temperature Options". Les modèles incluent des simulations Monte Carlo pour estimer les prix des options et une approche de pricing en utilisant des mesures de volatilité et des paramètres de risque. Les résultats peuvent être utilisés pour l'évaluation des contrats à terme sur des dérivés climatiques, comme les options liées aux degrés-jours de chauffage.

## Méthodes Utilisées

1. **Méthode de Monte Carlo** : Simulation de 10 000 trajectoires de température pour évaluer le prix des options avec un échantillon de données sur plusieurs années.
2. **Modèle BSA (Black-Scholes Adapté)** : Application de la formule de Black-Scholes pour le pricing des options en fonction des degrés-jours de chauffage, avec des ajustements de volatilité et du taux d'intérêt.

## Fonctionnalités

- **Options Call et Put** : Calcul de la valeur d'options basées sur des températures avec une gestion de la volatilité et du risque à l'aide de la mesure risque-neutre.
- **Modélisation de la Volatilité** : Utilisation de modèles de volatilité pour ajuster les prix selon les variations de température au fil du temps.
- **Visualisation** : Graphiques des prix des options avec différentes strikes, pour aider à l'analyse des impacts des variations des températures.

## Installation

1. Clonez ce projet sur votre machine locale.
2. Assurez-vous d'avoir les dépendances suivantes installées :
   - `numpy`
   - `pandas`
   - `scipy`
   - `matplotlib`
   - `statsmodels`

Vous pouvez installer ces dépendances avec `pip` :
```bash
pip install numpy pandas scipy matplotlib statsmodels
