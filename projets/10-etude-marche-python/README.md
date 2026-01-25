# Projet 10 : La Poule qui Chante – Étude de faisabilité à l’export (ACP + Clustering)
 
# 🎯 Objectifs  
Proposer au COMEX des **groupements de pays** à cibler pour exporter des poulets “AB”, avec une démarche claire et des recommandations compréhensibles (15 min, peu technique). :contentReference[oaicite:0]{index=0}

Pour cela, nous allons :
- Partir des données **FAO** fournies et compléter avec d’autres sources open data. :contentReference[oaicite:1]{index=1}
- Utiliser une analyse **PESTEL** pour identifier des variables utiles à ajouter (minimum **8 variables**). :contentReference[oaicite:2]{index=2}
- Préparer / nettoyer les données et regrouper les sources dans un **fichier unique** si nécessaire. :contentReference[oaicite:3]{index=3}
- Construire un périmètre robuste : **≥ 100 pays** couvrant **≥ 60%** de la population mondiale. :contentReference[oaicite:4]{index=4}
- Réaliser une **exploration** des données (notebook 1). :contentReference[oaicite:5]{index=5}
- Réaliser une **ACP** + un **clustering** (notebook 2 séparé) : CAH puis K-Means. :contentReference[oaicite:6]{index=6}
- Présenter les résultats + recommandations (pays/segments) dans un **support** adapté au COMEX. :contentReference[oaicite:7]{index=7}

# 📋 Présentation du sujet  

# Contexte  
La Poule qui Chante est une entreprise française d’agroalimentaire dont l’activité principale est l’élevage et la vente de poulets labellisés “Poulet Agriculture Biologique”.  
Le PDG souhaite évaluer un développement à l’international, sans pays cible défini à ce stade (tous les pays sont envisageables). :contentReference[oaicite:8]{index=8}

# La demande métier  
Objectif principal : **identifier des groupes de pays** pertinents à cibler pour une première phase d’export, avant l’étude de marché détaillée. :contentReference[oaicite:9]{index=9}

# Les données  
- Point de départ : données **FAO** (pièce jointe au brief). :contentReference[oaicite:10]{index=10}  
- Enrichissement : données open data (FAO, Banque Mondiale, etc.) guidé par **PESTEL**. :contentReference[oaicite:11]{index=11}  
- Contraintes : au minimum **8 variables**, au moins **100 pays**, couvrant **60%** de la population mondiale. :contentReference[oaicite:12]{index=12}

# Les analyses attendues (notebooks)  
Notebook 1 — Exploration  
- Contrôles qualité (valeurs manquantes, cohérence, outliers, distributions).  
- Premières lectures (corrélations, tendances, ordres de grandeur). :contentReference[oaicite:13]{index=13}

Notebook 2 — ACP + Clustering  
- **ACP** : réduction de dimension, analyse du cercle des corrélations, projection des individus. :contentReference[oaicite:14]{index=14}  
- **Clustering** :  
  - commencer par une **CAH** (classification ascendante hiérarchique),  
  - puis un **K-Means** (sur données ACP ou données brutes). :contentReference[oaicite:15]{index=15}

# Comment lire les résultats (repères “COMEX”)  
- **ACP** : sert à résumer l’information de plusieurs variables en quelques axes lisibles et comparables. :contentReference[oaicite:16]{index=16}  
- **Clustering** : regroupe les pays “qui se ressemblent” pour proposer des segments cibles cohérents (au lieu de choisir un pays au hasard). :contentReference[oaicite:17]{index=17}  
- **CAH vs K-Means** : deux méthodes de regroupement à comparer (cohérence / différences de segmentation). :contentReference[oaicite:18]{index=18}

# Livrables attendus  
- 2 notebooks :  
  1) exploration des données,  
  2) ACP + clustering (séparé). :contentReference[oaicite:19]{index=19}  
- 1 support de présentation (15 min) :  
  - contexte,  
  - démarche (collecte + préparation + analyses),  
  - résultats (segments),  
  - recommandations de pays/segments à prioriser. :contentReference[oaicite:20]{index=20}