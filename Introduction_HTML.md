# Introduction

HyperText Markup Language (HTML) est le code utilisé pour structurer une page web et son contenu.
Par exemple, le contenu de votre page pourra être structuré en un ensemble de paragraphes,
une liste à puces ou avec des images, vidéos et des tableaux de données.
Ici, nous allons voir ce qu'est le HTML et certaines balises importantes.

# 1. Qu'est-ce que le HTML?
HTML n'est pas un langage de programmation (comme le Python par exemple), ici, pas question de conditions, de boucles....c'est un langage de description.
On cherche plutôt à présenter un contenu (texte, image, son, vidéo). La desciption se fait avec des ```balises```.

Par exemple, si on veut écrire:<br/>

```html
La SNT, c'est génial!
```
Il faut écrire le code suivant, pour dire qu'il s'agit d'un paragraphe. <br/>
`<p>La SNT, c'est génial!</p>`

<p>Grâce au HTML tu vas pouvoir, dans ton navigateur (Firefox, Chrome, Opera,....), afficher du texte, afficher des images, proposer des hyperliens (liens vers d'autres pages web), afficher des formulaires et même maintenant afficher des vidéos (grâce à la dernière version du HTML, l'HTML5).
</p>
 
# 2.Squelette d'un document HTML

Voici a quoi ressemble un document html.

**Squelette d'un document HTML** 
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

***Explication de l'anatomie du document.***

Ce document contient les éléments suivants:
* `<!DOCTYPE html>`: Le type de document. Ici, on dit qu'il s'agit d'un document HTML
* `<html></html>` : C'est dans ces balises que se trouverons l'ensemble du code html de la page.
* `<head></head>`: On mettra dedans toute chose que tu souhaites inclure dans la page HTML mais qui ne sera pas afficher aux visiteurs de la page (mots clés, style CSS)
* `<title>Ceci est le titre de la page</title>`: Il s'agit du titre de la page.
* `<meta charset="utf-8">` : Cet élément définit le jeu de caractères à utiliser pour le document: UTF-8 comporte la quasi‑totalité des caractères de toutes les écritures de langues humaines connues
* `<body></body>`: Il contient tout le contenu que tu souhaites afficher aux internautes lorsqu'ils visitent ta page, que ce soit du texte, des images, des vidéos, des jeux.

# 3. Utilisation des balises

Comme déjà évoqué ci-dessus, en HTML tout est une histoire de balise que l'on ouvre et que l'on ferme.
Une balise ouvrante est de la forme <nom_de_la_balise>, les balises fermantes sont de la forme </nom_de_la_balise>.
Chaque balise ouvrante doit être automatiquement fermée.

## 3.1 Les commentaires
En HTML, comme pour la plupart des langages de programmation, il existe un mécanisme permettant d'écrire des commentaires dans le code.
Les commentaires sont ignorés par le navigateur et invisibles à l'utilisateur.
Leur but est de permettre d'inclure des commentaires dans le code pour dire comment il fonctionne, que font les diverses  parties du code, etc.
Cela peut s'avérer très utile si vous revenez à un codage que vous n'avez pas travaillé depuis 6 mois et que vous ne pouvez pas vous rappeler ce que vous avez fait — ou si vous donnez votre code à quelqu'un d'autre pour qu'il y travaille.<br>
**Il faut prendre la bonne habitude de toujours documenter son code, cest à dire de mettre des commenter son code.**<br>

Pour transformer une section de contenu dans votre fichier HTML en commentaire, vous devez la mettre dans les marqueurs spéciaux <!--  et -->, par exemple :

```html
<p>Je ne suis pas dans un commentaire</p>

<!-- <p>Je suis dans un commmentaire!</p> -->
```
**A toi**<br>
Ajoute un commentaire dans la balise `<body></body>` et explique a quoi sert cette balise.

Pense à cliquer sur `RUN` pour voir le résultat.
```html runnable
<!DOCTYPE html>
<html>
<head>
  <!-- Balise head: On y trouve ce qu'on veut inclure dans la page mais qui ne sera pas vu par l'internaute-->
  <meta charset="utf-8">
</head>

<body>
    <p>Je ne suis pas dans un commentaire, mais j'en attends un juste après moi.</p>

</body>

</html>

```
`Analyse:` En cliquant sur RUN, tu as remarqué que seul ce qui est dans body est affiché.
Les commentaires et ce qui est dans head ne sont pas visibles par l'utilisateur.

## 3.2 Les balises essentiels pour débuter

Pour bien débuter en HTML, il est important de connaitres ces quelques balises.

* `<h1>Titre principal</h1> :` Il s'agit du titre principal: Le titre le plus important est h1. Le moins important h6
* `<h2>Titre de section</h2> :`
* `<h3>Sous titre</h3> :`
* `<p> Ce ceci est une paragraphe. Je peux écrire ici autant que je veux.</p> :`C'est ici que l'on écrira nos paragraphes
* `<p>J'ai mis en <strong>gras</strong> le mot gras gros!</p> : `On peut mettre en gras avec la balise strong
* `<a href="https://www.ac-mayotte.fr/">Cliquz ici pour vous rendre sur le site de l'académie de Mayotte</a> : `On peut créer des lien cliquables avec la balise a. La première partie est le lien, la deuxième est la description du lien.
* `<img src="https://octodex.github.com/images/filmtocat.png" alt="Cette image représente un poulpe-chat." /> : `On peut aussi insérer une image: src est la source; alt est la description de l'image.

Clique sur `RUN` pour voir le résultat. Et lit les commentaires pour savoir à quoi sert chaque balise.
Tu peux recliquer sur `SUCCESS` autant de fois que nécessaire pour relancer la page.
Tu peux rajouter des titres de sections, des paragaphes, des liens, des images, tout ce qui te passe passe par la tête.

```html runnable
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  
</head>

<body>
    <h1>Titre principal</h1> 
    <h2>Titre de section</h2>
    <p> Ce ceci est une paragraphe. Je peux écrire ici autant que je veux.</p>
    <p>J'ai mis en <strong>gras</strong> le mot gras gros!</p>
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
-[ ] Hi Teacher MaouLida


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
<p>Nature, berce-leu chaudement: il a froid.</p>
```
?[Cette balise correspond à]
-[ ] Le titre
-[ ] Les lignes
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
<head></head>
```
?[Ce code html décrit]
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
?[Ce code html décrit]
-[ ] Du texte en gras.
-[ ] Un un lien hypertexte.
-[x] Au contenu visible par l'internaute.
-[ ] (^o^)   

---

# 4 Excercice d'application.
**A toi**<br/>
Complète la squelette ci-desssous en y ajoutant le titre de la page WEB:<br/>
**Je suis le titre le plus cool de l'histoire du WEB.**<br/>

Dans body, ajouter le texte suivant:<br/>
**Le WEB** (titre h1)<br/>
***Le berceau du WEB***(titre h2)<br/>
Le chercheur britannique Tim Berners-Lee a inventé le World Wide Web en 1989, lorsqu’il travaillait au CERN.
À l’origine, le projet a été conçu et développé pour que des scientifiques travaillant dans des universités du monde entier puissent s'échanger des informations instantanément.<br/>
***Le navigateur qui a rendu le WEB populaire***(Titre h2)<br/>
Le navigateur qui a rendu le WEB populaire est Mosaic. Il est née en 1993.
Ce navigateur a été publié en 1993 alors que le World Wide Web développé par le CERN ne comptait que 200 sites, 3 ans après son lancement.<br/>

***Ajouter un lien qui mène vers l'ENT NEO*** (https://mayotte.opendigitaleducation.com) <br/>
Pense à cliquer sur `RUN` pour voir le résultat.<br/>
Tu peux recliquer sur `SUCCESS` autant de fois que nécessaire pour relancer la page.

```html runnable
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  
</head>

<body>

</body>

</html>
```
