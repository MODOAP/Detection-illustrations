Détection d'images dans les documents historiques

Script d'auto apprentissage
Ce script permet d'entraîner l'algorithme Mask-RCNN à la segmentation d'objets sur ses propres données d'entraînement.
Il requiert un corpus d'entraînement : un dossier sur un Google Drive composé de deux dossiers "train" et "val" contenant chacun les images et leur fichier d'annotation.
L'annotation du corpus peut être opérée grâce aux outils VIA (https://www.robots.ox.ac.uk/~vgg/software/via/) et Annotate.

Le script implémente la configuration décrite sur https://github.com/matterport/Mask_RCNN
