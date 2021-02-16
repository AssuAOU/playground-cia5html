# Notre première page
Nous allons ici créer notre premier page WEB. Cette page sera dédiée au SNT au lycée.

## Le titre
Nous allons commencer par donner un titre à notre page. C'est le titre qui sera affiché sur l'onglet.
Il est recommandé de saisir manuellement l'ensemble du code. Mais tu peux aussi copier-coller le code html.
Pour commencer, recopie donc le code de la partie `Code à recopie` dans la partie `Zone de saisie`.<br>
Puis clique sur `Run` pour voir le résultat final.<br>

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
Recopie l'ensemble du code ci-dessus  dans la zone de saisie puis clique sur ***RUN*** pour voir le résultat.

**Zone de saisie:**
```html runnable
<!DOCTYPE html>
<html>

</html>
```
***Analyse:*** Pour l'instant, on a une page vide. On a juste ajouté le titre de la page WEB.
Ce titre est visible quand on lance le code HTML avec un navigateur WEB.
Donc on ne voit pas le titre de la page dans notre exemple.

<h2>Le menu de navigation</h2>
Ici, nous allons ajouter des liens cliquables. Pour le moment,ces liens ne menerons à...rien.
Voici a quoi ressemblera le menu:
* Page d'accueil
* Thème 1: Internet
* Thème 2: Le WEB
* Thème 3: Les réseaux sociaux
* Thème Transverse: La programmation

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
      <li>Page d'accueil</li>
      <li>Thème 1: Internet</li>
      <li>Thème 2: Le WEB</li>
      <li>Thème 3: Les réseaux sociaux</li>
      <li>Thème Transverse: Python</li>       
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
       <li>Page d'accueil
        <li>Thème 1: Internet
        <li>Thème 2: Le WEB
        <li>Thème 3: Les réseaux sociaux
        <li>Thème Transverse: Python
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
        <li>Page d'accueil
        <li>Thème 1: Internet
        <li>Thème 2: Le WEB
        <li>Thème 3: Les réseaux sociaux
        <li>Thème Transverse: Python
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
      <li>Page d'accueil
        <li>Thème 1: Internet
        <li>Thème 2: Le WEB
        <li>Thème 3: Les réseaux sociaux
        <li>Thème Transverse: Python
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
