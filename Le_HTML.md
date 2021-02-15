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

# 1.Anatomie d'un document HTML

<p>Voici a quoi un document html.<br></p>

```html
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>Ma première page avec du style</title>
</head>

<body>
    <h1> Je suis un titre</h1>
    <h2> Je suis un sous titre</h2>
    <p>Ceci est un paragraphe, du début à la fin</p>
</body>

</html>
```

Explication de l'anatomie du document.

Ce document contient les éléments suivants:
* `<!DOCTYPE html>`: Il s'agit du doctype
* `<html></html>` : C'est dans ces balises que se trouverons l'ensemble de du code html
* `<head></head>`: C'est la tête. C'est pour spécifier des choses qui n'appraittrons pas dans le corps de la page.
* `<meta charset="utf-8">` : C'est pour dire qu'on peut afficher l'ensemble des caractères possibles
* `<title>Ma page de test</title>`: Le titre de la page. C'est ce qui va s'afficher sur l'onglet du navigateur
* `<body></body>`: Le corps de la page html

# 2. Le langage HTML

```html runnable
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>Ma première page avec du style</title>
</head>

<body>

<!-- Contenu principal -->
<h1>Ma première page avec du style</h1>

<p>Bienvenue sur ma page avec du style! 

<p>Je devrais étayer, mais je ne sais comment encore.

</body>
</html>
```

###### Exercice 1 :
Ecrire
![Minion](http://octodex.github.com/images/minion.png)
---
# Sources

<https://developer.mozilla.org/fr/docs/Apprendre/Commencer_avec_le_web/Les_bases_HTML>
<https://www.w3.org/Style/Examples/011/firstcss.fr.html>
<https://assemble.io/docs/Cheatsheet-Markdown.html>
<https://developer.mozilla.org/fr/docs/Apprendre/Commencer_avec_le_web>
