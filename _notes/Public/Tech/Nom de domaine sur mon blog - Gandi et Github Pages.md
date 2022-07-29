---
title : Nom de domaine sur mon blog - Gandi et Github Pages
notetype : feed
date : 26-07-2022
---
Je vais mettre ici mes notes sur la mise en place du nom de domaine sur mon blog. Je me suis rendu compte que c'était pas si facile de trouver les infos et savoir quoi faire, donc après pas mal d'essais et d'erreur, ça me semble intéressant de mettre la procédure ici :)

J'utilise Jekyll via Github Pages, et Gandi comme fournisseur de nom de domaine.

## Index
<!-- TOC titleSize:2 tabSpaces:2 depthFrom:1 depthTo:3 withLinks:1 updateOnSave:1 orderedList:0 skip:1 title:0 charForUnorderedList:* -->
* [A - Enregistrement du nom de domaine sur Gandi](#a---enregistrement-du-nom-de-domaine-sur-gandi)
* [B - Paramétrage du nom de domaine](#b---paramétrage-du-nom-de-domaine)
* [C - Paramétrage de Github Pages](#c---paramétrage-de-github-pages)
<!-- /TOC -->

## A - Enregistrement du nom de domaine sur Gandi
1. Aller sur [le shop de Gandi](https://shop.gandi.net/fr/5d1cd542-ab7f-11ec-8372-00163e816020/domain/suggest) pour les noms de domaines
2. Choisir son nom de domaine et l'acheter (pour un an minimum)

## B - Paramétrage du nom de domaine
1. Aller sur nom de domaine sur l'espace client de Gandi
2. Onglet "Enregistrement DNS"
3. On va créer une redirection Ipv4 (A) et ipv6 (AAAA) vers les adresses ip listées dans
	- Création de la redirection ipv4  
	<img src="../assets/img/tutoDNS/screen-DNS-A.jpg" alt="Screen de l'interface Gandi pour l'ajout de la redirection DNS A" width="90%"/>
	- Création de la redirection ipv6  
	<img src="../assets/img/tutoDNS/screen-DNS-AAAA.jpg" alt="Screen de l'interface Gandi pour l'ajout de la redirection DNS AAAA" width="90%"/>
1. Supprimer l'adresse ip déjà enregistrée
<img src="../assets/img/tutoDNS/screen-liste-DNS.jpg" alt="Screen de l'interface Gandi listant les enregistrements DNS. La première ligne AAAA est barrée." width="100%"/>  
5. Créer une redirection CNAME vers `nom-de-compte.github.io.` (ne pas oublier le . à la fin !)
<img src="../assets/img/tutoDNS/screen-DNS-CNAME.jpg" alt="Screen de l'interface Gandi pour l'ajout de la redirection DNS CNAME" width="90%"/>

## C - Paramétrage de Github Pages
1. Aller sur votre projet Github contenant votre site Jekyll
2. Onglet Settings, section Pages
3. Activer Github Pages en selectionnant la source (branche) du site.
4. Custom domain : entrer votre nom de domaine (sans le www.)
5. Attendez que Github vérifie les DNS et génère un certificat TLS
<img src="../assets/img/tutoDNS/screen-github-pages.jpg" alt="Screen de l'interface Github Pages pour activer" width="100%"/>
6. Si les étapes précédentes ont été suivies correctement, on devrait pouvoir activer "Enforce HTTPS" et accéder correctement à notre site Jekyll depuis l'adresse du nom de domaine ! Bravo :)

-----
Édité le 26-07-22.  
Tags : Tech, Tuto
