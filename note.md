# TP3

## INTERPRETATION DES RESULTATS


L'inertie (Inertia) et le score Davies Bouldin sont deux métriques utilisées pour évaluer la performance d'un algorithme de clustering, comme le K-Means.

Inertie (Inertia): L'inertie mesure la somme des carrés des distances entre chaque point de données et le centre de son cluster assigné. Une inertie plus faible indique que les points à l'intérieur du cluster sont plus proches les uns des autres, ce qui est généralement souhaitable. Cependant, il n'indique pas la qualité globale des clusters.

Score Davies Bouldin: Le score Davies Bouldin mesure la compacité et la séparation des clusters. Un score plus bas indique une meilleure séparation entre les clusters et une meilleure compacité des points à l'intérieur de chaque cluster.

Interprétation des résultats pour votre exécution :

Inertie: L'inertie est de 487739.66. Cela signifie que la somme des carrés des distances entre les points et les centres de cluster est relativement élevée. Une valeur d'inertie plus basse serait préférable, mais la qualité des clusters dépend également de la distribution réelle des données.

Score Davies Bouldin: Le score est de 2.72. Un score Davies Bouldin plus bas est généralement souhaitable. Cependant, la qualité dépend du contexte spécifique de vos données. En général, si le score est proche de zéro, cela indique une meilleure séparation entre les clusters.

# Rapport sur le TP : Classification de Fruits avec K-Means

## Introduction
Le présent TP vise à explorer l'application de l'algorithme K-Means pour la classification d'images de fruits. Nous avons suivi des étapes allant du téléchargement du jeu de données au prétraitement des images, à l'augmentation du jeu de données, à l'application de K-Means pour regrouper les fruits en clusters, et enfin, à l'évaluation de la qualité de la classification.

## Étape 1 : Téléchargement du jeu de données
Nous avons téléchargé l'ensemble de données "fruits.zip" et l'avons extrait localement. Cet ensemble de données contient des images de fruits dans différentes catégories.

## Étape 2 : Chargement des images
Un script Python utilise la bibliothèque Pillow pour charger les images du jeu de données dans un format adapté à scikit-learn, sous forme de matrices de pixels.

## Étape 3 : Prétraitement des images
Afin de simplifier le processus, toutes les images ont été redimensionnées à une taille fixe de 100x100 pixels, et les valeurs des pixels ont été normalisées.

## Étape 4 : Augmentation du jeu de données
Des techniques d'augmentation de données ont été appliquées pour générer de nouvelles variations des images. Cela inclut des transformations telles que la rotation, le changement d'échelle, le recadrage et le changement de luminosité.

## Étape 5 : Application de K-Means
L'algorithme K-Means a été appliqué sur les images prétraitées et augmentées pour regrouper les fruits en clusters. Nous avons choisi un nombre approprié de clusters (10 dans notre cas) et expérimenté avec différentes valeurs.


L'algorithme K-Means est une technique de clustering largement utilisée en apprentissage non supervisé. Son objectif principal est de regrouper des données similaires dans des ensembles appelés "clusters". Voici les principaux objectifs et applications de l'algorithme K-Means :

1. **Clustering :** L'objectif principal de K-Means est de diviser un ensemble de données en groupes homogènes appelés clusters. Chaque cluster est caractérisé par un "centroid" représentatif, qui est le centre géométrique du groupe.

2. **Segmentation de données :** K-Means est souvent utilisé pour segmenter un ensemble de données en groupes distincts en fonction de caractéristiques similaires. Par exemple, dans le domaine du marketing, il peut être utilisé pour segmenter les clients en groupes ayant des comportements d'achat similaires.

3. **Réduction de dimension :** K-Means peut également être utilisé comme technique de réduction de dimension en attribuant à chaque donnée un label correspondant à son cluster. Cela peut être utile pour simplifier les données et accélérer les calculs ultérieurs.

4. **Détection d'anomalies :** En observant la distribution des données, les anomalies peuvent souvent être identifiées comme des points qui ne s'alignent pas bien avec les clusters existants.

5. **Compression d'image :** Dans le traitement d'image, K-Means peut être utilisé pour compresser une image en réduisant le nombre de couleurs tout en préservant les caractéristiques visuelles essentielles.

6. **Initialisation d'autres algorithmes :** Les résultats de K-Means peuvent servir d'initialisation pour d'autres algorithmes d'apprentissage automatique, améliorant ainsi leur efficacité.

Le fonctionnement de l'algorithme K-Means consiste à minimiser la somme des carrés des distances entre chaque point de données et le centroïde du cluster auquel il est assigné. Il alterne entre l'affectation des points au cluster le plus proche et la mise à jour des centroïdes en fonction des points assignés. Cette itération se poursuit jusqu'à ce que les affectations des points aux clusters ne changent plus significativement.

## Étape 6 : Visualisation des clusters
Matplotlib a été utilisé pour afficher quelques images de chaque cluster, permettant ainsi une évaluation visuelle de la qualité de la classification.

## Étape 7 : Évaluation de la classification
L'évaluation de la classification s'est faite en utilisant l'inertie, qui mesure la cohésion des clusters. Plus l'inertie est faible, plus les clusters sont cohérents. Nous avons également utilisé le score de Davies-Bouldin pour évaluer la séparation entre les clusters.

## Résultats et Conclusions
L'inertie obtenue fournit une indication de la qualité de la classification. Cependant, d'autres évaluations telles que la visualisation des clusters et le score de Davies-Bouldin peuvent fournir des informations complémentaires sur la cohérence et la séparation des clusters.

Le code fourni accomplit les tâches spécifiées, et les résultats obtenus peuvent être analysés pour affiner la qualité de la classification. En répétant ces étapes avec un deuxième jeu de données ("fruits-vegetables.zip"), il est possible d'étendre l'analyse à un ensemble plus diversifié de fruits et légumes.


