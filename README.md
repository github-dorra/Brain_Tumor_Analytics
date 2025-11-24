# Brain_Tumor_Analytics

**🧠 Diagnostic , Classification et Segmentation des Tumeurs Cérébrales par Transfer Learning (VGG16)**

l'implémentation complète d'un modèle de Deep Learning destiné à la classification assistée de tumeurs cérébrales à partir d'images IRM.

**1. Classification Multi-classe**
L'objectif principal est de classifier chaque image IRM dans l'une des quatre catégories suivantes :

no_tumor (Pas de tumeur)

glioma_tumor

meningioma_tumor

pituitary_tumor

<img width="1000" height="550" alt="image" src="https://github.com/user-attachments/assets/aad79bb6-5b61-405d-aa4c-c9ce39b882d6" />


**2. Transfer Learning (VGG16)**
La méthodologie repose sur le Transfer Learning en utilisant l'architecture VGG16, pré-entraînée sur le vaste jeu de données ImageNet.

Pourquoi VGG16 ? Pour bénéficier des poids appris sur des millions d'images, permettant au modèle de reconnaître les caractéristiques générales (bords, textures, formes) avant de se concentrer sur les spécificités des tumeurs.

Fine-Tuning : Une approche avancée est utilisée où seules les dernières couches convolutionnelles de VGG16 sont dégelées et entraînées, combinée à un taux d'apprentissage très bas, afin d'adapter les caractéristiques générales aux caractéristiques médicales sans perdre les connaissances initiales.

<img width="1000" height="550" alt="image" src="https://github.com/user-attachments/assets/e3242208-efbb-4d62-b253-6fac891417b5" />

**3. Segmentation de Tumeur**
Délimiter précisément les frontières et la localisation de la tumeur sur l'image.
Utilisation d'une architecture optimisée (souvent basée sur l'idée Encoder-Decoder) pour générer un masque binaire (ou multiclasse) de la tumeur, montrant la localisation précise en pixels.

<img width="1000" height="602" alt="image" src="https://github.com/user-attachments/assets/142381b1-d839-42ff-b4ea-9d14e612e901" />

