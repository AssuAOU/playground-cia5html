# 1: Introduction: Qu'est-ce que le CSS?

Les **Cascading StyleSheets** — ou CSS — (Feuilles de style en cascade) sont les premières techniques à apprendre après le HTML.
Alors que le HTML s'utilise pour définir la structure du contenu, les CSS sont employées pour composer et déterminer l'apparence de ce contenu.
Ainsi par exemple, vous utiliserez les CSS pour modifier les POLICE, la `couleur`, la taille et l'e s p a c e m e n t de votre contenu,
pour le répartir sur plusieurs colonnes ou bien pour ajouter des animations et autres fonctionnalités décoratives.    

Nous allons ajouter du style à la page suivante. Cliquez sur `RUN` pour voir le résultat.
```html runnable
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>Bienvenue à la cité scolaire</title>
</head>

<body>
    <!-- Menu de navigation du site-->
    <ul class="navbar">
        <li>Accueil</li>
        <li>Actualité</li>
        <li>La cité scolaire</li>
        <li>Classes et options</li>
        <li>Examens</li>
        <li>L'accès à Pronote et NEO</li>
    </ul>
    <img src="https://cdn.pixabay.com/photo/2017/07/04/10/07/board-2470557_960_720.jpg" alt="Never Give up" />
    <h1>Accueil</h1> 
    <h1>Bienvenue à la cité scolaire</h1> 
    <h3>Horaires</h3>
    <p> La cité sclaire est ouverte du lundi au samedi. Pour joindre l'accueil, il faut composer le 0269 70 71 72</p>
    <p>En cas d'urgence, contacter le <strong>06 39 40 41 42</strong>.</p>
   
   <!--Signature -->
   <adress>Site crée en Mars 2020 par les classes de 2nd A et B.</adress><br>

    <a href="https://www.ac-mayotte.fr/">Cliquz ici pour vous rendre sur le site de l'académie de Mayotte</a>.
</body>

</html>
```
**Vous remarquerez que la page n'est pas très belle. Nous allons faire la mise en page de notre page avec le CSS.(^-^)**

## Questionnaire QCM

Voici quelques QCM pour voir si tu as bien compris. N'hésite pas à relire ce qui précède si tu as un doute.

---
###### QCM 1
?[Que veut dire CSS? ]
-[ ] ^-^
-[x] Cascading StyleSheets
-[ ] Caisse de Sécurité Sociale
-[ ] Cours de Style Sécurisé

---
###### QCM 2
?[Comment peut-on traduire CSS en français ? ]
-[ ] ^ ^
-[ ] Caisse de Sécurité Sociale
-[x] Feuilles de style en cascade
-[ ] Feuilles de Mise en page

---
###### QCM 3
?[Le CSS permet de: ]
-[ ] -_-
-[ ] Convertir du binaire en décimal avec un navigateur WEB.
-[ ] Répartir une charge de manière uniforme.
-[x] Faire la mise en page et décorer une page WEB.

---
###### QCM 4
?[Peut-on utiliser le CSS sans HTML? ]
-[ ] ^-^
-[ ] OUI
-[x] NON
-[ ] ça dépend de la taille de la page WEB à créer.

---
###### QCM 5
?[On peut utiliser le HTML sans le CSS ]
-[ ] ^-^
-[ ] OUI
-[ ] NON
-[x] Techniquement oui, esthétiquement non ("La page sera moche<sup>100</sup>...")

---
# 2. Comment utiliser la feuille de style?
Dans ce tutoriel, nous partirons du code HTML ci-dessus et y appliquerons des règles de CSS.
Il y'a plusieurs façon pour appliquer les règles de CSS à un document:

1. On peut écrire les règles `dans un fichier à part` et créer un lien vers la feuille de style CSS depuis l'en-tête (dans head) du document HTML.
2. On peut écrire les règles directement `dans le document HTML`.

Dans ce tutoriel, nous allons faire la **deuxième méthode** pour des questions pratiques **MAIS** la première méthode est la plus utilisée et la plus "propre".

#### Méthode 1
Voici comment appliquer cette méthode:

* Avec un éditeur de code(Bloc-notes, Notepad++,sublime Text), dans le dossier où se trouve le document HTML, créer un fichier et sauvegarder le sous le nom **styles.css**
L'extension **.css** indique que c'est un **fichier CSS**.

* Pour lier le fichier **styles.css** à au fichier **index.html**, il faut ajouter la ligne suivante dans la section <head> du document HTML :
```html
<link rel="stylesheet" href="styles.css">
```
Cet élément `<link>` indique au navigateur la présence d'une feuille de style, grâce à l'attribut **rel** ; la valeur de l'attribut **href** donne la localisation du fichier CSS.

Et enfin, il suffira d'ajouter les règles de style dans le document **styles.css** les unes à la suite des autres.
Comme dans l'éxemple suivant, où l'on met les paragraphes en rouge.

```html
p{
  color: red;
  }
```

#### Méthode 2
Voici comment appliquer cette méthode:
Dans le document .html, il faut ajouter les lignes suivantes dans l'en-tête (dans "body").
```html
<style type="text/css">
    <!-- Zone de saisie des règles CSS-->
 </style>
```

Et écrire les règles suivantes dans la balise `<style></style>`.
Dans le code suivant, l'ensemble des paragraphes seront écrits en rouge.

```html
 <style type="text/css">
    p {
        color: red;
    }
</style>
```
## Questionnaire QCM

Voici quelques QCM pour voir si tu as bien compris. N'hésite pas à relire ce qui précède si tu as un doute.

---
###### QCM 6
?[Est-ce que je peux faire du CSS et du HTML dans le même fichier? ]
-[ ] ^-^
-[x] OUI
-[ ] Qu'est-ce que le HTML et le CSS?
-[ ] NON

---
###### QCM 7
?[L'extension **.css** indique: ]
-[ ] -_-
-[ ] Qu'on peut faire du CSS et HTML dans ce fichier.
-[x] Qu'il s'agit d'un fichier CSS.
-[ ] Que l'on peut ranger ce fichier dans le dossier CSS.

---

###### QCM 8
```html
<link rel="stylesheet" href="styles.css">
```
?[Ce code doit être placé: ]
-[ ] -_-
-[ ] Dans les balises **body.**
-[x] Dans les balises **head.**
-[ ] Dans les balises **css.**

---

###### QCM 9
```html
<link rel="stylesheet" href="styles.css">
```
?[A quoi sert ce code? ]
-[ ] -_-
-[x] Il indique au navigateur la présence d'une feuille de style.
-[ ] Il indique au navigateur un fichier corrompu.
-[ ] Il sert à décorer le code HTML.

---

###### QCM 10
```html
<link rel="stylesheet" href="styles.css">
```
?[A quoi sert l'attribut **href**? ]
-[ ] -_-
-[x] Indique le nom (ou chemin) du fichier CSS.
-[ ] Indique le style du CSS.
-[ ] Indique la hauteur de la référence **styles.css.**

---


# 3. Mise en forme de notre page

## La couleur de fond et du texte.
On va commencer par modifier la couleur de fond de la page WEB et la couleur de police.
On va mettre le fond en noir et le texte en blanc.
Cette action se fait avec le code suivant:

```html
body{
    color: white;
    background-color: black
  }
```

**A toi**<br>
Clique sur `RUN` pour voir le résultat.<br>
Ensuite, modifie le code pour afficher le texte en ***rouge*** (red) et le fond en ***vert***(green).<br>
Clique sur `SUCCESS` pour relancer la page et voir le résultat.

```html runnable
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>Bienvenue à la cité scolaire</title>
 
  <style type="text/css">
  body{
    color: yellow;
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
    <img src="https://cdn.pixabay.com/photo/2017/07/04/10/07/board-2470557_960_720.jpg" alt="Never Give up" />
    <h1>Accueil</h1> 
    <h1>Bienvenue à la cité scolaire</h1> 
    <h3>Horaires</h3>
    <p> La cité sclaire est ouverte du lundi au samedi. Pour joindre l'accueil, il faut composer le 0269 70 71 72</p>
    <p>En cas d'urgence, contacter le <strong>06 39 40 41 42</strong>.</p>
   
   <!--Signature -->
   <adress>Site crée en Mars 2020 par les classes de 2nd A et B.</adress><br>

    <a href="https://www.ac-mayotte.fr/">Cliquz ici pour vous rendre sur le site de l'académie de Mayotte</a>.
</body>

</html>
```
## Les titres
On va ensuite changer la couleur des titres. En CSS, on peut cibler plusieurs éléments d'un coup en les listant, séparés par une virgule.
Si on veut que tous les titres (h1, h2 et h3) et tous les éléments d'une liste soient en bleus, alors on écrira la règle suivante :

```html
h1, h2, h3, li {
        color: blue;
  }
```

**A toi**<br>
Clique sur `RUN` et observe le résultat.
Ensuite change la couleur des titres en **vert**; la liste reste en bleu.

```html runnable
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>Bienvenue à la cité scolaire</title>
 
  <style type="text/css">
  body{
    color: yellow;
    background-color: black
  }
  
  h1, h2, h3, li {
        color: blue;
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
    <img src="https://cdn.pixabay.com/photo/2017/07/04/10/07/board-2470557_960_720.jpg" alt="Never Give up" />
    <h1>Accueil</h1> 
    <h2>Bienvenue à la cité scolaire</h2> 
    <h3>Horaires</h3>
    <p> La cité sclaire est ouverte du lundi au samedi. Pour joindre l'accueil, il faut composer le 0269 70 71 72</p>
    <p>En cas d'urgence, contacter le <strong>06 39 40 41 42</strong>.</p>
   
   <!--Signature -->
   <adress>Site crée en Mars 2020 par les classes de 2nd A et B.</adress><br>

    <a href="https://www.ac-mayotte.fr/">Cliquz ici pour vous rendre sur le site de l'académie de Mayotte</a>.
</body>

</html>
```
**Note importante:** Vous remarquerez que la première règles qu'on a écrit (fond noir et texte en jaune) n'est plus totalement respectée.
En CSS, les règles sont appliquées **les une à la suite des autres**. Donc, si une règle vient contredire une autre, c'est la dernière qui est prise en compte.

## Ajouter une classe
Jusqu'ici, nous avons mis en forme des éléments HTML repérés par leur **nom de balise**.
Cela fonctionne tant que tu veux appliquer **le même style à tous les éléments de ce type** dans le document.
La plupart du temps ce n'est pas le comportement désiré ;
il faut donc trouver une méthode pour sélectionner un sous-ensemble des éléments à mettre en forme sans changer l'apparence des autres éléments du même type.
L'approche la plus commune pour obtenir ce comportement est **d'ajouter une classe (pensez à une étiquette)** aux éléments HTML à mettre en forme puis de sélectionner cette classe.

Nous allons donc ajouter une classe dans notre document HTML.
Dans notre document HTML, nous allons donc ajouter un  attribut **class** au 4eme élément de la liste :
```html
<ul>
        <li>Accueil</li>
        <li>Actualité</li>
        <li>La cité scolaire</li>
        <li class="special">Classes et options</li> 
        <li>Examens</li>
        <li>L'accès à Pronote et NEO</li>
    </ul>
```
Ensuite, dans la balise **style**, nous pouvons maintenant cibler la classe **special** grâce à un sélecteur constitué du **nom de la classe précédé d'un point.**
Ce qui donne le code suivant :

```html
.special {
  color: orange;
  font-weight: bold;
}
```

Le résultat final se trouve dans le code suivant, où tu peux remarquer les deux ajouts cités plus haut.

**A toi**<br>
Clique sur `RUN` pour voir le résultat.
Puis rajoute une classe que tu appeleras `internet` pour que seul l'élément **"L'accès à Pronote et Néo"** soit en violet.

```html runnable
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>Bienvenue à la cité scolaire</title>
 
  <style type="text/css">
  body{
        color: yellow;
        background-color: black
  }
  
  h1, h2, h3, li {
        color: blue;
  }
    
  .special {
        color: orange;
        font-weight: bold;
    }
  
 </style>
</head>

<body>
    <!-- Menu de navigation du site-->
    <ul>
        <li>Accueil</li>
        <li>Actualité</li>
        <li>La cité scolaire</li>
        <li class="special">Classes et options</li>
        <li>Examens</li>
        <li>L'accès à Pronote et NEO</li>
    </ul>
    <img src="https://cdn.pixabay.com/photo/2017/07/04/10/07/board-2470557_960_720.jpg" alt="Never Give up" />
    <h1>Accueil</h1> 
    <h2>Bienvenue à la cité scolaire</h2> 
    <h3>Horaires</h3>
    <p> La cité sclaire est ouverte du lundi au samedi. Pour joindre l'accueil, il faut composer le 0269 70 71 72</p>
    <p>En cas d'urgence, contacter le <strong>06 39 40 41 42</strong>.</p>
   
    <!--Signature -->
    <adress>Site crée en Mars 2020 par les classes de 2nd A et B.</adress><br>

    <a href="https://www.ac-mayotte.fr/">Cliquez ici pour vous rendre sur le site de l'académie de Mayotte</a>.
</body>

</html>
```

## Questionnaire QCM

Voici quelques QCM pour voir si tu as bien compris. N'hésite pas à relire ce qui précède si tu as un doute.

---
###### QCM 11
```html
body{
    color: purple;
    background-color: yellow
  }
```
?[Que fait ce code? ]
-[ ] ^-^
-[ ] Met le fond en violet et la couleur de police en jaune.
-[x] Met le fond en jaune et la couleur de police en violet.
-[ ] Permet de dire qu'il s'agit d'un code HTML (body).

---

###### QCM 12
 ```html
h1, h2, h3, li {
        color: blue;
  }
```
?[Que fait ce code?(Plusieurs choix possibles) ]
-[ ] Programme le déplacement des images.
-[x] Met les titres h1 en bleu.
-[x] Met les titres h2 en bleu.
-[ ] Met uniquement les titres h3 en bleu.

---
###### QCM 13
?[A quoi sert une classe? ]
-[ ] A programmer le déplacement des images.
-[ ] A apppliquer le même style à tous les éléments de ce type.
-[x] A appliquer un style à un élément en particulier.
-[ ] A classer le code par niveau.

---
###### QCM 14
```html
.special {
  color: orange;
  font-weight: bold;
}
```
?[Que fait ce code? ]
-[ ] Indique une zone spéciale qui ne sera pas prise en compte par le navigateur.
-[ ] Applique le même style à tous les éléments de ce type
-[x] Met les élments de la classe special en orange et en gras.
-[ ] Indique la présence d'une ligne en orange.

---
###### QCM 15
?[Comment faire pour cibler une classe ]
-[ ] Il faut mettre le nom de la classe dans des balises.
-[ ] Il faut simplement écrire le nom de la classe.
-[x] Il faut écrire le nom de la classe précédé d'un point.
-[ ] Il faut mettre le nom de la classe en commentaire

---

# Sources
<https://developer.mozilla.org/fr/docs/Learn/CSS/First_steps/Getting_started>