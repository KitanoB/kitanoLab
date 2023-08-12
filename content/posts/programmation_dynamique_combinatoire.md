+++
title = "4 - Algorithmique et structures de données: Mon parcours d'apprentissage"
description = "article about algorithmic"
date = "2023-08-01"
author = "Kitano B"
enableComments = true
+++

# Programmation Dynamique : Une Approche Efficace pour les Problèmes de Combinatoire

## Introduction

La programmation dynamique est une technique puissante en informatique et en mathématiques, utilisée pour résoudre des problèmes qui peuvent être décomposés en sous-problèmes plus petits. La méthode repose sur le stockage de solutions à des sous-problèmes de sorte à ne pas avoir à les résoudre plusieurs fois.

## Définition de la Programmation Dynamique

La programmation dynamique consiste à décomposer un problème en une série de sous-problèmes plus simples, à résoudre ces sous-problèmes, puis à combiner ces solutions pour résoudre le problème original. Elle utilise souvent un tableau ou une autre structure de données pour stocker les solutions intermédiaires, évitant ainsi les recalculs inutiles.

## Quand Utiliser la Programmation Dynamique et Pourquoi Elle est Performante

La programmation dynamique est particulièrement utile lorsqu'il existe de nombreux chevauchements de sous-problèmes, c'est-à-dire lorsque les mêmes sous-problèmes doivent être résolus plusieurs fois. En mémorisant les résultats de ces sous-problèmes dans une structure de données, la programmation dynamique peut réduire considérablement le temps d'exécution.

L'efficacité de cette méthode peut souvent transformer un algorithme ayant une complexité exponentielle en un algorithme ayant une complexité polynomiale, ou même linéaire. Cela rend la programmation dynamique idéale pour traiter des problèmes de combinatoire, où les approches naïves peuvent rapidement devenir infaisables.

## Application Pratique : La Suite de Fibonacci

### Introduction à la Suite de Fibonacci

La suite de Fibonacci est une séquence célèbre où chaque nombre est la somme des deux précédents. Elle commence avec 0 et 1, et chaque nombre suivant est la somme des deux précédents. La séquence commence donc ainsi : 0, 1, 1, 2, 3, 5, 8, 13, etc.

### Pseudo-Code pour Calculer le n-ième Nombre de Fibonacci

Nous pouvons utiliser la programmation dynamique pour calculer le n-ième nombre de Fibonacci de manière efficace. Voici un pseudo-code pour cette tâche :

```
Fonction fibo(n) :
    Si n = 0, retourner 0
    Créer un tableau array de taille n
    array[0] = 0
    Si n > 1, array[1] = 1
    Pour i de 2 à n-1 :
        array[i] = array[i - 2] + array[i - 1]
    Retourner array[n - 1]
```

Ce code utilise un tableau pour stocker les nombres de Fibonacci calculés, réduisant ainsi la complexité temporelle de exponentielle à linéaire.

### Implémentation en Kotlin

```java
fun fibo(num: Int): Int {
    if (num == 0) return 0
    var array = IntArray(num)
    for (i in 0 until num) {
        if(i == 0 || i == 1) array[i] = i
        else array[i] = array[i - 2] + array[i - 1]
    }
    return array[num - 1]
}
```

### Implémentation en Python

Le code suivant est une traduction en Python de l'algorithme précédent, utilisant la programmation dynamique pour calculer le n-ième nombre de Fibonacci :

```python
def fibo(num):
    if num == 0:
        return 0
    array = [0] * num
    array[0] = 0
    if num > 1:
        array[1] = 1
    for i in range(2, num):
        array[i] = array[i - 2] + array[i - 1]
    return array[num - 1]
```

## Application à un Problème Combinatoire : Le Robot sur une Grille

### Problème

Un robot est situé en haut à gauche d'une grille de taille m x n. Le robot cherche à atteindre la case en bas à droite. Il peut seulement se déplacer vers le bas ou vers la droite.

Étant donnés deux entiers m et n, déterminez le nombre de chemins uniques que le robot peut prendre pour atteindre la case en bas à droite.

### Solution Utilisant la Programmation Dynamique

#### Pseudo-Code

```
Fonction uniquePaths(m, n) :
    Créer un tableau 2D dp de taille m x n
    Pour i de 0 à m-1 :
        Pour j de 0 à n-1 :
            Si i = 0 ou j = 0 :
                dp[i][j] = 1
            Sinon :
                dp[i][j] = dp[i - 1][j] + dp[i][j - 1]
    Retourner dp[m - 1][n - 1]
```

Cette solution utilise un tableau 2D pour stocker le nombre de chemins à chaque case de la grille. Chaque case est accessible à partir de la case du dessus ou de la case de gauche, d'où l'utilisation de la somme dans le code.

#### Implémentation en Kotlin

```java
fun uniquePaths(m: Int, n: Int): Int {
    val dp = Array(m) { IntArray(n) }
    for (i in 0 until m) {
        for (j in 0 until n) {
            dp[i][j] = if (i == 0 || j == 0) 1 else dp[i - 1][j] + dp[i][j - 1]
        }
    }
    return dp[m - 1][n - 1]
}
```

#### Implémentation en Python

```python
def uniquePaths(m, n):
    dp = [[0] * n for _ in range(m)]
    for i in range(m):
        for j in range(n):
            if i == 0 or j == 0:
                dp[i][j] = 1
            else:
                dp[i][j] = dp[i - 1][j] + dp[i][j - 1]
    return dp[m - 1][n - 1]
```

## Conclusion

La programmation dynamique est une technique robuste et efficace qui transforme des problèmes complexes en une série de sous-problèmes plus simples. Grâce à sa capacité à réduire la complexité temporelle, elle est idéale pour résoudre des problèmes de combinatoire et d'optimisation.

En utilisant deux exemples pratiques, la suite de Fibonacci et le problème du robot sur une grille, cet article a montré comment appliquer la programmation dynamique pour obtenir des solutions efficaces et élégantes.
