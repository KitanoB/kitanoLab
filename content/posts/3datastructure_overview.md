+++
title = "3 - Data Structures Overview"
description = "article about data structures in computer science"
date = "2023-07-29"
author = "Kitano B"
+++

## Reprise du plan d'apprentissage 

Comme nous l'avons vu dans les posts précédents, je vais focaliser mon apprentissage sur ces différentes structures de données. Ce sont celles les plus fréquemments rencontrées dans les tests techniques et les plus utiles à la résolution de problèmes.

#### Arrays 

Une structure de données linéaire qui stocke une collection d'éléments dans un ordre donné. Les arrays sont simples, mais essentielles dans presque tous les programmes informatiques.

#### LinkedList 

Une structure de données linéaire où chaque élément pointe vers le prochain élément de la liste. Les LinkedList sont utiles lorsque les insertions et suppressions fréquentes sont nécessaires.

#### Stacks (Piles) et Queues (Files)

Ces structures de données sont utilisées pour gérer les éléments de manière LIFO (Last In First Out) pour les stacks et FIFO (First In First Out) pour les queues. Elles sont utiles dans de nombreux algorithmes et problèmes de programmation.

#### Trees et Graphs

Les trees et les graphs sont des structures de données non linéaires qui permettent de représenter des relations hiérarchiques et des réseaux complexes.

#### Hashmap 

Une structure de données qui utilise une fonction de hachage pour mapper des clés à des valeurs. Les Hashmaps sont extrêmement efficaces pour la recherche, l'insertion et la suppression d'éléments.

#### Set 

Une structure de données qui stocke des éléments uniques dans un ordre non spécifique. Les sets sont utilisés lorsque la présence d'un élément dans une collection est plus importante que l'ordre ou la fréquence.

## L'importance des Structures de Données

Aucun sofware developer ne peut prétendre maîtriser l'algorithmique sans avoir une bonne compréhension des structures de données. Les structures de données sont le fondement sur lequel nous construisons nos algorithmes. Sans une connaissance approfondie de leur fonctionnement, leur utilisation et leurs avantages et inconvénients, il serait difficile d'utiliser efficacement les algorithmes.

Prenons l'exemple des LinkedLists. Une LinkedList est une structure de données dans laquelle les éléments sont liés par des pointeurs, chaque élément pointant vers le suivant. Cette structure de données présente des avantages, comme l'insertion et la suppression efficaces d'éléments, mais elle a aussi des inconvénients, comme l'accès inefficace aux éléments par leur indice. Connaître ces détails peut avoir un impact significatif sur l'efficacité de vos algorithmes.

L'algorithmique et les structures de données sont intimement liées à d'autres aspects de la computer science, comme la gestion de la mémoire. Par exemple, comprendre comment les arrays sont stockés en mémoire peut vous aider à comprendre pourquoi leur taille doit être définie à l'avance et ne peut être modifiée ultérieurement. Cela peut aussi vous aider à comprendre pourquoi l'accès à un élément d'un array par son indice est une opération de temps constant, tandis que l'accès à un élément d'une LinkedList par son indice est une opération de temps linéaire.

Il est également intéressant de noter que l'algorithmique et les structures de données ont des applications pratiques dans de nombreux domaines de la computer science, comme le machine learning, l'optimisation de requêtes dans les bases de données, la conception de systèmes de recommandation, et bien d'autres.

## Mise en Pratique : Le Tri d'une Liste

Pour illustrer comment l'algorithmique et les structures de données peuvent être utilisées en pratique, nous allons prendre un problème simple mais classique en informatique : le tri d'une liste de nombres.

### Le problème
Soit une liste de nombres non triés. Notre objectif est de trier cette liste en ordre croissant. Par exemple, si notre liste est [4, 3, 2, 1], nous voulons la transformer en [1, 2, 3, 4].

### Découpage en sous-problèmes

Une manière de résoudre ce problème est de le découper en sous-problèmes. Dans ce cas, nous pourrions dire que notre sous-problème est de trouver le plus petit nombre dans la liste, de le déplacer au début de la liste, et de répéter ce processus pour le reste de la liste.

### Solution simple : Le tri par sélection (Selection Sort)

Le tri par sélection est un algorithme simple qui suit exactement cette approche. Voici une implémentation en Python :

def selection_sort(liste):
    for i in range(len(liste)):
        min_index = i
        for j in range(i+1, len(liste)):
            if liste[j] < liste[min_index]:
                min_index = j
        liste[i], liste[min_index] = liste[min_index], liste[i]
    return liste

Cet algorithme a une complexité temporelle de O(n²), ce qui signifie que le temps d'exécution augmente quadratiquement avec la taille de la liste. En termes simples, cela signifie que si la taille de la liste double, le temps d'exécution sera multiplié par quatre.

### Solution optimisée : Le tri rapide (Quick Sort)
Bien que le tri par sélection soit simple à comprendre et à mettre en œuvre, il n'est pas le plus efficace pour les grandes listes. Un algorithme de tri plus rapide et plus efficace est le tri rapide, ou Quick Sort. Voici une implémentation en Python :

``` python
def quick_sort(liste):
    if len(liste) <= 1:
        return liste
    else:
        pivot = liste[0]
        lesser = [x for x in liste[1:] if x <= pivot]
        greater = [x for x in liste[1:] if x > pivot]
        return quick_sort(lesser) + [pivot] + quick_sort(greater)
```

Cet algorithme a une complexité temporelle moyenne de O(n log n), ce qui signifie que le temps d'exécution augmente logarithmiquement avec la taille de la liste. Cela en fait un algorithme beaucoup plus efficace pour trier de grandes listes.

Cet exemple illustre comment une compréhension approfondie de l'algorithmique et des structures de données peut aider à résoudre des problèmes de manière plus efficace. En continuant à apprendre et à pratiquer, vous pourrez améliorer vos compétences en algorithmique et en structures de données, et devenir un meilleur ingénieur logiciel.


## Conclusion

En résumé, l'algorithmique et les structures de données sont des sujets vastes et profonds qui sont au cœur de la computer science. L'apprentissage de ces compétences est un voyage passionnant qui vous aidera non seulement à devenir un meilleur ingénieur logiciel, mais aussi à développer une compréhension plus profonde de l'informatique en général. 

