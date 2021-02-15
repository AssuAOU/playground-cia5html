**texte en gras**
*texte en italique*
<h1>Introduction</h1>

HyperText Markup Language (HTML) est le code utilisé pour structurer une page web et son contenu.
Par exemple, le contenu de votre page pourra être structuré en un ensemble de paragraphes,
une liste à puces ou avec des images et des tableaux de données.
Ce tutoriel va vous fournit les bases de compréhension du HTML et de ses fonctions à travers la création d'une page WEB simple

<h1>1. Qu'est-ce que le HTML?</h1>
<p>HTML n'est pas un langage de programmation. On ne cherche pas à programmer le comportement d'un objet.
On cherche plutôt à présenter un contenu (texte, image, son, vidéo).
C'est un langage de balises qui définit la structure de votre contenu.
HTML se compose d'une série d'éléments, utilisés pour entourer, ou envelopper, les diverses parties du contenu pour les faire apparaître ou agir d'une certaine façon.
Les balises entourantes peuvent être rendues par un mot ou une image lien hypertexte vers quelque chose d'autre, un texte en italique,
une police plus grande ou plus petite, et ainsi de suite.
Par exemple, si on veut écrire:<br>

```html
La SNT, c'est génial!
```
Il faut écrire le code suivant, pour dire qu'il s'agit d'un paragraphe. <br>
`<p>La SNT, c'est génial!</p>`
</p>

# 1.Squelette d'un document HTML

<p>Voici a quoi ressemble un document html.<br></p>

```html
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
</head>

<body>
</body>

</html>
```

*** Explication de l'anatomie du document.

Ce document contient les éléments suivants:
* `<!DOCTYPE html>`: Il s'agit du doctype
* `<html></html>` : C'est dans ces balises que se trouverons l'ensemble de du code html
* `<head></head>`: C'est la tête. C'est pour spécifier des choses qui n'appraittrons pas dans le corps de la page.
* `<meta charset="utf-8">` : C'est pour dire qu'on peut afficher l'ensemble des caractères possibles
* `<body></body>`: Le corps de la page html. C'est là ou on va écire nos paragraphes.


<h1>2. Notre première page</h1>
<h2>Le titre</h2>
<p>Nous allons commencer par donner un titre à notre page. C'est le titre qui sera affiché sur l'onglet.
Nous allons commencer par le squelette et y rajouter des éléments au fur et à mesure.<br>
Il est recommandé de saisir manuellement l'ensemble du code. Mais tu peux aussi copier-coller le code html.<br>
Recopie donc le squelette html et y rajouter le titre de la page. Puis cliquer sur "Run" pour voir le résultat final.<br>
Le titre sera La SNT au lycée </p>

**Code à recopier:**
```html
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>La SNT au lycée</title>
</head>

<body>
</body>

</html>
```
### A toi:
Recopie l'ensemble du code ci-dessus  dans la zone de saisie puis clique sur ***RUN** pour voir ce que ça donne.

**Zone de saisie:**
```html runnable
<!DOCTYPE html>
<html>

</html>
```
***Remarque:*** Pour l'instant, on a une page vide.
C'est normal car on n'exécute pas le code à travers un navigateur.
Donc on ne voit pas le titre de la page.

<h2>Le menu de navigation</h2>
Ici, nous allons ajouter des liens cliquables. Pour le moment,ces liens ne menerons à...rien.
Le code est à recopier est le code qui se trouve entre les commentaires de début et fin.

**Code à recopier**
```html
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>La SNT au collège</title>
</head>

<body>
    <!-- Début Menu de navigation du site à copier -->
    <ul class="navbar">
        <li><a href="index.html">Page d'accueil</a>
        <li><a href="Thème_1_Internet.html">Thème 1: Internet</a>
        <li><a href="Thème_Transverse_Python.html">Thème Transverse</a>
    </ul>
    <!-- Fin Menu de navigation du site à copier-->
</body>

</html>
```

### A toi:
Recopie le code du menu de navigation puis clique sur ***RUN** pour voir ce que ça donne.

**Zone de saisie**
```html runnable
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>La SNT au collège</title>
</head>

<body>
    <!-- Début Menu de navigation du site -->
   


    <!-- Fin Menu de navigation du site-->
</body>

</html>
```
***Analyse:*** On a maintenant une page, avec des liens, mais qui ne mènent à rien pour le moment.

<h2>Le contenu principal</h2>
<p>Nous allons maintenant rajouter du contenu. Un contenu est généralement constitué d'un titre principal, d'un sous-titre et de paragraphes.</p>
<p>Voici comment introduire ces différents éléments.<br></p>

* `<h1>Mon titre principal</h1>`:
* `<h2>Mon sous titre</h2>`:
* `<p>Mon paragraphe</p>`:

**Code à recopier**
```html
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>La SNT au collège</title>
</head>

<body>
    
    <ul class="navbar">
       <li><a href="index.html">Page d'accueil</a>
        <li><a href="Thème_1_Internet.html">Thème 1: Internet</a>
        <li><a href="Thème_Transverse_Python.html">Thème Transverse</a>
    </ul>
    <!-- Début Contenu Principal à copier -->
    <h1>La SNT au lycée</h1>
    <h2>Qu'est-ce que la SNT au lycée?</h2>
    <p>La SNT s’inscrit dans le prolongement de l’algorithmique, d’informatique et de programmation vus au collège.</p>
    <h2>Thème 1: Internet</h2>
    <p>Internet est un réseau informatique mondial.</p>
    <h2>Thème Transverse: Python</h2>
    <p>Python est un langage de programmation facile à prendre en main.</p>
    <!-- Fin Contenu principal à copier-->
</body>

</html>
```

**Zone de saisie**
```html runnable
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>La SNT au collège</title>
</head>

<body>
    
    <ul class="navbar">
        <li><a href="index.html">Page d'accueil</a>
        <li><a href="Thème_1_Internet.html">Thème 1: Internet</a>
        <li><a href="Thème_Transverse_Python.html">Thème Transverse</a>
    </ul>
    <!-- Début Contenu Principal à copier -->
    


    <!-- Fin Contenu principal à copier-->
</body>

</html>
```
***Analyse:*** On a maintenant une page, avec des liens, et un contenu minimaliste.


<h2>Ajouter une image</h2>
<p>Nous allons ajouter une image à notre page.</p>

**Code à recopier**
```html
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>La SNT au collège</title>
</head>

<body>
    
    <ul class="navbar">
       <li><a href="index.html">Page d'accueil</a>
        <li><a href="Thème_1_Internet.html">Thème 1: Internet</a>
        <li><a href="Thème_Transverse_Python.html">Thème Transverse</a>
    </ul>
    
    <h1>La SNT au lycée</h1>
    <h2>Qu'est-ce que la SNT au lycée?</h2>
    <p>La SNT s’inscrit dans le prolongement de l’algorithmique, d’informatique et de programmation vus au collège.</p>
    <h2>Thème 1: Internet</h2>
    <p>Internet est un réseau informatique mondial.</p>
    <h2>Thème Transverse: Python</h2>
    <p>Python est un langage de programmation facile à prendre en main.</p>
    
    <!-- Début lien image à copier -->
    <img src="https://octodex.github.com/images/collabocats.jpg" alt="" />
    <!-- Début lien image à copier-->
</body>

</html>
```

**Zone de saisie**
```html runnable
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>La SNT au collège</title>
</head>

<body>
    
    <ul class="navbar">
       <li><a href="index.html">Page d'accueil</a>
        <li><a href="Thème_1_Internet.html">Thème 1: Internet</a>
        <li><a href="Thème_Transverse_Python.html">Thème Transverse</a>
    </ul>
    
    <h1>La SNT au lycée</h1>
    <h2>Qu'est-ce que la SNT au lycée?</h2>
    <p>La SNT s’inscrit dans le prolongement de l’algorithmique, d’informatique et de programmation vus au collège.</p>
    <h2>Thème 1: Internet</h2>
    <p>Internet est un réseau informatique mondial.</p>
    <h2>Thème Transverse: Python</h2>
    <p>Python est un langage de programmation facile à prendre en main.</p>
    
    <!-- Début lien image à copier -->
    

    <!-- Début lien image à copier-->
</body>

</html>
```
<h2>Ajouter un lien</h2>
<p>Nous allons finir cette partie en ajoutant un lien à la fin de notre page.
Le WEB existe grâce aux liens.</p>
<a href="https://pixees.fr/informatiquelycee/n_site/snt.html">Cours sur le SNT</a>


###### Sources :

<https://developer.mozilla.org/fr/docs/Apprendre/Commencer_avec_le_web/Les_bases_HTML>
<https://www.w3.org/Style/Examples/011/firstcss.fr.html>
<https://assemble.io/docs/Cheatsheet-Markdown.html>
<https://developer.mozilla.org/fr/docs/Apprendre/Commencer_avec_le_web>
