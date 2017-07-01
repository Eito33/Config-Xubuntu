# Config Xubuntu
![ImageLOAD](http://i.imgur.com/4GPHrtH.png)

## SOMMAIRE : 

* Général
* Environement Graphique
* Logiciels
* Autres


------------------------------


### 1. Général

Ce dépot concerne principalement les différentes chose a mettre en place aprés un reformatage pour linux!

1. Testé sous **Xubuntu**. Il concerne également les environement **Xfce**.
2. Toutes les infos concernant l'iso se trouve [ici](http://xubuntu.fr/). (`V. 16.04LTS`)
3. Toutes les infos pour la doc se trouve [ici](https://doc.ubuntu-fr.org/).
4. Pour tous télécharger d'un coup utiliser la commande :

        git clone https://github.com/Eito33/Config-Xubuntu.git


*Mise a jour le 01/07/2017* 

### 2. Environement Graphique

#### a) Theme Arc Flatabulous
*` Nécessite l'installation de Git (sudo apt-get install git) `*

Le theme choisit est Arc-Flatabulous. Vous pouvez le télécharger a partir d'[ici](https://github.com/Eito33/Config-Xubuntu/tree/master/arc-flatabulous).
Néanmoins il se trouve par défaut dans le répository [suivant](https://github.com/andreisergiu98/arc-flatabulous-theme).

`Repository Perso :`

    git clone https://github.com/Eito33/Config-Xubuntu.git
  
 `Autres Repository :`

    git clone https://github.com/andreisergiu98/arc-flatabulous-theme
 
 
` Une fois le theme télécharger, accéder via le terminal au dossier ou il a été mis (via la commande cd).`

Puis rentrer les commandes suivante :

    sudo apt-get install autoconf automake pkg-config libgtk-3-dev
    sudo ./autogen.sh --prefix=/usr
    sudo make install

Il ne vous reste plus cas accéder au **Paramétres d'apparence** et au **Gestionnaire de fênetres** pour régler votre Environement sur *Arc-flatabulous*.


#### b) Arc Icons
*` Nécessite l'installation de Git (sudo apt-get install git) `*

Le theme choisit pour les icones est Arc Icon. Vous pouvez le télécharger a partir d'[ici](https://github.com/Eito33/Config-Xubuntu/tree/master/arc-icon).
Néanmoins il se trouve par défaut dans le répository [suivant](https://github.com/horst3180/arc-icon-theme).

`Repository Perso :`

    git clone https://github.com/Eito33/Config-Xubuntu.git
  
 `Autres Repository :`

    git clone https://github.com/horst3180/arc-icon-theme --depth 1
 
 
`Une fois le theme télécharger, accéder via le terminal au dossier ou il a été mis (via la commande cd).`

Puis rentrer les commandes suivante :

    sudo ./autogen.sh --prefix=/usr
    sudo make install

Il ne vous reste plus cas accéder au **Paramétres d'apparence** dans la section **Icones** mettre sur le theme Arc pour régler votre Environement sur *Arc Icon*.


### 3. Logiciels

#### a) Xampp

Pour installez xampp vous devez dans un premier temps choisir la version a télécharger sur le site de [xampp](https://www.apachefriends.org/fr/download.html).

`Une fois le logiciel télécharger, accéder via le terminal au dossier ou il a été mis (via la commande cd).`

Puis rentrer les commandes suivante : 

    sudo chmod 755 xampp-linux-*-installer.run<
    sudo ./xampp-linux-*-installer.run
    sudo ln -s /opt/lampp/lampp /usr/bin/lampp

` Vérifier bien que le nom du fichier correspond !`

[Logo Xampp](https://drive.google.com/drive/folders/0B8eas3cznJoBRGxHdVlFeHJUX0E?usp=sharing) pour le lanceur du Tableau de Bord.

#### b) Brackets
`Nécessite l'installation de ` **[libgcrypt11_1.5.3.deb](https://github.com/Eito33/Config-Xubuntu/tree/master/lib)**

Pour installez brackets vous devez dans un premier temps obtenir le .deb a télécharger sur le site de [Brackets](http://brackets.io/).
Une fois le logiciel télécharger, il suffit de lancer le .deb.

**Liste des plugins indispensable :**
* Beautify
* Brackets Tree Icons
* PHP Syntax Hint
* Quick Menu Search

`Penser a lancer Brackets dans un terminal avec la commande sudo pour qu'il puisse modifier n'importe quel fichier.`




### 3. Autres

Liste de tous les logiciels utile installer par défaut :

* [Chromium](https://doc.ubuntu-fr.org/chromium-browser)
* [Firefox](https://doc.ubuntu-fr.org/firefox)
* [Brackets](http://brackets.io/)
* [Xampp](https://doc.ubuntu-fr.org/xampp)
* [Gimp](https://doc.ubuntu-fr.org/gimp)
* [Discord](https://doc.ubuntu-fr.org/discord)
* [Nautilus ](https://doc.ubuntu-fr.org/nautilus)


` Editer par Eito33 pour un usage personel `
