<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>En-tête avec Image</title>
    <style>
        .header-image {
            display: block;
            margin: 0 auto; /* Centre l'image horizontalement */
            max-width: 100%; /* Assure que l'image ne dépasse pas la largeur de l'écran */
            height: auto; /* Maintient le ratio de l'image */
            width: 30%; /* Réduit la taille de l'image à 50% de sa largeur originale */
        }
    </style>
</head>
<body>
    <img src="zargha site.jpg" class="header-image">
</body>
</html>



[Link to another page](./another-page.html).


# Bio

Max Zargha est un artiste franco-iranien diplômé de l’Université Paris 8 dans le domaine des arts. À travers ses collages, plusieurs intentions se manifestent : Celle de vouloir intriguer le spectateur jusqu'à esquisser un sourire sur son visage. Il lui arrive également de vouloir politiser son œuvre avec une conscience moralisatrice ; il aime aussi montrer la dualité de notre monde ainsi que nos propres inégalités sociologiques. Lorsqu'il laisse parler son inspiration sur tablette graphique, il n’a de cesse de découvrir de nouvelles techniques pour tenter de mettre en visuel les énergies subtiles et inconscientes de l’être humain. Fortement inspiré par les surréalistes, il illustre en globalité des êtres vivants, avec pour idée fixe de représenter leurs spectres énergétiques en liquéfaction.

## Galerie

<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <title>Galerie d'images défilante</title>
    <style>
        .carousel {
            width: 80%; /* Largeur du carrousel */
            overflow: hidden; /* Cache les images non visibles */
            margin: 20px auto; /* Centre le carrousel */
        }

        .carousel-container {
            display: flex; /* Affichage en ligne des images */
            width: 500%; /* 5 fois la largeur du carrousel pour contenir toutes les images */
            animation: slide 20s infinite; /* Animation définie ci-dessous */
        }

        .carousel-item {
            width: 20%; /* Chaque image utilise 20% de l'espace (pour 5 images) */
            flex-shrink: 0; /* Empêche le redimensionnement des images */
        }

        .carousel-item img {
            width: 100%; /* Adapte l'image à la largeur disponible */
            height: auto; /* Maintient le ratio */
        }

        /* Keyframes pour l'animation de défilement */
        @keyframes slide {
            0% { transform: translateX(0); }
            20% { transform: translateX(0); }
            25% { transform: translateX(-100%); }
            45% { transform: translateX(-100%); }
            50% { transform: translateX(-200%); }
            70% { transform: translateX(-200%); }
            75% { transform: translateX(-300%); }
            95% { transform: translateX(-300%); }
            100% { transform: translateX(-400%); }
        }
    </style>
</head>
<body>
    <div class="carousel">
        <div class="carousel-container">
            <div class="carousel-item">
                <img src="Colonel.jpg" alt="Image 1">
            </div>
            <div class="carousel-item">
                <img src="L'Autel.jpg" alt="Image 2">
            </div>
            <div class="carousel-item">
                <img src="Le Chirurgien.jpg" alt="Image 3">
            </div>
            <div class="carousel-item">
                <img src="Surréalisme.jpg" alt="Image 4">
            </div>
            <div class="carousel-item">
                <img src="Tristesse.jpg" alt="Image 5">
            </div>
        </div>
    </div>
</body>
</html>


### Header 3

```js
// Javascript code with syntax highlighting.
var fun = function lang(l) {
  dateformat.i18n = require('./lang/' + l)
  return true;
}
```

```ruby
# Ruby code with syntax highlighting
GitHubPages::Dependencies.gems.each do |gem, version|
  s.add_dependency(gem, "= #{version}")
end
```

#### Header 4

*   This is an unordered list following a header.
*   This is an unordered list following a header.
*   This is an unordered list following a header.

##### Header 5

1.  This is an ordered list following a header.
2.  This is an ordered list following a header.
3.  This is an ordered list following a header.

###### Header 6

| head1        | head two          | three |
|:-------------|:------------------|:------|
| ok           | good swedish fish | nice  |
| out of stock | good and plenty   | nice  |
| ok           | good `oreos`      | hmm   |
| ok           | good `zoute` drop | yumm  |

### There's a horizontal rule below this.

* * *

### Here is an unordered list:

*   Item foo
*   Item bar
*   Item baz
*   Item zip

### And an ordered list:

1.  Item one
1.  Item two
1.  Item three
1.  Item four

### And a nested list:

- level 1 item
  - level 2 item
  - level 2 item
    - level 3 item
    - level 3 item
- level 1 item
  - level 2 item
  - level 2 item
  - level 2 item
- level 1 item
  - level 2 item
  - level 2 item
- level 1 item

### Small image

![Octocat](https://github.githubassets.com/images/icons/emoji/octocat.png)

### Large image

![Branching](https://guides.github.com/activities/hello-world/branching.png)


### Definition lists can be used with HTML syntax.

<dl>
<dt>Name</dt>
<dd>Godzilla</dd>
<dt>Born</dt>
<dd>1952</dd>
<dt>Birthplace</dt>
<dd>Japan</dd>
<dt>Color</dt>
<dd>Green</dd>
</dl>

```
Long, single-line code blocks should not wrap. They should horizontally scroll if they are too long. This line should be long enough to demonstrate this.
