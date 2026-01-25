# Projet 8 : Analyse des ventes d’une librairie en ligne (Lapage)

# 🎯 Objectifs  
Réaliser une analyse orientée “décision” pour le CODIR (15 min, public non-technique) afin de faire un point global sur l’activité e-commerce et le comportement client. :contentReference[oaicite:0]{index=0}

# Pour cela, nous allons :
- Construire et vérifier un dataset exploitable à partir de la base fournie.
- Produire des indicateurs de vente (CA, volumes, clients, produits…) et des visualisations claires. :contentReference[oaicite:1]{index=1}
- Faire un zoom produit (tops/flops, répartition par catégories). :contentReference[oaicite:2]{index=2}
- Analyser des profils clients (BtoB, concentration du CA via courbe de Lorenz, etc.). :contentReference[oaicite:3]{index=3}
- Étudier 5 corrélations clés demandées par l’équipe BI (Julie). :contentReference[oaicite:4]{index=4}
- Synthétiser les résultats en recommandations actionnables pour la direction. :contentReference[oaicite:5]{index=5}

# 📋 Présentation du sujet  

# Contexte  
Lapage est une librairie historique (plusieurs points de vente) qui a ouvert un site de vente en ligne il y a environ 2 ans. L’entreprise souhaite mieux comprendre ses performances e-commerce pour décider des prochaines actions (offres, prix, ciblage, etc.). :contentReference[oaicite:6]{index=6}

# Les demandes métier  
1) Indicateurs de vente (brief Annabelle / Sylvain)  
Graphiques et KPI attendus, par exemple : :contentReference[oaicite:7]{index=7}
- Évolution du chiffre d’affaires dans le temps + moyenne mobile (période au choix : jour/semaine/mois).
- Chiffre d’affaires par catégorie.
- Nombre de clients par mois.
- Nombre de transactions.
- Nombre de produits vendus.
- Zoom “références” : tops, flops, répartition par catégorie.

2) Analyse clients (demandes Julie – comportement client)  
Étudier en particulier ces 5 relations : :contentReference[oaicite:8]{index=8}
- Lien entre le genre et les catégories de livres achetés.
- Lien entre l’âge et le montant total des achats.
- Lien entre l’âge et la fréquence d’achat.
- Lien entre l’âge et la taille du panier moyen.
- Lien entre l’âge et la catégorie des livres achetés.

# Comment lire / interpréter les résultats (version “CODIR”)  
- **Moyenne mobile** : lisse les variations (pics/creux) pour mieux voir la tendance de fond du CA.   
- **Tops / flops** : identifie les références qui tirent le CA (ou qui freinent), pour ajuster stock, mise en avant, prix. :contentReference[oaicite:10]{index=10}  
- **Courbe de Lorenz (concentration du CA)** : montre si une minorité de clients génère une grande partie du CA (utile pour piloter fidélisation et risques). :contentReference[oaicite:11]{index=11}  
- **Corrélations / tests** : on choisit le test selon le type de variables (quali/quanti) pour conclure proprement (et éviter les interprétations “à l’intuition”). 

# Livrables attendus  
- Un notebook (Jupyter ou R Markdown) contenant préparation + analyses (Annabelle + Julie). :contentReference[oaicite:13]{index=13}  
- Un support de présentation (PPT ou équivalent) pour le CODIR, format clair et non-technique, 15 minutes. :contentReference[oaicite:14]{index=14}