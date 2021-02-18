# Introduction

Qu'est-ce que le CSS?

Les Cascading StyleSheets — ou CSS — (Feuilles de style en cascade) sont la première technique à apprendre après le HTML.
Alors que HTML s'utilise pour définir la structure du contenu, les CSS sont employées pour composer et déterminer l'apparence de ce contenu.
Ainsi par exemple, vous utiliserez les CSS pour modifier les POLICE, la `couleur`, la taille et l'e s p a c e m e n t de votre contenu,
pour le répartir sur plusieurs colonnes ou bien pour ajouter des animations et autres fonctionnalités décoratives.

# 1. Comment utiliser la feuille de style?
Dans ce tutoriel, nous partirons d'un document HTML simple et y appliquerons des CSS, tout en apprenant des choses pratiques sur le langage.
Il y'a plusieurs façon pour appliquer CSS à un document:

1. On peut écrire les règles `dans un fichier à part` et créer un lien vers la feuille de style CSS depuis l'en-tête (dans head) du document HTML.
2. On peut écrire les règles directement `dans le document HTML`.

Dans ce tutoriel, nous allons faire la **deuxième méthode** pour des questions pratique **MAIS** la première méthode est la plus utilisée et la plus "propre".

#### Méthode 1
Voici comment appliquer cette méthode:

* Avec votre éditeur de code, dans le dossier où se trouve le document HTML, créez un fichier et sauvegardez le sous le nom styles.css
L'extension .css indique que c'est un fichier CSS.

* Pour lier styles.css à index.html ajoutez la ligne suivante dans la section <head> du document HTML :
```html
<link rel="stylesheet" href="styles.css">
```
Et enfin, il suffira d'ajouter les règles de style dans le document styles.css les un à la suite des autres. Comme dans l'éxemple suivant, où on met les paragraphes en rouge.

```html
p {
  color: red;
  }
```

#### Méthode 2
Voici comment appliquer cette méthode:
Dans le document html, ajouter les lignes suivantes dans l'en-tête (dans "body").
```html
<style type="text/css">
 
 </style>
```

Et écrire les règles dans la balise `<style></style>`.
Dans le code ci-après, l'ensemble des paragraphe seront écrits en rouge.

```html
 <style type="text/css">
  
  p {
  color: red;
  }
```


Cet élément <link> indique au navigateur la présence d'une feuille de style, grâce à l'attribut rel ; la valeur de l'attribut href donne la localisation du fichier CSS.
Il ne reste plus qu'à ajouter les lignes de code à la feuille de style CSS.

# Mise en forme de notre page

On commencer par modifier la couleur de fond de la page WEB. Et la couleur de police.
On va mettre le fond en noir et le texte en blanc.
Cette action se fait avec le code suivant.
```html
body{
    color: white;
    background-color: black
  }
```

**A toi**</br>
Clique sur `RUN` pour voir le résultat.</br>
Ensuite, modifie le code pour afficher le texte en ***Rouge*** (red) et le fond en ***vert***(green).</br>
Clique sur `SUCCESS` pour relancer la page et voir le résultat.

```html runnable
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>Bienvenue à la cité scolaire</title>
 
  <style type="text/css">
  body{
    color: white;
    background-color: black
  }
 </style>
</head>

<body>
    <!-- Menu de navigation du site-->
    <ul>
        <li>Accueil</li>
        <li>Actualité</li>
        <li>La cité scolaire</li>
        <li>Classes et options</li>
        <li>Examens</li>
        <li>L'accès à Pronote et NEO</li>
    </ul>
    <h1>Accueil</h1> 
    <h1>Bienvenue à la cité scolaire</h1> 
    <h3>Horaires</h3>
    <p> La cité sclaire est ouverte du lundi au samedi. Pour joindre l'accueil, il faut composer le 0269 70 71 72</p>
    <p>En cas d'urgence, contacter le <strong>06 39 40 41 42</strong>.</p>
   
   <!--Signature -->
   <adress>Site crée en Mars 2020 par les classes de 2nd A et B.</adress>

    <a href="https://www.ac-mayotte.fr/">Cliquz ici pour vous rendre sur le site de l'académie de Mayotte</a>.
</body>

</html>
```

On va ensuite changer la couleur des titres et paragraphes.
```html runnable
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>Ceci est le titre de cette page</title>
 
  <style type="text/css">
  body{
    color: purple;
    background-color: #d8da3d
  }

  h1 {
  color: red;
  }

  p {
  color: red;
  }
 </style>
</head>

<body>
    <h1>Titre principal</h1> 
    <h2>Titre de section</h2>
    <p> Ce ceci est une paragraphe. Je peux écrire ici autant que je veux.</p>
    <p>J'ai mis en <strong>gras</strong> le mot gras gros!</p>
    <a href="https://www.ac-mayotte.fr/">Cliquz ici pour vous rendre sur le site de l'académie de Mayotte</a>.

</body>

</html>
```


# Bilan
Dans ce tutoriel nous avons vu plusieurs façons de mettre en forme un document grâce aux règles CSS.

# Sources
<https://developer.mozilla.org/fr/docs/Learn/CSS/First_steps/Getting_started>
