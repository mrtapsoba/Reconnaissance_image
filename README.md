# Étude sur CNN avec TensorFlow sur les images CIFAR10

## Auteur : TAPSOBA Abdoul Kader

Ce projet est une étude sur l'utilisation des réseaux de neurones convolutifs (CNN) pour la classification d'images à l'aide du jeu de données CIFAR10. Le projet est implémenté en utilisant TensorFlow et Keras, et il est structuré dans un notebook Jupyter.

## Objectif

L'objectif de ce projet est de construire et d'entraîner un modèle de réseau de neurones convolutif (CNN) pour classer les images du jeu de données CIFAR10. Le jeu de données CIFAR10 contient 60 000 images en couleur de 32x32 pixels, réparties en 10 classes différentes (avion, automobile, oiseau, chat, cerf, chien, grenouille, cheval, bateau, camion).

## Structure du projet

Le projet est structuré en plusieurs étapes :

1. **Importation des packages** : Importation des bibliothèques nécessaires telles que TensorFlow, Keras, NumPy, et Matplotlib.
2. **Chargement et exploration des données** : Chargement du jeu de données CIFAR10 et exploration des dimensions des ensembles d'entraînement et de test.
3. **Prétraitement des données** : Normalisation des pixels entre 0 et 1 et conversion des étiquettes en représentation one-hot.
4. **Construction du modèle** : Création d'un modèle CNN simple avec des couches convolutives, de pooling, et des couches fully connected.
5. **Affichage des images** : Visualisation de quelques images du jeu de données avec leurs étiquettes correspondantes.
6. **Entraînement du modèle** : Compilation et entraînement du modèle sur les données d'entraînement.
7. **Évaluation du modèle** : Évaluation des performances du modèle sur les données de test.

## Détails du modèle

Le modèle CNN utilisé dans ce projet est composé des couches suivantes :

- **Couche Conv2D** : Une couche convolutive avec 64 filtres de taille 3x3.
- **Couche MaxPooling2D** : Une couche de pooling pour réduire la dimension spatiale des caractéristiques.
- **Couche Conv2D** : Une deuxième couche convolutive avec 64 filtres de taille 3x3.
- **Couche MaxPooling2D** : Une deuxième couche de pooling.
- **Couche Flatten** : Une couche pour aplatir les caractéristiques en un vecteur.
- **Couche Dense** : Une couche fully connected avec 64 neurones.
- **Couche Dense** : Une couche de sortie avec 10 neurones (un par classe) et une activation softmax.

## Utilisation

Pour exécuter ce projet, vous aurez besoin des bibliothèques suivantes :

- TensorFlow
- Keras
- NumPy
- Matplotlib

Vous pouvez installer ces bibliothèques en utilisant pip :

```bash
pip install tensorflow numpy matplotlib
```

Une fois les bibliothèques installées, vous pouvez exécuter le notebook Jupyter pour entraîner et évaluer le modèle.

## Résultats

Les résultats de l'entraînement et de l'évaluation du modèle seront affichés dans le notebook. Vous pourrez visualiser les performances du modèle en termes de précision et de perte sur les ensembles d'entraînement et de test.

## Améliorations possibles

- **Augmentation des données** : Utiliser des techniques d'augmentation des données pour améliorer la généralisation du modèle.
- **Architectures plus complexes** : Expérimenter avec des architectures de réseaux de neurones plus complexes comme ResNet ou VGG.
- **Réglage des hyperparamètres** : Effectuer une recherche d'hyperparamètres pour optimiser les performances du modèle.

## Conclusion

Ce projet fournit une introduction à l'utilisation des réseaux de neurones convolutifs pour la classification d'images avec TensorFlow et Keras. Il peut servir de point de départ pour des projets plus complexes impliquant des modèles de deep learning.
