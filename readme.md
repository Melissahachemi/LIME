======================================================
PROJET : Explicabilité de Modèles (LIME)
======================================================


## 1. Instructions d'Exécution

Pour exécuter les expériences et reproduire les résultats du projet, veuillez suivre ces étapes :

### 1.1. Pré-requis

Assurez-vous que l'environnement d'exécution dispose de Python (version recommandée : **Python 3.9+**).

### 1.2. Installation des Dépendances

Les bibliothèques requises sont listées ci-dessous :

* numpy (>= 1.22.0)
* pandas (>= 1.4.0)
* scikit-learn (>= 1.0.0)
* matplotlib (>= 3.5.0)
* jupyter (pour exécuter le notebook)

Vous pouvez installer toutes les dépendances via la commande suivante :

pip install numpy pandas scikit-learn matplotlib jupyter


### 1.3. Exécution du code 

Assurez-vous que les fichiers lime_implementation.py et experimentation.ipynb se trouvent dans le même répertoire.
1-Naviguez jusqu'au répertoire du projet dans le terminal ou invite de commande :

					cd LIME

2-Lancez le Notebook Jupyter. pour importer correctement la classe SimpleLIME :

					jupyter notebook experimentation.ipynb

3-Ouvrez le fichier experimentation.ipynb dans le navigateur et exécutez toutes les cellules séquentiellement pour :

								dérouler les expériences.
							        entraîner le modèle .
								générer les explications LIME.
