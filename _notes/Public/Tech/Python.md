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
  * [`if`, `elif`, `else`](#if-elif-else)
  * [Entrées et sorties](#entrées-et-sorties)
  * [Les boucles](#les-boucles)
* [Commandes intégrées](#commandes-intégrées)
<!-- /TOC -->

## To do  

- bases python à saisir (en cours)
  - Revoir rendu site (ajouts espaces ?)
- Remplir la partie spécificités (en cours)

## Getting started
On utilise la console Idle, installée en même temps que Python. Elle sers à tester le code si il tiens sur peu de lignes. Pour de vrais scripts, on créera un fichier en .py.

## Spécificités  

### Divers
- Commentaires avec `#` : `#Ceci est un commentaire en python`  
  > Il est possible de faire un commentaire sur plusieurs lignes en déclarant une chaine de charactères non liée à une variable, mais autant utiliser # à chaque fois, c'est peu coûteux.  

- Opérateurs arithmétiques : `+` `-` `*` `/`  

```py  
    prix = 8 + (5 - 6)
    taxe = prix * (20/100)
    print(taxe)
1.4000000000000001
```  

- Listes : entre crochet, séparé par des virgules

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

### `if`, `elif`, `else`  

```py
    quiz_score = 9
    if quiz_score > 8:
      print("Vous etes un champion !")
    elif quiz_score > 5:
      print("Vous auriez pu faire mieux !")
    else:
    print("Étiez-vous bien réveillé ?")
    Vous etes un champion !
```

> `elif` est un raccourcis pour else if  

### Entrées et sorties  

- `input` permet de demander à l’utilisateurice de saisir une donnée.

```py  
  nom = input("Saississez votre nom :")
Saississez votre nom :Alex
  print("Bonjour "+nom+" !")
Bonjour Alex !
```

### Les boucles

#### La boucle `for`  

Utilisée si l’on sait combien de fois le bloc de code sera répété.

```py  
for chrono in range (1,4): # équivalent d’une liste contenant 1-3.
    print(chrono)
else :
    print("Go !")
1
2
3
Go !
```  

#### La boucle `while`  

Utilisée si l’on ne sais pas combien de fois une boucle doit s’exécuter, à la place de la boucle `for`.  

```py
number = 1
while number <10:
    print(number)
    number = number +1 # On incrémente de 1 number pour ne pas produire une boucle infinie.
1
2
3
4
5
6
7
8
9
```  

#### Sortie de boucle  

On peut interrompre une boucle totalement avec `break`, alors que `continue` permet de "sauter" une itération et de passer à la suivante.


## Commandes intégrées  

- ### `print()`  
```py
print() #Permet d'afficher un résultat, le contenu d'une variable, etc.
```  

Exemple :  
```py
   num = 4
   print(num)
4
```  

- ### `input`  
```py
input #variable de base
```  

Exemple :  
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

Exemple :   
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

Exemple :   
```py
   len("Hello World")
11
```  


-----

Dernière édition le 02-04-22.  
Tags : Code, Python, Apprentissage
