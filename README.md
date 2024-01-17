# Projet 6 OpenClassrooms Data Scientist : Classifiez automatiquement des biens de consommation
## Créé par Agnès Regaud
## Sujet
Vous êtes Data Scientist au sein de l’entreprise "Place de marché”, qui souhaite lancer une marketplace e-commerce.
Sur la "place de marché", des vendeurs proposent des articles à des acheteurs en postant une photo et une description.

Pour l'instant, l'attribution de la catégorie d'un article est effectuée manuellement par les vendeurs, et est donc peu fiable. De plus, le volume des articles est pour l’instant très petit.

Pour rendre l’expérience utilisateur des vendeurs (faciliter la mise en ligne de nouveaux articles) et des acheteurs (faciliter la recherche de produits) la plus fluide possible, et dans l'optique d'un passage à l'échelle, il devient nécessaire d'automatiser cette tâche.

Linda, Lead Data Scientist, vous demande donc d'étudier la faisabilité d'un moteur de classification des articles en différentes catégories, avec un niveau de précision suffisant.

La première mission est de réaliser, une étude de faisabilité d'un moteur de classification d'articles, basé sur une image et une description, pour l'automatisation de l'attribution de la catégorie de l'article.

La 2ème mission est de réaliser une classification supervisée à partir des images ? Je souhaiterais que tu mettes en place une data augmentation afin d’optimiser le modèle.

Enfin, l'entreprise souhaite élargir sa gamme de produits, en particulier dans l’épicerie fine. Il faut donc tester la collecte de produits à base de “champagne” via une API fournie en fournissant une extraction de 10 produits dans un fichier csv contenant pour chaque produit les données suivantes : foodId, label, category, foodContentsLabel, image.

## Objectifs du projet :
- Prétraitement données textes (nettoyage, tokeniser, stemmer, lemmatiser)
- Construction de features : bag-of-words, Tf-idf, Word2Vec, BERT, USE
- Prétraitement données images
- Extraction de features : bag-of-images, avec Transfert Learning CNN et train/test split
- Data augmentation afin d’optimiser le modèle
- Comparaison des modèles d’apprentissage profond avec métrique et optimisation d’hyper-paramètre : fonction loss par exemple
- Maîtrise de l’overfitting
-  ACP
-  t-SNE afin de projeter les produits sur un graphique 2D
-  Analyse du graphique afin d’en déduire ou pas, à l’aide des descriptions ou des images, la faisabilité de regrouper automatiquement des produits de même catégorie
-  Réalisation d’une mesure pour confirmer ton analyse visuelle, en calculant la similarité entre les catégories réelles et les catégories issues d’une segmentation en clusters
-  Collecte de produits venant d'une API pour augmenter le nombre d'images servant à l'entraînement du modèle
-  Vérification de la propriété intellectuelle textes et images

## Compétences évaluées:
- Prétraiter des données textes pour obtenir un jeu de données exploitable
- Prétraiter des données images pour obtenir un jeu de données exploitable
- Mettre en œuvre des techniques de réduction de dimension
- Représenter graphiquement des données à grandes dimensions
- Définir la stratégie de collecte de données en recensant les API disponibles, et réaliser la collecte des données répondant à des critères définis via une API (interface de programmation) en prenant en compte les normes RGPD, afin de les exploiter pour l’élaboration d’un modèle
- Définir la stratégie d’élaboration d’un modèle d'apprentissage profond, concevoir ou ré-utiliser des modèles pré-entraînés (transfer learning) et entraîner des modèles afin de réaliser une analyse prédictive
- Évaluer la performance des modèles d’apprentissage profond selon différents critères (scores, temps d'entraînement, etc.) afin de choisir le modèle le plus performant pour la problématique métier
- Utiliser des techniques d’augmentation des données afin d'améliorer la performance des modèles
