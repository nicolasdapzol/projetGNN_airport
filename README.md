# TP M2 IA DL GNN 
# Yann Amer Jules Caroile et Nicolas Dapzol 
#
# prédiction de liesn entre aéroports


# résumé : 
Ce projet étudie la prédiction de liens entre aéroports.
Dans une première partie , nous enrichissons la base initiale : de nouvelles features sont ajoutées ( coordonnées 3D , normalisation de la population et one_hot encoding )
Dans une deuxième parties des modèles GNN sont comparés avec différentes couches de convolution (GCN, GAT et GraphSAGE) et évalués avec l'AUC et l'Average Precision ainsi que les matrices de confusions

## Reproduire les expériences

1. Préparer un environnement Python avec PyTorch, PyTorch Geometric, NetworkX, pandas, NumPy, scikit-learn, matplotlib et seaborn. Utiliser des versions compatibles entre PyTorch et PyTorch Geometric.
2. Depuis `code/`, ouvrir et exécuter toutes les cellules de `0_import_data et description.ipynb`. Le notebook lit `../data/airportsAndCoordAndPop.graphml`, construit les caractéristiques et génère les jeux train, validation et test dans `data/`.
3. Exécuter toutes les cellules de `1 construction_modeles.ipynb`. Le notebook entraîne les modèles puis enregistre les modèles et résultats dans `resultats/` et affiche les indicateurs ainsi queles graphiques dans le notebook

Les fichiers `.pt` de `data/` contiennent les jeux de données et splits déjà générés : les conserver permet de réutiliser le même découpage. 


Note 1 : utilisation IA : 
COPILOT : correction de bugs 
COPILOT : création de coordonnées 3D 

Note 2 : 
Les notebooks de `code/backup/` sont des variantes ou essais antérieurs et ne font pas partie du parcours principal.

