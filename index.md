<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfolio de Max Zargha</title>
    <link href="https://fonts.googleapis.com/css2?family=Nunito:wght@400;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Nunito', sans-serif; /* Utilisation d'une police plus moderne */
            margin: 0;
            padding: 0;
            background: #f4f4f4;
            color: #333;
        }

        header {
            background: #fff;
            padding: 20px 0;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            text-align: center;
        }

        .header-image {
            max-width: 180px; /* Taille plus appropriée pour l'en-tête */
            height: auto;
        }

        .carousel {
            width: 80%;
            overflow: hidden;
            margin: 50px auto;
            position: relative;
            box-shadow: 0 5px 15px rgba(0,0,0,0.15);
        }

        .carousel-container {
            display: flex;
            transition: transform 0.5s ease;
            will-change: transform;
        }

        .carousel-item {
            flex: 0 0 100%;
        }

        .carousel-item img {
            width: 100%;
            height: auto;
            display: block;
        }

        #gallery h2 {
            text-align: center;
            margin: 40px 0;
        }
    </style>
    <script>
        document.addEventListener("DOMContentLoaded", function() {
            const container = document.getElementById("carouselContainer");
            let currentIndex = 0;

            function nextImage() {
                const totalItems = container.children.length;
                currentIndex = (currentIndex + 1) % totalItems;
                container.style.transform = `translateX(-${100 * currentIndex}%)`;
            }

            container.addEventListener('click', nextImage);
        });
    </script>
</head>
<body>
    <header>
        <img src="zargha_site.jpg" alt="Logo de Max Zargha" class="header-image">
    </header>

    <section id="bio">
        <h1>Max Zargha</h1>
        <p>Artiste franco-iranien diplômé de l’Université Paris 8 dans le domaine des arts. À travers ses collages, Max cherche à intriguer, politiser, et illustrer la dualité du monde et des inégalités sociologiques, tout en explorant les énergies subtiles de l’être humain inspiré par le surréalisme.</p>
    </section>

    <section id="gallery">
        <h2>Galerie</h2>
        <div class="carousel">
            <div class="carousel-container" id="carouselContainer">
                <div class="carousel-item">
                    <img src="Colonel.jpg" alt="Colonel">
                </div>
                <div class="carousel-item">
                    <img src="L'Autel.jpg" alt="L'Autel">
                </div>
                <div class="carousel-item">
                    <img src="Le Chirurgien.jpg" alt="Le Chirurgien">
                </div>
                <div class="carousel-item">
                    <img src="Surréalisme.jpg" alt="Surréalisme">
                </div>
                <div class="carousel-item">
                    <img src="Tristesse.jpg" alt="Tristesse">
                </div>
            </div>
        </div>
    </section>
</body>
</html>
