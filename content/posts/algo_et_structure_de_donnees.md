+++
title = "2 - Algorithmique et structures de données: Fondamentaux et Applications"
description = "article about algorithmic"
date = "2023-07-28"
author = "Kitano Bjorgssen"
enableComments = true
+++

# Algorithmique et structures de données: Fondamentaux et Applications

La résolution de problèmes est l'essence même de la programmation. Qu'il s'agisse de créer une nouvelle fonctionnalité, d'optimiser une routine existante ou de déboguer un code énigmatique, chaque défi auquel un ingénieur logiciel est confronté peut être considéré comme un problème à résoudre. Comment y parvenons-nous de manière efficace et élégante ? Deux des outils les plus précieux dans l'arsenal d'un ingénieur sont l'algorithmique et les structures de données.

## Qu'est-ce que l'Algorithmique ?

L'algorithmique est l'étude des procédures étape par étape pour résoudre des problèmes ou accomplir des tâches. C'est un domaine fondamental en informatique qui sous-tend tout, du tri des données à la recherche d'informations, en passant par la réalisation de calculs complexes.

## L’algorithmique comme une méthode de résolution de problèmes

L'algorithmique est bien plus qu'un simple ensemble de règles à suivre pour résoudre un problème. C'est une discipline qui nécessite de l'expérience et de la pratique pour être maîtrisée. Dans cette section, nous allons discuter de l'importance de l'algorithmique et de la manière dont elle peut aider à décomposer les problèmes en sous-problèmes gérables.

## Reconnaissance des schémas de résolution

La reconnaissance des schémas de résolution est une compétence précieuse en programmation. Pourquoi ? Parce que bien souvent, les problèmes auxquels nous sommes confrontés ne sont pas uniques. Ils peuvent partager des éléments communs, des schémas que nous pouvons reconnaître et utiliser à notre avantage pour résoudre efficacement le problème.

Par exemple, considérez le problème de la recherche d'un élément dans une liste non triée. L'approche brute consisterait à vérifier chaque élément un par un jusqu'à ce que vous trouviez l'élément recherché ou que vous ayez épuisé la liste. C'est ce que nous appelons une recherche linéaire. Mais supposez maintenant que la liste est triée. Pouvez-vous reconnaître un schéma qui vous permettrait de résoudre le problème plus rapidement ? En effet, nous pourrions appliquer la recherche binaire, un algorithme qui coupe la liste en deux à chaque itération, réduisant ainsi considérablement le temps de recherche.

Ce n'est qu'un exemple, mais il illustre le pouvoir de la reconnaissance des schémas en algorithmique. En reconnaissant les schémas dans les problèmes, nous pouvons appliquer des solutions éprouvées qui nous permettent de résoudre les problèmes de manière plus efficace.

## Découpage des problèmes en sous-problèmes

Un autre avantage important de l'algorithmique est sa capacité à décomposer les problèmes en sous-problèmes plus gérables. C'est une approche qui est souvent utilisée dans la technique de programmation appelée "diviser pour régner".

Prenons l'exemple du tri d'une liste d'éléments. Le tri est un problème complexe, mais nous pouvons le décomposer en sous-problèmes plus petits, chacun concernant le tri d'une partie de la liste. Ces sous-problèmes sont plus faciles à gérer et à résoudre. Une fois que nous avons trié chaque sous-liste, nous pouvons les fusionner pour obtenir la liste triée complète.

Il s'agit là de l'idée de base derrière l'algorithme de tri par fusion, qui est un exemple classique de la technique de "diviser pour régner". En décomposant le problème en sous-problèmes, nous pouvons rendre le problème global plus gérable et plus facile à résoudre.

## L'importance des structures de données

Nous ne pouvons pas discuter de l'algorithmique sans parler des structures de données. Les structures de données sont au cœur de la programmation. Elles sont les conteneurs dans lesquels nous stockons nos données. Mais plus important encore, la structure de données que nous choisissons peut avoir un impact significatif sur la performance de nos algorithmes.

Connaître les structures de données en détail
Les structures de données sont conçues pour organiser les données de manière à faciliter certaines opérations. Par exemple, un tableau (Array) est conçu pour faciliter l'accès aux éléments par leur indice. Une LinkedList facilite l'ajout et la suppression d'éléments en début et en fin de liste. Un arbre binaire de recherche (Binary Search Tree) facilite la recherche d'éléments.

Chaque structure de données a ses avantages et ses inconvénients, et comprendre ces détails est crucial pour choisir la structure de données la plus appropriée pour un problème donné.

## Faire le lien avec la science informatique

Les structures de données ne sont pas seulement utiles pour résoudre des problèmes, elles sont aussi étroitement liées à de nombreux aspects de la science informatique. Par exemple, la manière dont les tableaux sont implémentés a un impact direct sur la manière dont la mémoire est gérée. Un tableau est une structure de données contiguë, ce qui signifie que ses éléments sont stockés côte à côte dans la mémoire. Cette connaissance peut être importante lorsque nous avons à résoudre des problèmes qui nécessitent une gestion efficace de la mémoire.

Pour conclure cette section, il est important de noter que la connaissance de l'algorithmique et des structures de données ne vient pas du jour au lendemain. Il faut de la pratique, beaucoup de pratique. Mais avec le temps, vous développerez une intuition qui vous permettra de reconnaître les schémas, de décomposer les problèmes en sous-problèmes et de choisir la structure de données la plus appropriée pour votre problème.

## Reprise du plan d'apprentissage 

Comme nous l'avons vu dans l'intro, je vais focaliser mon apprentissage sur ces différentes structures de données. Ce sont celles les plus fréquemments rencontrées dans les tests techniques et les plus utiles à la résolution de problèmes.

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

## Démystifier l'Algorithmique 

Pour beaucoup, l'algorithmique semble être une discipline réservée aux experts et aux mathématiciens. En réalité, l'algorithmique est une compétence accessible à tous, qui repose sur une idée simple : diviser un problème complexe en sous-problèmes plus simples à résoudre. 

Prenons un exemple simple : le tri d'une liste de nombres. Ce problème peut sembler déroutant si vous le considérez dans son ensemble. Cependant, en le décomposant en sous-problèmes plus simples (par exemple, en trouvant le plus petit nombre, en le plaçant au début de la liste, puis en répétant l'opération pour le reste de la liste), il devient plus gérable. C'est là que réside l'essence de l'algorithmique : décomposer les problèmes et trouver des solutions pas à pas.

En outre, l'algorithmique n'est pas qu'une question de résolution de problèmes, mais aussi de reconnaissance de schémas. Plus vous résolvez de problèmes, plus vous êtes susceptible de reconnaître des schémas récurrents. Vous commencerez à remarquer que de nombreux problèmes, bien que différents en surface, partagent des structures communes qui peuvent être résolues avec des approches similaires. Ces "patterns" de résolution de problèmes peuvent grandement accélérer votre processus de résolution de problèmes.

## L'importance des Structures de Données

Aucun ingénieur logiciel ne peut prétendre maîtriser l'algorithmique sans avoir une bonne compréhension des structures de données. Les structures de données sont le fondement sur lequel nous construisons nos algorithmes. Sans une connaissance approfondie de leur fonctionnement, leur utilisation et leurs avantages et inconvénients, il serait difficile d'utiliser efficacement les algorithmes.

Prenons l'exemple des LinkedLists. Une LinkedList est une structure de données dans laquelle les éléments sont liés par des pointeurs, chaque élément pointant vers le suivant. Cette structure de données présente des avantages, comme l'insertion et la suppression efficaces d'éléments, mais elle a aussi des inconvénients, comme l'accès inefficace aux éléments par leur indice. Connaître ces détails peut avoir un impact significatif sur l'efficacité de vos algorithmes.

## Faire le lien avec la Computer Science

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

def quick_sort(liste):
    if len(liste) <= 1:
        return liste
    else:
        pivot = liste[0]
        lesser = [x for x in liste[1:] if x <= pivot]
        greater = [x for x in liste[1:] if x > pivot]
        return quick_sort(lesser) + [pivot] + quick_sort(greater)

Cet algorithme a une complexité temporelle moyenne de O(n log n), ce qui signifie que le temps d'exécution augmente logarithmiquement avec la taille de la liste. Cela en fait un algorithme beaucoup plus efficace pour trier de grandes listes.

Cet exemple illustre comment une compréhension approfondie de l'algorithmique et des structures de données peut aider à résoudre des problèmes de manière plus efficace. En continuant à apprendre et à pratiquer, vous pourrez améliorer vos compétences en algorithmique et en structures de données, et devenir un meilleur ingénieur logiciel.


## Conclusion

En résumé, l'algorithmique et les structures de données sont des sujets vastes et profonds qui sont au cœur de la computer science. L'apprentissage de ces compétences est un voyage passionnant qui vous aidera non seulement à devenir un meilleur ingénieur logiciel, mais aussi à développer une compréhension plus profonde de l'informatique en général. 

