---
title : Problèmes bluetooth sur Ubuntu
notetype : feed
date : 24-03-2022
---

Problème de bluetooth sur Ubuntu 20.04.4 LTS résolu par [cette marche à suivre](https://askubuntu.com/questions/1231074/ubuntu-20-04-bluetooth-not-working "Ask Ubuntu : Ubuntu 20-04 bluetooth not working"){:target="_blank"} :

```
sudo apt install blueman

sudo add-apt-repository ppa:blaze/rtbth-dkms
sudo apt-get update
sudo apt-get install rtbth-dkms
```  


``sudo vim /etc/modules``

Commenter tout et ajouter cette ligne :

``rtbth``

Reboot et ouvrir :

``sudo blueman-manager``

> It worked !!

En fait, ça ouvre blueman, un utilitaire bluetooth plus performant que celui natif à Ubuntu!

-----

Édité le 24-03-22.   
Tags : Libre, FOSS, Linux, Ubuntu, Bug
