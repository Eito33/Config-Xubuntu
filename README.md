<<<<<<< HEAD
*** Export HTML ***
*******************

<center>

<h1>Config Xubuntu</h1>
<a href="http://i.imgur.com/FAqxDCk.png"><img src = "http://i.imgur.com/FAqxDCkl.png"></a>
</center>
<br /><br />
<h2><b>SOMMAIRE :</b></h2>
<br />
<ol>
    <li> Général</li>
    <li>Environement Graphique</li>
    <li>Logiciels</li>
</ol>
<br />
<hr />
<br />
<h3>1. Général</h3>

<br />
<p>
    Ce dépot concerne principalement les différentes chose a mettre en place aprés un reformatage pour linux!<br /> Testé sous Xubuntu. Il concerne également les environement Xfce.<br />
    <br />
    Toutes les infos concernant l'iso se trouve <a href="http://xubuntu.fr/">ici</a>. (V. 16.04LTS)<br />
    Toutes les infos pour la doc se trouve <a href="https://doc.ubuntu-fr.org/">ici</a>.<br />
    Ce fichier est disponible au format txt.<br />
    Mise a jour le 29/06/2017
</p><br />
<br />
<br />
<h3>2. Environement Graphique</h3>
<br />
<p>
<b><h4>Theme Arc Flatabulous</h4></b><br />
<font color="red"><i>Nécessite l'installation de Git (sudo apt-get install git)</i></font><br /><br />
Le theme choisit est Arc-Flatabulous. Vous pouvez le télécharger a partir d'<a href="">ici</a>. Néanmoins il se trouve par défaut dans le répository <a href="https://github.com/andreisergiu98/arc-flatabulous-theme">suivant</a>.<br /><br />

<pre><code>code</code> <font color="red">Repository perso</font></pre><br />
<pre><code>git clone https://github.com/andreisergiu98/arc-flatabulous-theme</code>  <font color="red">Autre repository</font></pre><br />

Une fois le theme télécharger, accéder via le terminal au dossier ou il a été mis (via la commande cd).<br /><br />

Puis rentrer les commandes suivante : <br /><br />
<pre><code>sudo apt-get install autoconf automake pkg-config libgtk-3-dev</code></pre><br />
<pre><code>sudo ./autogen.sh --prefix=/usr</code></pre><br />
<pre><code>sudo make install</code></pre><br />
Il ne vous reste plus cas accéder au paramétres d'apparence et au Gestionnaire de fênetres pour régler votre Environement sur <b>Arc-flatabulous</b>.
</p><br />
<p>
<b><h4>Arc Icon</h4></b><br />
<font color="red"><i>Nécessite l'installation de Git (sudo apt-get install git)</i></font><br /><br />
Le theme choisit pour les icones est Arc Icon. Vous pouvez le télécharger a partir d'<a href="">ici</a>. Néanmoins il se trouve par défaut dans le répository <a href="https://github.com/horst3180/arc-icon-theme">suivant</a>.<br /><br />

<pre><code>code</code> <font color="red">Repository perso</font></pre><br />
<pre><code>git clone https://github.com/horst3180/arc-icon-theme --depth 1</code>  <font color="red">Autre repository</font></pre><br />

Une fois le theme télécharger, accéder via le terminal au dossier ou il a été mis (via la commande cd).<br /><br />

Puis rentrer les commandes suivante : <br /><br />
<pre><code>git clone https://github.com/horst3180/arc-icon-theme --depth 1</code></pre><br />
<pre><code>sudo ./autogen.sh --prefix=/usr</code></pre><br />
<pre><code>sudo make install</code></pre><br />
Il ne vous reste plus cas accéder au paramétres d'apparence dans la section " Icones " mettre sur le theme Arc pour régler votre Environement sur <b>Arc Icon</b>.
</p><br />

<h3>3. Logiciels</h3>
<br />
<p>
<b><h4>Xampp</h4></b><br />

Pour installez xampp vous devez dans un premier temps choisir la version a télécharger sur le site de <a href="">xampp</a>.
<br/>
<br/>
Une fois le logiciel télécharger, accéder via le terminal au dossier ou il a été mis (via la commande cd).<br /><br />

Puis rentrer les commandes suivante : <br /><br />
<pre><code>sudo chmod 755 xampp-linux-*-installer.run</code> <font color="red">Vérifier le nom de l'app</font></pre><br />
<pre><code>sudo ./xampp-linux-*-installer.run</code> <font color="red">Vérifier le nom de l'app</font></pre><br />
<pre><code>sudo ln -s /opt/lampp/lampp /usr/bin/lampp</code> <font color="red">Permet de lancer Xampp depuis un terminal avec la commande suivante : sudo lampp start</font></pre><br />
</p><br />
<p>
<b><h4>Brackets</h4></b><br />
<font color="red"><i>Nécessite l'installation de <a href="">libgcrypt11_1.5.3.deb</a></i></font><br /><br />

Pour installez brackets vous devez dans un premier temps obtenir le .deb a télécharger sur le site de <a href="">brackets</a>.
<br/>
<br/>
Une fois le logiciel télécharger, accéder via le terminal au dossier ou il a été mis (via la commande cd).<br /><br />

<i>Liste des plugins indispensable :</i><br /><br />
<ol>
    <li>Beautify</li>
    <li>Brackets Tree Icons</li>
    <li>PHP Syntax Hint</li>
    <li>Quick Menu Search</li>
</ol>
<br />
<font color="red"><i>Penser a lancer Brackets dans un terminal avec la commande <u>sudo</u> pour qu'il puisse modifier n'importe quel fichier.</font>
</p><br />
<br />
<br />
=======
# Config-Xubuntu
>>>>>>> e04905700f17788be2df1a6891bdb001db8caa9d
