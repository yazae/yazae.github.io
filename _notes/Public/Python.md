---
title : Python
notetype : feed
date : 24-03-2022
---
Python 10.3 - Initiation avec Mon cours visuel de programmation de Sean McManus, 2020  

## Index  
<!-- TOC titleSize:2 tabSpaces:2 depthFrom:1 depthTo:3 withLinks:1 updateOnSave:1 orderedList:0 skip:1 title:0 charForUnorderedList:* -->
* [To do](#to-do)
* [Getting started](#getting-started)
* [Spécificités](#spécificités)
  * [Divers](#divers)
  * [Opérateurs logiques et booléens](#opérateurs-logiques-et-booléens)
* [Commandes intégrées](#commandes-intégrées)
<!-- /TOC -->

## To do  

- bases python à saisir (en cours)
  - Opérateurs logiques
- Remplir la partie spécificités (en cours)

## Getting started
On utilise la console Idle, installée en même temps que Python. Elle sers à tester le code si il tiens sur peu de lignes. Pour de vrais scripts, on créera un fichier en .py.

## Spécificités  

### Divers
- Commentaires avec `#` : `#Ceci est un commentaire en python`  
  > Il est possible de faire un commentaire sur plusieurs lignes en déclarant une chaine de charactères non liée à une variable, mais autant utiliser # à chaque fois, c'est peu coûteux.  

- Opérateurs arithmétiques : `+` `-` `*` `/`
> Exemple :
```py
    prix = 8 + (5 - 6)
    taxe = prix * (20/100)
    print(taxe)
1.4000000000000001

```  

- Listes : entre crochet, séparé par des virgules
> Exemple :
```py
    ma_liste = [1, "deux", 3, 5, 7.4]
    ma_liste
[1, 'deux', 3, 5, 7.4]
    ma_liste[3] #pour appeller un seul élément
5 #[3] est le 4ème élément de la liste, le premier est [0]
```

### Opérateurs logiques et booléens
- Opérateurs logiques :
  * `<`   Plus petit que
  * `>`   Plus grand que
  * `==`  Égal à
  * `!=`  Différent de  

Une comparaison qui utilise des opérateurs logiques est appelée expression booléenne. Le résultat est une valeur booléenne (true / false).  

---

- Opérateurs booléens :

  * `and` ex : `x == 2 and y == 3` Les deux expressions doivent être vraies pour renvoyer true.  

  * `or`  ex : `x > 2 or y == 3` Une des deux expression doit être vraie pour renvoyer true.  

  * `not` ex : `not(y == 3)` Renvoie false si l'expression est true, true si l'expression est false.


## Commandes intégrées  

- ### `print()`  
```py
print() #Permet d'afficher un résultat, le contenu d'une variable, etc.
```  
> Exemple :  
```py
   num = 4
   print(num)
4
```  

- ### `input`  
```py
input #variable de base
```  
> Exemple :  
```py
   input = 5
   print(input)
5
```  

- ### `str()`  et `int()`
```py
str() #fonction qui convertis le contenu en chaine de caractères (string)
int() #fonction qui convertis le contenu en nombre entier (integer ?)
```  
> Exemple :  
```py
    input = 5
    name = "Vincent"
    concat = name + str(input)
    print(concat)
Vincent5
```  

- ### `len()`  
```py
len() #fonction qui donne le nombre de caractères d'une chaine de caractères (string)
```  
> Exemple :  
```py
   len("Hello World")
11
```  


-----

Édité le 24-03-22.  
Tags : Code, Python, Apprentissage
