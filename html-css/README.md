# HTML & CSS - INTRODUCTION

## Prerequisite
- IDE (recommended : [Visual Studio Code](https://code.visualstudio.com/))
- Web Browser (recommended : [Google Chrome](https://www.google.com/intl/fr_fr/chrome/))

## Languages
- [HTML](https://fr.wikipedia.org/wiki/Hypertext_Markup_Language) (HyperText Markup Language)
- [CSS](https://fr.wikipedia.org/wiki/Feuilles_de_style_en_cascade) (Cascading Style Sheets)

## Resources
### Documentations
- [Mozilla - HTML](https://developer.mozilla.org/fr/docs/Web/HTML)
- [Mozilla - CSS](https://developer.mozilla.org/fr/docs/Web/CSS)
### Class & Tutorials
- [W3schools - HTML](https://www.w3schools.com/html/)
- [W3schools - CSS](https://www.w3schools.com/css/)
- [OpenClassrooms - HTML & CSS (fr)](https://openclassrooms.com/fr/courses/1603881-apprenez-a-creer-votre-site-web-avec-html5-et-css3)
- [OpenClassrooms - HTML & CSS (en)](https://openclassrooms.com/en/courses/5265446-build-your-first-web-pages-with-html-and-css)
### Forum
- [Stackoverflow](https://stackoverflow.com/)

# HTML - FUNDAMENTALS
- Balises
- Attributs
- Doctype, Html, Head, Body, Title
- Commentaire, Indentation
```html
<!DOCTYPE html>

<html>

    <head>
        <!-- page header -->
        <meta charset="utf-8" />
        <title>Titre</title>
    </head>

    <body>
    </body>

</html>
```

## Balises
### les titres
```html
<h1>Titre super important</h1>
<h2>Titre important</h2>
<h3>Titre un peu moins important (sous-titre)</h3>
```

### Les paragraphes
```html
<p>Ceci est un paragraphe</p>
```

### Mettre l'emphase
```html
<p>
    ceci est une phrase <em>volontairement longue</em>
    pour avoir l'opportunité de <strong>mettre en valeur</strong>
    certains mots pour voir un peu comment le <mark>html</mark> les gère.
</p>
```

### Les listes
```html
<ul>
    <li>Premier élément de la liste</li>
    <li>Deuxième élément de la liste</li>
    <li>Troisième élément de la liste</li>
</ul>
```

## Attributs
### Les liens
- La balise <a>
- L’attribut href
- Particularité des liens (bleu, sous-ligné, pointer)
- Les liens absolus
- Les liens relatifs
- Les ancres
- Autres utilisations (téléchargements, nouvel onglet, etc.)
```html
<p>
    <a href="http://www.google.fr" >Ceci est un lien vers GOOGLE</a>
</p>

<p>
    Cliquez <a href="./page2.html">ici</a> pour accèder à la page 2
</p>

<h1 id="ancre1">Titre</h1>
<!-- ... -->
<a href="#ancre1">Revenir au titre</a>
```

### Les images
- La balise <img>
- Attributs :
    - src : le lien de l’image
    - alt : une description de celle-ci
- Format :
    - Une photo : JPEG
    - Un graphique : PNG

```html
<img src="./image.jpg" alt="la description de l'image" />
```

# CSS - FUNDAMENTALS
## Les sélecteurs
```html
<h1>Titre en rouge, italique</h1>
<h1>Titre en bleu, italique, souligné</h1>
<h1>Titre en vert, souligné </h1>
```
```html
<h1 id="title-id-1" class="title-class-1">Titre en rouge, italique</h1>
<h1 id="title-id-2" class="title-class-1 title-class-2">Titre en bleu, italique, souligné</h1>
<h1 id="title-id-3" class="title-class-2">Titre en vert, souligné </h1>
```
- balise
```css
h1 {
    font-family: monospace;
}
```
- class
```css
.title-class-1 {
    font-style: italic;
}
.title-class-2 {
    text-decoration: underline;
}
```
- id
```css
#title-id-1 {
    color: red;
}
#title-id-2 {
    color: blue;
}
#title-id-3 {
    color: green;
}
```

## Ajouter son CSS au HTML
- comme attribut
```html
<h1 style="color:red;">Titre en rouge</h1>
```
- dans une balise de style
```html
<style>
    h1 {
        color: red;
    }
</style>
<h1>Titre en rouge</h1>
```
- nouveau fichier CSS
```css
h1 {
    color: red;
}
```
```html
<html>
    <head>
        <link rel="stylesheet" href="main.css" />
    </head>

    <body>
        <h1>Titre en rouge</h1>
    </body>

</html>
```

## Flexbox
- overview / démo : main2.html
- [explications & tuto](https://openclassrooms.com/fr/courses/1603881-apprenez-a-creer-votre-site-web-avec-html5-et-css3/3298561-faites-votre-mise-en-page-avec-flexbox)
- [mini-jeux](https://flexboxfroggy.com/)