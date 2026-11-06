# Rakuten France Multimodal Product Data Classification

## Team DS juil23_continu_ds

## Comment configurer votre environnement

1. Utilisez [vscode](https://code.visualstudio.com/) avec les extensions Microsoft pour Python et Jupyter.
2. Exécutez le script `Init.ipynb ` pour configurer correctement votre environnement.
3. Téléchargez les fichiers de ressources du projet, fournis sur [le site du challenge](https://challengedata.ens.fr/participants/challenges/35/), dans le dossier `resources`.
    * x_train: variables explicatives pour l’entraînement
    * y_train: variable(s) cible(s) pour l’entraînement
    * x_test: variables explicatives pour le test
    * images.zip: à décompresser dans le dossier `resources`
    * Vous devriez avoir à la fin dans `resources`:
        * `X_train_update.csv`
        * `Y_train_CVw08PX.csv`
        * `X_test_update.csv`
        * Un dossier `images` avec :
            * Un sous-dossier `image_test` avec 13812 éléments
            * Un sous-dossier `image_train` avec 84916 éléments
4. Vous pouvez commencer à dérouler le projet par `01 - Data Exploration.ipynb`

## Commit des notebooks

* Les notebooks contiennent le résultat de leur exécution, ce qui peut alourdir grandement les commits.
* Pour commiter les versions sans les résultats, beaucoup plus légères, éxécuter la commande suivante :
    * `python3 -m nbconvert --ClearOutputPreprocessor.enabled=True --ClearMetadataPreprocessor.enabled=True --inplace *.ipynb notebooks/*.ipynb`
* Pour générer leurs résultats avant de les ouvrir, exécuter la commande suivante :
    * `python3 -m nbconvert --ExecutePreprocessor.timeout=-1 --execute --inplace *.ipynb notebooks/*.ipynb`
        * `--ExecutePreprocessor.timeout=-1` évite les timeouts
* [Pour plus d'infos sur la gestion des notebooks avec git](https://mg.readthedocs.io/git-jupyter.html)

## Infos supplémentaires

* Vous devez mettre à jour le fichier `requirements.txt` lors de l'ajout de nouvelles librairies au projet.
* Les fichiers et sous-dossiers dans `resources` ne seront pas versionnés.