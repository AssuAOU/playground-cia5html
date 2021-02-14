# Introduction

Nous allons apprendre le HTML et CSS ensemble dans ce tutoriel.
Duant ce tutoriel, tu vas apprendre à créer une page html pas à pas.
Il faudra bien lire le contenu et faire les exercices qui te seront donnés au fur et à mesure.


# 1.Anatomie d'un document HTML
```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>Ma page de test</title>
  </head>
  <body>
    <img src="images/firefox-icon.png" alt="Mon image de test">
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