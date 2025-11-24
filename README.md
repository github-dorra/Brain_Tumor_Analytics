# Brain_Tumor_Analytics
🧠 Classification de Tumeurs Cérébrales par Transfer Learning (VGG16) Vue d'ensemble du Projet Ce dépôt contient l'implémentation complète d'un modèle de Deep Learning destiné à la classification assistée de tumeurs cérébrales à partir d'images IRM.

1. Classification Multi-classe
L'objectif principal est de classifier chaque image IRM dans l'une des quatre catégories suivantes :

no_tumor (Pas de tumeur)

glioma_tumor

meningioma_tumor

pituitary_tumor

2. Transfer Learning (VGG16)
La méthodologie repose sur le Transfer Learning en utilisant l'architecture VGG16, pré-entraînée sur le vaste jeu de données ImageNet.

Pourquoi VGG16 ? Pour bénéficier des poids appris sur des millions d'images, permettant au modèle de reconnaître les caractéristiques générales (bords, textures, formes) avant de se concentrer sur les spécificités des tumeurs.

Fine-Tuning : Une approche avancée est utilisée où seules les dernières couches convolutionnelles de VGG16 sont dégelées et entraînées, combinée à un taux d'apprentissage très bas, afin d'adapter les caractéristiques générales aux caractéristiques médicales sans perdre les connaissances initiales.

<img width="1432" height="590" alt="image" src="https://github.com/user-attachments/assets/e3242208-efbb-4d62-b253-6fac891417b5" />

