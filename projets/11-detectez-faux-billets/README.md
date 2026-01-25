Projet 11 : ONCFM — Détection automatique de faux billets (Machine Learning)

🎯 Objectifs  
Développer un algorithme capable de prédire automatiquement si un billet en euros est **vrai** ou **faux** à partir de ses caractéristiques géométriques, puis livrer une **application/script** utilisable par les équipes ONCFM. 

Pour cela, nous allons :
- Réaliser une **analyse descriptive** du jeu de données (répartition des variables, équilibre vrai/faux, etc.). :contentReference[oaicite:1]{index=1}
- Préparer les données et construire un pipeline de traitement (contrôles, nettoyage si nécessaire, standardisation selon les modèles). :contentReference[oaicite:2]{index=2}
- Tester et comparer 4 algorithmes recommandés : **Régression logistique**, **K-Means**, **KNN**, **Random Forest**. 
- Évaluer les modèles avec une **matrice de confusion** (faux positifs / faux négatifs). :contentReference[oaicite:4]{index=4}
- Choisir le **modèle final** selon le critère métier prioritaire : détecter un maximum de faux billets. :contentReference[oaicite:5]{index=5}
- Livrer un **script de prédiction** utilisable en production (valeurs unitaires ou fichier CSV). 
- Présenter la démarche et les résultats dans un **support** clair. 

📋 Présentation du sujet  

Contexte  
L’Organisation nationale de lutte contre le faux-monnayage (ONCFM) souhaite mettre en place une application de machine learning pour aider les équipes à identifier plus rapidement les contrefaçons. Après scan d’un billet (mesures physiques), l’outil doit prédire sa nature : vrai/faux. 

Les données (features disponibles)  
Chaque billet est décrit par **6 dimensions géométriques** (en mm) : :contentReference[oaicite:9]{index=9}
- length : longueur
- height_left : hauteur côté gauche
- height_right : hauteur côté droit
- margin_up : marge supérieure (bord → image)
- margin_low : marge inférieure (bord → image)
- diagonal : diagonale

Un fichier d’exemple contient **1 500 billets** : **1 000 vrais** et **500 faux**, avec une colonne indiquant la classe. 

Les modèles à comparer  
L’ONCFM souhaite mettre en concurrence 4 approches : 
- Régression logistique
- K-Means (en utilisant les centroïdes pour la prédiction)
- KNN
- Random Forest

Comment lire les résultats (repères simples)  
- **Matrice de confusion** : permet de voir concrètement les erreurs du modèle (nombre de faux billets détectés vs manqués, et vrais billets rejetés à tort). :contentReference[oaicite:12]{index=12}  
- **Faux négatif (FN)** = un faux billet prédit comme vrai → c’est l’erreur la plus critique si l’objectif est d’identifier un maximum de contrefaçons. :contentReference[oaicite:13]{index=13}  
- **Faux positif (FP)** = un vrai billet prédit comme faux → gêne opérationnelle (contrôle inutile), mais moins critique que laisser passer une contrefaçon (selon la logique métier). :contentReference[oaicite:14]{index=14}

Exigence “production” (script)  
Le livrable final doit être un **script** qui : 
- prend en entrée soit les **valeurs** d’un billet, soit le **chemin** vers un fichier CSV (format type fourni : `billets_production.csv`) ;
- renvoie un **output binaire** (vrai/faux) pour un ou plusieurs billets.

Livrables attendus  
- Un notebook avec : analyse descriptive, préparation, entraînement/évaluation des 4 modèles, comparaison et sélection finale.   
- Un **script de prédiction** “fonctionnel” (utilisable par l’ONCFM).   
- Un support de présentation incluant : traitements amont, résultats des modèles, choix du modèle final, démonstration du script. 