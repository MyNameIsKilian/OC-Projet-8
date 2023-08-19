# OC - Projet 8 - Parcours Data Scientist

### 🚀 Objectif

Vous êtes Data Scientist dans une très jeune start-up de l'AgriTech, nommée  "Fruits!", qui cherche à proposer des solutions innovantes pour la récolte des fruits.
La volonté de l’entreprise est de préserver la biodiversité des fruits en permettant des traitements spécifiques pour chaque espèce de fruits en développant des robots cueilleurs intelligents.

Fruits souhaite dans un premier temps se faire connaître en mettant à disposition du grand public une application mobile qui permettrait aux utilisateurs de prendre en photo un fruit et d'obtenir des informations sur ce fruit.

Pour la start-up, cette application permettrait de sensibiliser le grand public à la biodiversité des fruits et de mettre en place une première version du moteur de classification des images de fruits.

De plus, le développement de l’application mobile permettra de construire une première version de l'architecture Big Data nécessaire.

### ❗️Contraintes

Je dois tenir compte dans mes développements du fait que le volume de données va augmenter très rapidement après la livraison de ce projet. Je dois continuer à développer des scripts en Pyspark et à utiliser le cloud AWS pour profiter d’une architecture Big Data (EMR, S3, IAM).
Vous devez faire une démonstration de la mise en place d’une instance EMR opérationnelle, ainsi qu’ expliquer pas à pas le script PySpark, que vous aurez complété : 
- d’un traitement de diffusion des poids du modèle Tensorflow sur les clusters (broadcast des “weights” du modèle) qui avait été oublié par l’alternant. Vous pourrez vous appuyer sur l’article “Distributed model inference using TensorFlow Keras” disponible dans les ressources
- d’une étape de réduction de dimension de type PCA en PySpark 
  
Je dois respecter les contraintes du RGPD : dans notre contexte, je veille à paramétrer mon installation afin d’utiliser des serveurs situés sur le territoire européen 


### 💾 Dataset

Le jeu de données utilisé provient de Kaggle : [Fruits](https://www.kaggle.com/moltean/fruits)

### 📁 Découpage des dossiers
------------

    ├── data                <- Images + features des images au format parquet
    │
    ├── images-cours        <- Images utilisées dans le notebbok local
    │
    ├── notebooks           <- Notebooks local/cloud 
    │
    ├── bootstrap-emr.sh    <- Fichier action d'amorçage pour cluster EMR
    │
    ├── links               <- Liens de téléchargement des données
    │
    ├── presentation        <- Support de présentation du projet
    |
    ├── README.md

    

### 🧰 Outils

- Python
- Pyspark
- TensorFlow
- AWS