<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Galerie de Max Zargha</title>
    <style>
        /* Réinitialiser les marges et les paddings */
        body, html {
            margin: 0;
            padding: 0;
        }

        /* Style pour l'image d'en-tête */
        .header-image {
            display: block;
            margin: 0 auto; /* Centre l'image horizontalement */
            max-width: 100%; /* Assure que l'image ne dépasse pas la largeur de l'écran */
            height: auto; /* Maintient le ratio de l'image */
            width: 50%; /* Réduit la taille de l'image à 50% de sa largeur originale */
        }

        /* Styles pour le carrousel */
        .carousel {
            width: 60%;
            overflow: hidden;
            margin: 20px auto; /* Ajustement de la marge pour une meilleure présentation */
            position: relative;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
        }

        .carousel-container {
            display: flex;
            transition: transform 1s ease;
            cursor: pointer; /* Indique que les éléments sont cliquables */
        }

        .carousel-item {
            flex: 0 0 100%; /* Chaque item prend 100% de la largeur du carousel */
        }

        .carousel-item img {
            width: 100%;
            height: auto;
            display: block;
        }
    </style>
</head>
<body>
    <!-- En-tête de la page avec image -->
    <img src="zargha site.jpg" class="header-image" alt="En-tête Max Zargha">

    <!-- Carrousel d'images -->
    <div class="carousel" onclick="nextImage()">
        <div class="carousel-container" id="carouselContainer">
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

    <script>
        var currentIndex = 0;
        function nextImage() {
            var container = document.getElementById("carouselContainer");
            var totalItems = container.children.length;
            currentIndex = (currentIndex + 1) % totalItems; // Cela permet de boucler le carrousel
            var newTranslateValue = -100 * currentIndex;
            container.style.transform = `translateX(${newTranslateValue}%)`;
        }
    </script>
</body>
</html>
