# Projets-Power-Query-Cas-pratiques-de-transformation-de-donn-es
Projet de transformation et d’analyse de données avec Power Query. Contient plusieurs cas pratiques : nettoyage, dé-pivotage, consolidation de fichiers volumineux et préparation de datasets pour tableaux croisés dynamiques (TCD) et analyses avancées.

## Cas 1 : traitement.xlsx

Ce jeu de données présente les ventes quotidiennes réalisées en mars 2025 dans trois villes : Paris, New York et Londres. Les informations incluent la date, la ville, le montant des ventes ainsi qu’un total journalier.

Cependant, la structure initiale du fichier n’est pas directement exploitable pour l’analyse. Plusieurs problèmes sont observés : présence de lignes de totaux, répétition des villes pour chaque date et incohérences dans l’écriture des noms de villes.

L’objectif de ce projet est d’utiliser Power Query afin de nettoyer et transformer les données pour obtenir une table structurée contenant les colonnes suivantes :

- Date

- Ville

- Ventes

Une fois les données préparées, elles peuvent être utilisées pour analyser l’évolution des ventes et comparer les performances entre les différentes villes.

## Cas 2 : ventes_entreprise.csv

Le fichier CSV contient environ 1000 transactions réalisées entre 2023 et 2025, avec les colonnes suivantes :
ID, date de vente, client, produit, catégorie, quantité, prix unitaire, total, mode de paiement et ville.

Objectifs du traitement avec Power Query

Corriger l’encodage des caractères et nettoyer les colonnes.

Convertir les dates et les nombres dans le format approprié.

Vérifier et recalculer les totaux afin d’assurer la cohérence des données.

Préparer le dataset pour des analyses par catégorie, ville, produit ou mode de paiement.

## Cas 3 : Dé-pivotage d’un tableau

Le tableau contient les ventes de différents produits dans quatre villes : Paris, Nice, Marseille et Toulouse. Les colonnes incluent l’identifiant du produit, le nom du produit et les montants de vente par ville.

Objectifs du traitement avec Power Query

Dé-pivoter le tableau afin de passer d’un format large (une colonne par ville) à un format long (une ligne par produit et par ville).

Créer des colonnes normalisées :

- Identifiant

- Produit

- Ville

- Montant (€)

Convertir les montants en valeurs numériques pour faciliter les calculs.

Préparer les données pour la création d’un tableau croisé dynamique (TCD) et des analyses par produit et par ville.

## Cas 4 : Gestion d’un fichier volumineux (.txt)

Le fichier TXT contient 2 000 000 de lignes avec les colonnes suivantes :
ID, Nom, Titre et Salaire.

La limite de lignes d’Excel (1 048 576 lignes) ne permet pas de charger l’ensemble des données dans une feuille classique.

Objectifs du traitement avec Power Query

Importer le fichier TXT directement dans Power Query pour contourner la limitation du nombre de lignes d’Excel.

Nettoyer et convertir les colonnes :

- ID en entier

- Nom et Titre en texte

- Salaire en nombre décimal

Préparer les données pour générer un tableau croisé dynamique (TCD) permettant d’analyser les salaires par titre, par nom ou par regroupement spécifique.

Maintenir les 2 000 000 de lignes dans Power Query sans les charger intégralement dans Excel afin de garantir la performance et la fiabilité des analyses.

## Cas 5 : Consolidation de plusieurs fichiers (Retailers)

Ce projet implique trois fichiers distincts correspondant aux enseignes Costco, Target et Walgreens, possédant les mêmes colonnes :

- Retailer

- Contact

- Retailer ID

- Order Date

- Payment Date

- Region--State

- Beverage Brand

- Price per Unit

- Units Sold

Chaque fichier contient l’historique des ventes avec des informations sur les produits, les quantités vendues et les prix unitaires.

Objectifs du traitement avec Power Query

Importer et consolider les trois fichiers dans Power Query afin d’obtenir un seul dataset pour l’analyse.

Nettoyer et harmoniser les données : correction de l’encodage, conversion des dates et des montants, suppression des caractères ou espaces inutiles.

Préparer les données pour des analyses avancées, notamment le calcul du chiffre d’affaires par enseigne, par produit, par région ou par période.

Faciliter la création de tableaux croisés dynamiques (TCD) et de visualisations analytiques.

Cette approche permet de gagner du temps, de réduire les erreurs de manipulation manuelle et de disposer d’un dataset fiable pour les analyses comparatives entre enseignes et produits.
