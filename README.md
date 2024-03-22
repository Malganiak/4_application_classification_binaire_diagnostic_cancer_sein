# 4_application_classification_binaire_diagnostic_cancer_sein

Diagnostic du cancer du sein par classification binaire avec la régression logistique

Introduction :
Cette présentation se consacre à la classification binaire, l'une des principales tâches du Machine Learning supervisé, en se penchant particulièrement sur son application au diagnostic du cancer du sein. Nous explorerons le Breast Cancer Wisconsin (diagnostic) Dataset, un ensemble de données classique, et utiliserons la régression logistique comme modèle de Machine Learning pour identifier le type de tumeur (bénigne ou maline) en fonction des caractéristiques géométriques mesurées sur les cellules issues de la biopsie.

Contexte du projet :
Le jeu de données se compose de 569 exemples, chacun caractérisé par 30 propriétés géométriques mesurées sur des cellules issues de la biopsie. La tumeur est classée comme "Benign" (n=357) si elle est bénigne et comme "Malignant" (n=212) si elle est maligne. Notre objectif est de former un modèle de Machine Learning pour identifier le type de tumeur en fonction de ces propriétés géométriques.

Concepts de base dans le notebook :

Classification binaire
Matrice de confusion
Faux négatif, vrai négatif, faux positif, vrai positif
Taux de classification (accuracy)
Rappel (recall)
Précision (precision)
F1-score
Courbe ROC
Area Under the Curve (AUC)
Description additionnelle dans le notebook :

Régression logistique
Feature Scaling
Objectif et avantages
Normalisation des données
Standardisation des données
Utilisation avec des ensembles d'entraînement et de test distincts
Implémentation en Python dans le Jupyter Notebook :

Importation des librairies Python nécessaires
Chargement des données du Breast Cancer Wisconsin (diagnostic) Dataset
Mise au format Numpy des données
Relabellisation des patients sains et malades
Echantillonnage des données (test_size = 113)
Affichage sous forme d'histogrammes de la distribution des données initiales, du jeu d'entraînement et du jeu de test pour chaque catégorie (bénigne et maline)
Feature Scaling
Entraînement du modèle de régression logistique (model = LogisticRegression(C = 0.1, max_iter = 10000))
Calcul et affichage des performances sur le jeu d'entraînement :
Matrice de confusion
Taux de classification, rappel, précision et F1-score
Courbe ROC, AUC
Calcul et affichage des performances sur le jeu de test :
Matrice de confusion
Taux de classification, rappel, précision et F1-score
Courbe ROC, AUC

Conclusion :
Nous avons désormais les éléments nécessaires pour fournir un outil d'aide à la prise de décision clinique au corps médical via un Jupyter Notebook.
