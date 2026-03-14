# 🚀 Projet : Implémentation de LIME (Local Interpretable Model-agnostic Explanations)
---

## 📝 1. Introduction & Contexte
L'intelligence artificielle moderne repose sur des modèles complexes ("boîtes noires") comme Random Forest ou les réseaux de neurones. Bien que performants, ils sont opaques. Ce projet implémente **LIME**, une méthode qui explique les prédictions localement en créant un modèle linéaire interprétable autour d'une instance spécifique.

### Objectifs du projet :
1. **Implémentation "from scratch"** de l'algorithme LIME en Python.
2. **Compréhension des mécanismes** : échantillonnage gaussien, pondération par noyau RBF et régression locale.
3. **Analyse des hyperparamètres** : étude de l'influence de la largeur du noyau ($\sigma$) et du nombre d'échantillons ($n\_samples$).
4. **Validation** : comparaison avec l'implémentation officielle de LIME.

---

## 🛠️ 2. Méthodologie
L'implémentation suit les étapes clés suivantes :
* **Génération de données** : Création de variations autour de l'instance à expliquer via des perturbations gaussiennes.
* **Prédiction** : Utilisation du modèle complexe pour prédire les labels de ces nouvelles instances.
* **Calcul des poids** : Application d'un noyau RBF pour accorder plus d'importance aux instances proches de l'originale.
* **Modèle d'explication** : Entraînement d'une régression Ridge (modèle interprétable) sur les données pondérées.

---

## 3. Instructions d'Exécution

Pour exécuter les expériences et reproduire les résultats du projet, veuillez suivre ces étapes :

### 3.1. Pré-requis

Assurez-vous que l'environnement d'exécution dispose de Python (version recommandée : **Python 3.9+**).

### 3.2. Installation des Dépendances

Les bibliothèques requises sont listées ci-dessous :

* numpy (>= 1.22.0)
* pandas (>= 1.4.0)
* scikit-learn (>= 1.0.0)
* matplotlib (>= 3.5.0)
* jupyter (pour exécuter le notebook)

Vous pouvez installer toutes les dépendances via la commande suivante :

pip install numpy pandas scikit-learn matplotlib jupyter


### 3.3. Exécution du code 

Assurez-vous que les fichiers lime_implementation.py et experimentation.ipynb se trouvent dans le même répertoire.
1-Naviguez jusqu'au répertoire du projet dans le terminal ou invite de commande :

					cd LIME

2-Lancez le Notebook Jupyter. pour importer correctement la classe SimpleLIME :

					jupyter notebook experimentation.ipynb

3-Ouvrez le fichier experimentation.ipynb dans le navigateur et exécutez toutes les cellules séquentiellement pour :

								dérouler les expériences.
							        entraîner le modèle .
								générer les explications LIME.
