# PESSD – Comment comprendre ce que mesure l’Insee ?

**Projet en Économie, Sociologie et Science des Données (PESSD)**  
**ENSAE Paris — Année 2024–2025**  
**Auteurs : Paul Dupire, Catherine Berleur**

---

## Objectif

Ce projet explore l’évolution des publications *Insee Première* et *Insee Analyse* entre 2010 et 2025, à travers une analyse diachronique du langage statistique employé par l’Insee.  
Grâce à des techniques avancées de **traitement automatique du langage naturel (NLP)** et de **plongement lexical Word2Vec**, nous visons à :

- Cartographier la terminologie utilisée par l’Insee
- Analyser les évolutions sémantiques et thématiques au fil du temps
- Comprendre les articulations entre méthodes statistiques et objets d’étude

---

## Données

Le corpus provient de deux publications de l’Insee :

- **Insee Première** (2011–2025) : publications courtes sur des sujets d’actualité
- - insee_premiere.csv
- **Insee Analyse** (2010–2025) : publications courtes et documents de travail
- - insee_analyse.csv
Les données accessibles sur le github sont tronquées par rapport aux données totales faute de place disponible sur github.

Chaque publication contient :
- Texte complet
- Date de publication
- Thème et sous-thème
- Onglet méthodologie
---

## Méthodologie
**A. Statistiques descriptives**
**B. NLP**

1. **Prétraitement linguistique** :  
   - Lemmatisation  
   - Nettoyage des textes  
   - Suppression des mots-outils

2. **Vectorisation sémantique** *(Word2Vec - Skip-Gram)*  
   - Entraînement par période de 4 ans  
   - Fenêtre contextuelle : 10 mots  
   - Dimension des vecteurs : 200

3. **Alignement diachronique**  
   - Méthode de Procrustes orthogonale  
   - Suivi des trajectoires sémantiques entre périodes

4. **Visualisation**  
   - Réduction de dimension avec **PaCMAP**  
   - Clustering lexical et cartographie thématique

---

## Résultats clés

- Une **structure lexicale cohérente** par grands domaines analytiques
- Un **développement des analyses locales** sans abandon des thématiques traditionnelles
- Une **généralisation transversale** de l’usage des concepts statistiques distributionelles (ex. : *décile*)

---

## Notebook

[Notebook_Pessd.ipynb](https://github.com/PaulD10/PESSD-/blob/main/Notebook_Pessd.ipynb)


