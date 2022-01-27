MODOAP - Détection et extraction d'illustrations dans les pages de journaux / manuels / magazines





# ModOAP - Détection d'illustrations dans les documents Gallica

Ce carnet permet de détecter et extraire les illustrations dans les pages d'un corpus de documents Gallica. Il requiert :

- des poids issus de l'entraînement préalable d'un modèle sur un corpus particulier
- un corpus de journaux / manuels sur lequel opérer la détection : il s'agit d'un dossier contenant directement les pages des documents au format image.

Le script implémente la configuration décrite sur https://github.com/matterport/Mask_RCNN

Il doit être lancé dans un environnement d'exécution GPU : Exécution -> Modifier le type d'exécution -> GPU

Ce carnet nécessite de synchroniser un compte Google Drive.


## Utilisation

1. Ouvrir le carnet dans l'interface Google Colab et se connecter à un compte Google Drive 

2. Lancer la première cellule et cliquer sur le lien généré pour synchroniser un compte Drive si demandé.
Cette cellule importe les bibliothèques nécessaires à l'utilisation du carnet, et connecte un compte Drive.

3. Dans la cellule "Chargement du modèle", spécifier le chemin vers le dossier Google Drive contenant le modèle entraîné et lancer la cellule. 

4. Dans la cellule suivante : 

	- Spécifier le chemin vers le dossier contenant le corpus d'images à classer
	- Spécifier le chemin vers le dossier où sauvegarder les images classées
	- Spécifier le seuil au dessus duquel associer une image à une classe (par défaut 80)
	- Lancer la cellule

5. Lancer la cellule "Visualiser la répartition des classes associées" pour générer un graphique des classes attribuées
