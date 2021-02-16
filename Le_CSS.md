# Introduction

Qu'est-ce que le CSS?

Les Cascading StyleSheets — ou CSS — (Feuilles de style en cascade) sont la première technique à apprendre après le HTML.
Alors que HTML s'utilise pour définir la structure du contenu, les CSS sont employées pour composer et déterminer l'apparence de ce contenu.
Ainsi par exemple, vous utiliserez les CSS pour modifier les POLICE, la `couleur`, la taille et l'e s p a c e m e n t de votre contenu,
pour le répartir sur plusieurs colonnes ou bien pour ajouter des animations et autres fonctionnalités décoratives.

# 1. Rappel sur le HTML
Dans ce tutoriel, nous partirons d'un document HTML simple et y appliquerons des CSS, tout en apprenant des choses pratiques sur le langage.
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

# 2. Ajouter du CSS au HTML

# Bilan
Dans ce tutoriel nous avons vu plusieurs façons de mettre en forme un document grâce aux règles CSS.

# Sources
<https://developer.mozilla.org/fr/docs/Learn/CSS/First_steps/Getting_started>
