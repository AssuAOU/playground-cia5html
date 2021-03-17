# Introduction

**HyperText Markup Language (HTML)** est le code utilisé pour structurer une page web et son contenu.
Par exemple, le contenu de votre page pourra être structuré en un ensemble de paragraphes,
une liste à puces ou avec des images, vidéos et des tableaux de données.
Ici, nous allons voir ce qu'est le HTML et certaines balises importantes.

# 1. Qu'est-ce que le HTML?
HTML n'est pas un langage de programmation (comme le Python par exemple), ici, pas question de conditions, de boucles....c'est un langage de description.
On cherche plutôt à présenter un contenu (texte, image, son, vidéo). La description se fait avec des ```balises```.

Par exemple, si on veut écrire:<br/>

```html
La SNT, c'est génial!
```
Il faut écrire le code suivant, pour dire qu'il s'agit d'un paragraphe. <br>
`<p>La SNT, c'est génial!</p>`

Grâce au HTML tu vas pouvoir, dans ton navigateur (Firefox, Chrome, Opera,....), afficher du texte, afficher des images, proposer des hyperliens (liens vers d'autres pages web), afficher des formulaires et même maintenant afficher des vidéos (grâce à la dernière version du HTML, l'HTML5).
 
# 2.Structure d'un document HTML

Voici à quoi ressemble un document html.

**Structure d'un document HTML** 
```html
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>Ceci est mon titre</title>
</head>

<body>

</body>

</html>
```

**Explication de la structure du document.**

Ce document contient les éléments suivants:
* `<!DOCTYPE html>`: Le type de document. Ici, on dit qu'il s'agit d'un document HTML5
* `<html></html>` : C'est dans ces balises que se trouverons l'ensemble du code html de la page.
* `<head></head>`: On mettra dedans toute chose que tu souhaites inclure dans la page HTML mais qui ne sera pas afficher aux visiteurs de la page (mots clés, style CSS)
* `<title>Ceci est le titre de la page</title>`: Il s'agit du titre de la page.
* `<meta charset="utf-8">` : Cet élément définit le jeu de caractères à utiliser pour le document: UTF-8 comporte la quasi‑totalité des caractères de toutes les écritures de langues humaines connues
* `<body></body>`: Il contient tout le contenu que tu souhaites afficher aux internautes lorsqu'ils visitent ta page, que ce soit du texte, des images, des vidéos, des jeux.

# 3. Les balises essentielles pour débuter
Comme déjà évoqué précedement, en HTML tout est une histoire de balise que l'on ouvre et que l'on ferme.
Une balise ouvrante est de la forme <nom_de_la_balise>, les balises fermantes sont de la forme </nom_de_la_balise>.
**Chaque balise ouvrante doit être automatiquement fermée.**

Pour bien débuter en HTML, il est important de connaitres ces quelques balises.

* `<h1>Titre principal</h1> :` Il s'agit du titre principal: Le titre le plus important est h1. Le moins important h6.
* `<h2>Titre de section</h2> :`
* `<h3>Sous titre</h3> :`
* `<p> Ce ceci est un paragraphe. Je peux écrire ici autant que je veux.</p> :`C'est ici que l'on écrira nos paragraphes
* `<p>J'ai mis en <strong>gras</strong> le mot gras!</p> : `On peut mettre en gras avec la balise **strong**
* `<a href="https://www.ac-mayotte.fr/">Cliquz ici pour vous rendre sur le site de l'académie de Mayotte</a> : `On peut créer des lien cliquables avec la balise **a**. La première partie est le lien, la deuxième est la description du lien.
* `<img src="https://octodex.github.com/images/filmtocat.png" alt="Cette image représente un poulpe-chat." /> : `On peut aussi insérer une image: **src** est la source; **alt** est la description de l'image.

# 4. A toi
Clique sur `RUN` pour voir le résultat.
Tu peux recliquer sur `SUCCESS` autant de fois que nécessaire pour relancer la page.
Voici le travail à faire:</br>
+ Changer le titre de la page: Mettre comme nouveau titre **La SNT au collège**
+ Changer le **Titre principal** en **Ceci est ma première page WEB.**
+ Changer le **titre de section** en **Le langage HTML**
+ Ajouter un petit paragraphe expliquant ce qu'est le HTML
+ Tu peux rajouter d'autres paragraphes, titres prinicpal et de section

```html runnable
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>Ceci est mon titre</title>
</head>

<body>
    <h1>Titre principal</h1> 
    <h2>Titre de section</h2>
    <p> Ce ceci est un paragraphe. Je peux écrire ici autant que je veux.</p>
    <p>J'ai mis en <strong>gras</strong> le mot gras!</p>
    <a href="https://www.ac-mayotte.fr/">Cliquz ici pour vous rendre sur le site de l'académie de Mayotte</a>.
    <img src="https://octodex.github.com/images/filmtocat.png" alt="Cette image représente un poulpe-chat qui prend une photo." />
</body>

</html>
```

## Questionnaire QCM

Voici quelques QCM pour voir si tu as bien compris. N'hésite pas à relire ce qui précède si tu as un doute.

---

###### QCM 1

?[Que veut dire HTML? ? ]
-[ ] ^-^
-[x] HyperText Markup Language
-[ ] HyperText Market Language
-[ ] Hi The Great Teacher Onizuka

---

###### QCM 2
 
?[On utilise le HTML pour ? ]
-[ ] Programmer le déplacement des images.
-[x] Décrire un contenu.
-[ ] Naviguer sur le WEB.
-[ ] Télécharger des vidéos,images.

---

###### QCM 3

?[Le code HTML utilise ]
-[ ] Des crochets: []
-[ ] Des parenthèses: ()
-[x] Des balises: <>
-[ ] (^_^)

---

###### QCM 4
```html
<p>Nature, berce-le chaudement: il a froid.</p>
```
?[Cette balise correspond à]
-[ ] Un titre
-[ ] Des lignes
-[x] Un paragraphe
-[ ] (~_~)  

---

###### QCM 5
```html
<h1>Le tour du monde en 80 jours.</h1>
```
?[Ce code html décrit]
-[ ] Un lien.
-[x] Un titre.
-[ ] Un paragraphe.
-[ ] 80 jours.  

---

###### QCM 6
```html
<head>

</head>
```
?[Cette balise html  décrit]
-[x] Des choses qui ne sont pas visible par l'internaute
-[ ] Des choses visibles par l'internaute
-[ ] Des paragraphes et des titres de section
-[ ] -_-  

---

###### QCM 7
```html
<body>
    
</body>
```
?[Cette balise html  décrit]
-[ ] Du texte en gras.
-[ ] Un un lien hypertexte.
-[x] Un contenu visible par l'internaute.
-[ ] (^o^)   

---
###### QCM 8

?[Chaque balise ouvrante doit être automatiquement]
-[x] fermée.
-[ ] ouverte.
-[ ] mise de côté.
-[ ] (^-^)   

---
###### QCM 9
```html
<p>Ceci est le TITRE de la page WEB</p>
```
?[Ce code HTML décrit ]
-[ ] Un titre
-[ ] Des lignes
-[x] Un paragraphe
-[ ] (~-~)  

---
###### QCM 10
```html
<a href="https://www.google.com/">Cliquz ici pour vous rendre sur le site de l'académie de Mayotte</a>.
```
?[Ce code html]
-[ ] ne fonctionnera pas car il y'a une incohérence.
-[x] fonctionnera mais la description du lien ne correspond pas à l'URL
-[ ] a 80 jours.

---
###### QCM 11
 
?[Le HTML permet de décrire? ]
-[ ] la forme d'une page Web.
-[x] Le contenu d'une page Web.
-[ ] Naviguer sur le WEB.
-[ ] le contenu et la forme, ça dépend du lien hypertexte.

---