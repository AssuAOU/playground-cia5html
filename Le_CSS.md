# 1: Introduction: Qu'est-ce que le CSS?

Les **Cascading StyleSheets** — ou CSS — (Feuilles de style en cascade) sont la première technique à apprendre après le HTML.
Alors que HTML s'utilise pour définir la structure du contenu, les CSS sont employées pour composer et déterminer l'apparence de ce contenu.
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

Vérification de la compréhension du cours.

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
###### QCM 2
?[Le CSS permet de: ]
-[ ] -_-
-[ ] Convertir du binaire en décimal avec un navigateur WEB.
-[ ] Répartir une charge de manière uniforme.
-[x] Faire la mise en page et décorer une page WEB.

---
###### QCM 3
?[on peut utiliser le CSS sans HTML? ]
-[ ] ^-^
-[ ] OUI
-[x] NON
-[ ] ça dépend de la taille de la page WEB à créer.

---
###### QCM 4
?[On peut utiliser le HTML sans le CSS ]
-[ ] ^-^
-[ ] OUI
-[ ] NON
-[x] Techniquement oui, esthétiquement non ("La page sera moche<sup>100</sup>...")

---
# 2. Comment utiliser la feuille de style?
Dans ce tutoriel, nous partirons du code HTML ci-dessus et y appliquerons des CSS.
Il y'a plusieurs façon pour appliquer CSS à un document:

1. On peut écrire les règles `dans un fichier à part` et créer un lien vers la feuille de style CSS depuis l'en-tête (dans head) du document HTML.
2. On peut écrire les règles directement `dans le document HTML`.

Dans ce tutoriel, nous allons faire la **deuxième méthode** pour des questions pratique **MAIS** la première méthode est la plus utilisée et la plus "propre".

**Les deux méthodes sont détaillées dans l'annexe, à la fin de ce tutoriel.**


# 3. Mise en forme de notre page

## La couleur de fond et du texte.
On commencer par modifier la couleur de fond de la page WEB et la couleur de police.
On va mettre le fond en noir et le texte en blanc.
Cette action se fait avec le code suivant.
```html
body{
    color: white;
    background-color: black
  }
```

**A toi**<br>
Clique sur `RUN` pour voir le résultat.<br>
Ensuite, modifie le code pour afficher le texte en ***Rouge*** (red) et le fond en ***vert***(green).<br>
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
Si on veut que tous les titres (h1, h2 et h3) et tous les items de liste soient bleus, alors on écrira la règle suivante :
```html
h1, h2, h3, li {
        color: blue;
  }
```

**A toi**<br>
Clique sur `RUN` et observe le résultat.
Ensuite change la couleur des titres en Vert.

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
**Note importante:** Vous remarquerez que la première règles qu'on a écrit (font noir et texte en jaune) n'est plus totalement respectée.
En CSS, les règles sont appliquées les une à la suite des autres. Donc, si une règle vient contredire une autre, c'est la dernière qui est prise en compte.

## Ajouter une classe
Jusqu'ici, nous avons mis en forme des éléments HTML repérés par leur **nom de balise**.
Cela fonctionne tant que vous voulez appliquer **le même style à tous les éléments de ce type** dans le document.
La plupart du temps ce n'est pas le comportement désiré ;
il faut donc trouver une méthode pour sélectionner un sous-ensemble des éléments à mettre en forme sans changer l'apparence des autres éléments du même type.
L'approche la plus commune pour obtenir ce comportement est **d'ajouter une classe (pensez à une étiquette)** aux éléments HTML à mettre en forme puis de sélectionner cette classe.
Dans le document HTML, ajouter un  attribut class au 4eme item de la liste :
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
Dans le code CSS vous pouvez maintenant cibler la classe special grâce à un sélecteur fait du nom de la classe précédé d'un point.
Ajoutez le code suivant dans head :

```html
.special {
  color: orange;
  font-weight: bold;
}
```

**A toi**<br>
Cliquez sur `RUN` pour voir le résultat.
Puis rajoutez une classe que vous appelerez `internet` pour que seul l'item **"L'accès à Pronote et Néo"** soient en violet.


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
###### QCM 1
```html
body{
    color: purple;
    background-color: yellow
  }
```
?[Que fait ce code? ]
-[ ] ^-^
-[ ] Met  le fond en violet et la couleur de police en jaune
-[x] Met  le fond en jaune et la couleur de police en violet
-[ ] Permet de dire qu'il s'agit d'un code HTML (body)

---

###### QCM 2
 ```html
h1, h2, h3, li {
        color: blue;
  }
```
?[Que fait ce code? ]
-[ ] Programmer le déplacement des images.
-[x] Met les titres h1 en bleu
-[x] Met les titres h2 en bleu
-[ ] Met uniquement les titres h3 en bleu

---
###### QCM 3
?[A quoi sert une classe? ]
-[ ] Programmer le déplacement des images.
-[ ] appliquer le même style à tous les éléments de ce type
-[x] appliquer un style à un élément en particulier
-[ ] Classer le code par niveau

---
###### QCM 4
```html
.special {
  color: orange;
  font-weight: bold;
}
```
?[Que fait ce code? ]
-[ ] Indique une zone spéciale qui ne sera pas prise en compte par le navigateur.
-[ ] Appliquer le même style à tous les éléments de ce type
-[x] Met les élments de la classe special en orange et en gras.
-[ ] Indique la présence d'une ligne en orange.

---
###### QCM 4
?[Comment faire pour cibler une classe ]
-[ ] Il faut mettre le nom de la classe dans des balises.
-[ ] Il faut simplement écrire le nom de la classe.
-[x] Il faut écrire le nom de la classe précédé d'un point.
-[ ] Il faut mettre le nom de la classe en commentaire

---

# [Annexe] Comment utiliser la feuille de style?
Dans ce tutoriel, nous partirons du code HTML ci-dessus et y appliquerons des CSS.
Il y'a plusieurs façon pour appliquer CSS à un document:

1. On peut écrire les règles `dans un fichier à part` et créer un lien vers la feuille de style CSS depuis l'en-tête (dans head) du document HTML.
2. On peut écrire les règles directement `dans le document HTML`.

Dans ce tutoriel, nous allons faire la **deuxième méthode** pour des questions pratique **MAIS** la première méthode est la plus utilisée et la plus "propre".

#### Méthode 1
Voici comment appliquer cette méthode:

* Avec un éditeur de code(Block note, Notepad++,sublime Text), dans le dossier où se trouve le document HTML, créer un fichier et sauvegarder le sous le nom styles.css
L'extension .css indique que c'est un fichier CSS.

* Pour lier styles.css à index.html ajouter la ligne suivante dans la section <head> du document HTML :
```html
<link rel="stylesheet" href="styles.css">
```
Cet élément <link> indique au navigateur la présence d'une feuille de style, grâce à l'attribut rel ; la valeur de l'attribut href donne la localisation du fichier CSS.
Il ne reste plus qu'à ajouter les lignes de code à la feuille de style CSS.</br>

Et enfin, il suffira d'ajouter les règles de style dans le document styles.css les un à la suite des autres. Comme dans l'éxemple suivant, où on met les paragraphes en rouge.

```html
p{
  color: red;
  }
```

#### Méthode 2
Voici comment appliquer cette méthode:
Dans le document html, ajouter les lignes suivantes dans l'en-tête (dans "body").
```html
<style type="text/css">
    <!-- Zone de saisie des règles CSS-->
 </style>
```

Et écrire les règles dans la balise `<style></style>`.
Dans le code ci-après, l'ensemble des paragraphe seront écrits en rouge.

```html
 <style type="text/css">
    p {
        color: red;
    }
</style>
```
## Questionnaire QCM

Vérification de la compréhension du cours.

---
###### QCM 1
?[Est-ce que je peut faire du CSS et du HTML dans le même fichier? ]
-[ ] ^-^
-[x] OUI
-[ ] Qu'est-ce que le HTML et le CSS?
-[ ] NON

---
###### QCM 2
?[L'extension .css indique: ]
-[ ] -_-
-[ ] Qu'on peut faire du CSS et HTML dans ce fichier.
-[x] Qu'il s'agit d'un fichier CSS.
-[ ] Qu'on peut ranger ce fichier dans le dossier CSS.

---

###### QCM 3
```html
<link rel="stylesheet" href="styles.css">
```
?[Ce code doit être placé: ]
-[ ] -_-
-[ ] Dans body
-[x] Dans head
-[ ] Dans css

---

###### QCM 4
```html
<link rel="stylesheet" href="styles.css">
```
?[A quoi sert ce code? ]
-[ ] -_-
-[x] Il indique au navigateur la présence d'une feuille de style
-[ ] Il indique au navigateur un fichier corrompu
-[ ] Il sert à décorer le code HTML

---

###### QCM 5
```html
<link rel="stylesheet" href="styles.css">
```
?[A quoi sert l'attribut href? ]
-[ ] -_-
-[x] Indique le nom (ou chemin) du fichier CSS.
-[ ] Indique le style du CSS.
-[ ] Indique la hauteur de la référence styles.css

---



# Sources
<https://developer.mozilla.org/fr/docs/Learn/CSS/First_steps/Getting_started>