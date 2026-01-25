# Projet 9 : DWFA – Drinking Water For All (Accès à l’eau potable)

# 🎯 Objectifs  
Réaliser un tableau de bord (Tableau ou Power BI) destiné à un bailleur de fonds pour :
- identifier les pays en difficulté d’accès à l’eau potable ;
- identifier les pays sur lesquels concentrer les efforts de l’ONG.

## Pour cela, nous allons :
- Sélectionner des indicateurs pertinents (socle commun + indicateurs par domaine d’expertise).
- Synthétiser le besoin via un document (et éventuellement un blueprint / mockup).
- Préparer les données (nettoyage, jointures, champs calculés).
- Construire 3 vues (monde / continent / pays) avec filtres et interactivité.
- Optimiser l’accessibilité et la lisibilité du dashboard.
- Présenter les résultats dans un support (PowerPoint ou équivalent).

# 📋 Présentation du sujet  

## Contexte  
DWFA (Drinking Water For All) est une ONG dont l’ambition est de donner accès à l’eau potable à tous.  
Elle intervient via 3 domaines d’expertise :
1) Création de services d’accès à l’eau potable  
2) Modernisation de services existants  
3) Consulting auprès d’administrations/gouvernements sur les politiques d’accès à l’eau  

DWFA a fait une demande de financement : si elle est accordée, elle permettra d’investir dans un des 3 domaines, dans un pays encore à déterminer.  
Le tableau de bord sert donc à guider la décision (où intervenir, et via quel type d’action).

# Les vues attendues (3 niveaux)  
1) Vue mondiale : indicateurs agrégés au niveau global  
2) Vue continentale : indicateurs agrégés pour le continent sélectionné  
3) Vue nationale : indicateurs détaillés pour le pays sélectionné  

# Les indicateurs (socle + par domaine)  

## Socle commun (pour comparer et prioriser)  
- Part de la population ayant accès à l’eau potable  
- Taux de mortalité lié à une eau insalubre  
- Population / densité de population  
- Stabilité politique  
- Évolution de certains indicateurs dans le temps (tendance)

Domaine 1 — Création de services  
Objectif : évaluer la difficulté “terrain” selon l’urbanisation.  
- Scatter : accès à l’eau potable (%)  VS  population urbaine (%)

Domaine 2 — Modernisation des services  
Objectif : repérer les pays qui ont des infrastructures “basiques” mais peu de services de qualité.  
- Scatter : services “basiques” (%)  VS  services “safely managed” (%)

Domaine 3 — Consulting (politiques publiques)  
Objectif : cibler les pays “consultables” (enjeu fort + contexte politique exploitable).  
- Scatter : efficacité politique d’accès à l’eau (accès élevé + mortalité faible)  VS  stabilité politique  
- Filtre dédié : exclusion des pays trop instables (seuil modifiable par l’utilisateur)

## Comment lire ces indicateurs (repères simples)  
- Accès à l’eau faible + mortalité élevée = urgence d’intervention  
- Population très rurale = création de services plus complexe (logistique / dispersion)  
- “Basiques” élevés mais “safely managed” faibles = priorité modernisation / qualité  
- Stabilité politique trop faible = risque élevé pour le consulting (d’où le filtre)

## Livrables attendus  
- Document de synthèse des indicateurs retenus par vue (blueprint / mockup optionnel)  
- Tableau de bord (Tableau Public via Story ou Power BI)  
- Support de présentation : contexte, préparation des données, justification de l’outil et démonstration du dashboard