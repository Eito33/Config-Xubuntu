# Config Xubuntu - `V. 16.04LTS`
![ImageLOAD](http://i.imgur.com/Hs1aI7b.png)

## SOMMAIRE : 

* [Général](https://github.com/Eito33/Config-Xubuntu#1-général)
* [Environement Graphique](https://github.com/Eito33/Config-Xubuntu#2-environement-graphique)
* [Logiciels](https://github.com/Eito33/Config-Xubuntu#3-logiciels)
* [Autres](https://github.com/Eito33/Config-Xubuntu#3-autres)
* [Ressources](https://github.com/Eito33/Config-Xubuntu#4-ressources)


------------------------------


### 1. Général

Ce dépot concerne principalement les différentes choses a mettre en place aprés un reformatage pour Linux!

1. Testé sous **Xubuntu**. Il concerne également les environements **Xfce**.
2. Toutes les infos concernant l'iso se trouvent [ici](http://xubuntu.fr/). (`V. 16.04LTS`)
3. Toutes les infos pour la doc se trouvent [ici](https://doc.ubuntu-fr.org/).
4. Pour tous télécharger d'un coup utiliser la commande :

        git clone https://github.com/Eito33/Config-Xubuntu.git


*Mise a jour le 03/07/2017* 

### 2. Environement Graphique

#### a) Theme Arc Flatabulous
*` Nécessite l'installation de Git (sudo apt-get install git) `*

Le thème choisit est Arc-Flatabulous. Vous pouvez le télécharger a partir d'[ici](https://github.com/Eito33/Config-Xubuntu/tree/master/theme/arc-flatabulous).
Néanmoins il se trouve par défaut dans le repository [suivant](https://github.com/andreisergiu98/arc-flatabulous-theme).

`Repository Perso :`

    git clone https://github.com/Eito33/Config-Xubuntu.git
  
 `Autres Repository :`

    git clone https://github.com/andreisergiu98/arc-flatabulous-theme
 
 
` Une fois le thème téléchargé, accéder via le terminal au dossier ou il a été mis (via la commande cd).`

Puis rentrer les commandes suivantes :

    sudo apt-get install autoconf automake pkg-config libgtk-3-dev
    sudo ./autogen.sh --prefix=/usr
    sudo make install

Il ne vous reste plus qu'a accéder au **Paramétres d'apparences** et au **Gestionnaire de fenêtres** pour régler votre Environement sur *Arc-flatabulous*.


#### b) Arc Icons
*` Nécessite l'installation de Git (sudo apt-get install git) `*

Le thème choisit pour les icones est Arc Icon. Vous pouvez le télécharger a partir d'[ici](https://github.com/Eito33/Config-Xubuntu/tree/master/theme/arc-icon).
Néanmoins il se trouve par défaut dans le repository [suivant](https://github.com/horst3180/arc-icon-theme).

`Repository Perso :`

    git clone https://github.com/Eito33/Config-Xubuntu.git
  
 `Autres Repository :`

    git clone https://github.com/horst3180/arc-icon-theme --depth 1
 
 
`Une fois le thème téléchargé, accéder via le terminal au dossier ou il a été mis (via la commande cd).`

Puis rentrer les commandes suivante :

    sudo ./autogen.sh --prefix=/usr
    sudo make install

Il ne vous reste plus cas accéder au **Paramétres d'apparences** dans la section **Icones** mettre sur le thème Arc pour régler votre Environement sur *Arc Icon*.


### 3. Logiciels

#### a) Xampp

Pour installez xampp vous devez dans un premier temps choisir la version a télécharger sur le site de [xampp](https://www.apachefriends.org/fr/download.html).

`Une fois le logiciel téléchargé, accéder via le terminal au dossier ou il a été mis (via la commande cd).`

Puis rentrer les commandes suivantes : 

    sudo chmod 755 xampp-linux-*-installer.run
    sudo ./xampp-linux-*-installer.run
    sudo ln -s /opt/lampp/lampp /usr/bin/lampp

` Vérifier bien que le nom du fichier corresponde !`

Pour démarrer ou stopper l'éxécution de Xampp il ne vous restera plus qu'a rentrer les commandes suivantes :

    sudo lampp start
    sudo lampp stop


#### b) Visual Studio Code

Pour installez Visual Studio Code vous devez dans un premier temps obtenir le .deb a télécharger sur le site de [Visual Studio](https://code.visualstudio.com/).
Une fois le logiciel téléchargé, il suffit de lancer le .deb.

**Liste des plugins indispensable :**
* [IntelliSense for CSS class names](https://marketplace.visualstudio.com/items?itemName=Zignd.html-css-class-completion)
* [Auto-Open Markdown Preview](https://marketplace.visualstudio.com/items?itemName=hnw.vscode-auto-open-markdown-preview)

`Liste a compléter`


### c) OverGrive

Pour installer Overgrive vous devez dans un premier temps obtenir le .deb a télécharger sur le site de [Overgrive](https://www.thefanclub.co.za/overgrive).

Une fois téléchargé lancer la commande suivante via un `terminal` :

    sudo add-apt-repository universe && sudo apt-get update


Une fois les dépots validés il ne vous reste plus qu'a installez le .deb et a le configurer.


### 3. Autres

### a) Pour PC portable UEFI (Aspire ONE)

Pour l'installation de [Xubuntu](https://doc.ubuntu-fr.org/uefi) sur un PC portable ACER Aspire ONE.
 Ne pas désactiver le [Secure Boot](https://forum.ubuntu-fr.org/viewtopic.php?pid=21468818#p21468818) et laisser par défaut la configuration du bios.

* Booter sur la clé USB en mode UEFI
* Installer Xubuntu normalement
* Ne pas installer les Mises a Jour ni les programmes additionnels
* Créer soit même les partitions comme suit 
    * Partition `Swap` (`1x a 1,5x votre ram`)
    * Partition `EFI` (`~600mo`)
    * Partition `/` 
    * `Installez le programme de démarrage sur la partition EFI`
* Redemarrer aprés l'installation
* Au redemarrage (aprés avoir enlever la Clé USB) appuyer sur F2 pour accéder au Bios
* Aller dans le 3éme onglets `Sécurity`
* Accéder a l'option `select an uefi as trusted for executing`
* Séléctionner `grubx64.efi` et nommer le `Xubuntux64`
* Redemarrer a nouveau et retourner dans le bios
* Aller dans l'onglet `Boot`
* Il suffit maintenant de remonter l'option `EFI File Boot 0 : Xubuntux64` en premiere position
* Redemarrer

### 4. Ressources

Liste des ressources pour la configuration

* [Icon Xampp](https://drive.google.com/drive/folders/0B8eas3cznJoBRGxHdVlFeHJUX0E?usp=sharing)
* [Fond d'écran Montagne](https://drive.google.com/drive/folders/0B8eas3cznJoBRGxHdVlFeHJUX0E?usp=sharing)

Liste de tous les logiciels utile installer par défaut :

* [Chromium](https://doc.ubuntu-fr.org/chromium-browser)
* [Firefox](https://doc.ubuntu-fr.org/firefox)
* [Visual Studio Code](https://code.visualstudio.com/)
* [Xampp](https://doc.ubuntu-fr.org/xampp)
* [Gimp](https://doc.ubuntu-fr.org/gimp)
* [Discord](https://doc.ubuntu-fr.org/discord)
* [Nautilus](https://doc.ubuntu-fr.org/nautilus)
* [Overgrive](https://doc.ubuntu-fr.org/google_drive)
* [Git](https://doc.ubuntu-fr.org/git)


` Edité par Eito33 pour un usage personel `