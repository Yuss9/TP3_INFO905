# TP3

## INTERPRETATION DES RESULTATS


L'inertie (Inertia) et le score Davies Bouldin sont deux métriques utilisées pour évaluer la performance d'un algorithme de clustering, comme le K-Means.

Inertie (Inertia): L'inertie mesure la somme des carrés des distances entre chaque point de données et le centre de son cluster assigné. Une inertie plus faible indique que les points à l'intérieur du cluster sont plus proches les uns des autres, ce qui est généralement souhaitable. Cependant, il n'indique pas la qualité globale des clusters.

Score Davies Bouldin: Le score Davies Bouldin mesure la compacité et la séparation des clusters. Un score plus bas indique une meilleure séparation entre les clusters et une meilleure compacité des points à l'intérieur de chaque cluster.

Interprétation des résultats pour votre exécution :

Inertie: L'inertie est de 487739.66. Cela signifie que la somme des carrés des distances entre les points et les centres de cluster est relativement élevée. Une valeur d'inertie plus basse serait préférable, mais la qualité des clusters dépend également de la distribution réelle des données.

Score Davies Bouldin: Le score est de 2.72. Un score Davies Bouldin plus bas est généralement souhaitable. Cependant, la qualité dépend du contexte spécifique de vos données. En général, si le score est proche de zéro, cela indique une meilleure séparation entre les clusters.




