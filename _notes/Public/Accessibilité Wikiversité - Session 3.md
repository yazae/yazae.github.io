---
title : Accessibilité Wikiversité - Session 3
notetype : unfeed
date : 14-06-2022
---
Notes sur la [troisième session](https://fr.wikiversity.org/wiki/Preparer_un_document_web_a_l_accessibilite_numerique-Notions_de_base) de la formation Accessibilité numérique de la Wikiversité.

## Index
Retour à [[Accessibilité Wikiversité - Session 2]]

<!-- TOC titleSize:2 tabSpaces:2 depthFrom:1 depthTo:3 withLinks:1 updateOnSave:1 orderedList:0 skip:1 title:0 charForUnorderedList:* -->
* [Session 3 - Publier accessible](#session-3---publier-accessible)
  * [Préparer un document web à l’accessibilité](#préparer-un-document-web-à-laccessibilité)
  * [Structurer l’information textuelle](#structurer-linformation-textuelle)
  * [Rendre accesssibles les liens](#rendre-accesssibles-les-liens)
  * [Rendre les images accessibles](#rendre-les-images-accessibles)
  * [Rendre les contenus audiovisuels accessibles](#rendre-les-contenus-audiovisuels-accessibles)
  * [Améliorer la présentation de l’information (AAA)](#améliorer-la-présentation-de-linformation-aaa)
<!-- /TOC -->

## Session 3 - Publier accessible

### Préparer un document web à l’accessibilité
Il n’y a qu’à fournir la matière première : le texte d’un site web. La structuration HTML va permettre au texte d’être adapté sur tous les supports utilisés par l’internaute.

- La langue d’un document doit être renseignée, afin que les lecteurs d’écrans puissent lire avec la bonne langue.
- Le titre (title) du document doit correctement renseigner la nature du document, c’est le premier élément qui sera lu par l’internaute.

### Structurer l’information textuelle
- Les titres doivent être déclarés avec la balise <h1>, <h2>, etc.
- Les listes, citations, tableux, etc. doivent utiliser leurs balises html.
- Les abréviations doivent être explicités, une fois au début de leur apparition. Si on manque de place, il existe une balise abbr pour renseigner la définition de l’abrev.

### Rendre accesssibles les liens
- Le titre du lien (title) (<a href="" title="">intitulé</a>) doit contenir l’intitulé du lien à l’identique, accompagné d’une info complémentaire.
- Avertir préalablement si un lien ouvre une nouvelle fenêtre.
- Dans le cas d’un téléchargement, indiquer le poids et le format dans title ou dans l’intitulé directement afin d’avertir l’utilisateurice.

### Rendre les images accessibles
- L’alternative textuelle (attribut alt) doit systématiquement être renseignée. En son absence, le lecteur de texte lis le titre de l’image, ce qui est une nuisance.
- Les images non porteuses d’information sont dites décoratives. On laisse l’attribut alt vide dans ce cas.
- L’alternative doit être courte et concise
- En cas d’images-liens, il faut renseigner le but du lien (ex : alt:nous suivre sur twitter).
- En cas d’images complexes, on saisira dans alt une courte description, le titre du graphique etc., et on devra fournir une description détaillée en parrallèle du graphique ou sur une page dédiée à cette description.

### Rendre les contenus audiovisuels accessibles
- Les vidéos doivent être accompagnés de sous-titres, idem pour les audios sans images si cela est possible.
- Une audiodescription peut être proposée en complément à une vidéo
- Une transcription textuelle peut être proposée, en terme de contenu, elle inclut le contenu des sous-titres + le contenu de l’audio-description (AA), mais ne les remplace pas (les deux sont utiles)
- La langue des signes peut-être proposée pour aider les personnes sourdes et malentendantes. Cela dépend de l’exigence d’accessibilité (AAA pour la langue des signes en plus du reste).

### Améliorer la présentation de l’information (AAA)
- Écrire sans faute (exemple : accentuation des capitales)
- Favoriser un interlignage suffisant (privilégier interlignage 150% mini)
- Ne pas dépasser 80 caractères par ligne de textes réduis les difficultés de lecture
- Éviter la justification si possible
- On doit pouvoir zoomer le texte en x2 minimum sans que ça ne casse le site (AA)
- **L’information ne doit pas reposer sur la seule couleur** (A)


----
Tous les contenus de la wikiversité sont sous license CC-BY-SA.  
Édité le 14-06-22.  
Tags : Libre, Accessibilité, Wikiversité, Wikipedia  
