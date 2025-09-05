# Détection de Fraude Bancaire avec Machine Learning

Ce projet vise à développer un modèle de machine learning capable d’identifier les transactions bancaires frauduleuses à partir de données clients, commerçants, appareils et lieux de transaction.

## Objectifs

- Détecter les transactions frauduleuses et légitimes.
- Identifier les anomalies et comportements suspects.
- Analyser les caractéristiques influençant la fraude (commerçants, appareils, localisations, types de compte).
- Optimiser la précision tout en limitant les faux positifs/négatifs.
- Proposer une solution évolutive pour la détection en temps réel.

## Pipeline du projet

1. **Importation des données** : Chargement et exploration du jeu de données.
2. **Prétraitement** : Nettoyage, gestion des valeurs manquantes, suppression des colonnes inutiles.
3. **Analyse exploratoire (EDA)** : Visualisation et analyse des variables numériques et catégorielles.
4. **Feature Engineering** : Conversion des dates, extraction de nouvelles variables.
5. **Encodage** : Transformation des variables catégorielles en variables numériques.
6. **Sélection de variables** : Importance des variables via Random Forest.
7. **Réduction de dimension** : Application de l’ACP (PCA).
8. **Train-test split** : Séparation des données pour l’entraînement et le test.
9. **Normalisation** : Mise à l’échelle des variables.
10. **Traitement du déséquilibre** : Utilisation de SMOTE et des poids de classe.
11. **Modélisation** : Entraînement et évaluation de plusieurs modèles (Logistic Regression, Random Forest, XGBoost, LightGBM, CatBoost, etc.).
12. **Évaluation** : Comparaison des modèles via précision, ROC AUC, matrices de confusion.

## Résultats

Le modèle de détection de fraude obtient de bons résultats globaux :  
- Précision élevée sur l’ensemble des données.
- Les principales transactions frauduleuses sont bien identifiées.
- Les métriques d’évaluation (accuracy, ROC AUC, F1-score) montrent une performance satisfaisante, en particulier pour la classe majoritaire.

Cependant, comme souvent en détection de fraude, la classe minoritaire reste plus difficile à détecter, mais le système permet déjà de réduire significativement le

## Conclusion

Le projet met en évidence la difficulté de la détection de fraude en présence d’un fort déséquilibre de classes. Des techniques avancées de rééquilibrage et d’optimisation sont nécessaires pour améliorer la détection des fraudes.

## Fichiers

- [`analyse-transactions-frauduleusesEXEc.ipynb`](analyse-transactions-frauduleusesEXEc.ipynb) : Notebook principal contenant tout le pipeline d’analyse et de modélisation.

---

*Projet réalisé dans le cadre d’une analyse de transactions bancaires pour la détection de
