# Config Xubuntu - `V. 16.04LTS`
![ImageLOAD](http://i.imgur.com/Hs1aI7b.png)

## SOMMAIRE : 

* Général
* Environement Graphique
* Logiciels
* Autres
* Ressources


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

    sudo chmod 755 xampp-linux-*-installer.run
    sudo ./xampp-linux-*-installer.run
    sudo ln -s /opt/lampp/lampp /usr/bin/lampp

` Vérifier bien que le nom du fichier correspond !`


#### b) Visual Studio Code

Pour installez Visual Studio Code vous devez dans un premier temps obtenir le .deb a télécharger sur le site de [Visual Studio](https://code.visualstudio.com/).
Une fois le logiciel télécharger, il suffit de lancer le .deb.

**Liste des plugins indispensable :**
* [IntelliSense for CSS class names](https://marketplace.visualstudio.com/items?itemName=Zignd.html-css-class-completion)
* [Auto-Open Markdown Preview](https://marketplace.visualstudio.com/items?itemName=hnw.vscode-auto-open-markdown-preview)


### c) OverGrive

Pour installez Overgrive vous devez dans un premier temps obtenir le .deb a télécharger sur le site de [Overgrive](https://www.thefanclub.co.za/overgrive).

Une fois télécharger lancer la commande suivante via un `terminal` :

    sudo add-apt-repository universe && sudo apt-get update


Une fois les dépots validés il ne vous reste plus cas installez le .deb


### 3. Autres

### a) Pour PC portable UEFI (Aspire ONE)

Pour l'installation de [Xubuntu](https://doc.ubuntu-fr.org/uefi) sur un PC portable ACER Aspire ONE.
 Ne pas désactiver le Secure Boot et laisser par défaut la configuration du bios.

* Booter sur la clé USB en mode UEFI
* Installez Xubuntu normalement
* Ne pas installer les Mise a Jour ni les programmes additionel
* Créer soit même les partitions comme suit 
    * Partition Swap (1x a 1,5x votre ram)
    * Partiont EFI (~600mo)
    * Partition / (Le reste)
    * `Installez le programme de démarrage sur la partition EFI`
* Redemarrer aprés l'installation
* Au redemarrage (aprés avoir enlever la Clé USB) appuyer sur F2 pour accéder au Bios
* Allez dans le 3éme onglets `Sécurity`
* Accédez a l'option `select an uefi as trusted for executing`
* Séléctionnez `grubx64.efi` et nommez le `Xubuntux64`
* Redemarrer a nouveau et retourner dans le bios
* Allez dans l'ongle `Boot`
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