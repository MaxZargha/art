<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfolio de Max Zargha</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Roboto', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f0f0f0;
            color: #333;
        }

        header {
            background: #ffffff;
            padding: 10px 0;
            text-align: center;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
        }

        .header-image {
            width: 150px; /* Adjusted image size for a better fit */
            height: auto;
            margin: 0 auto; /* Centering the image horizontally */
        }

        .content {
            padding: 20px;
            text-align: center;
        }

        .content h1 {
            color: #2c3e50;
        }

        .content p {
            font-size: 18px;
            line-height: 1.6;
        }

        .gallery {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            padding: 20px;
        }

        .gallery img {
            width: 30%; /* Consistent size for all images */
            margin-bottom: 20px;
        }

        @media (max-width: 600px) {
            .gallery img {
                width: 100%;
            }
        }
    </style>
</head>
<body>
    <header>
        <img src="zargha_site.jpg" class="header-image">
    </header>
    <div class="content">
        <h1>Max Zargha</h1>
        <p>Artiste franco-iranien diplômé de l’Université Paris 8, explorant la dualité du monde à travers le surréalisme.</p>
    </div>
    <div class="gallery">
        <img src="Colonel.jpg" alt="Colonel">
        <img src="L'Autel.jpg" alt="L'Autel">
        <img src="Le Chirurgien.jpg" alt="Le Chirurgien">
        <img src="Surréalisme.jpg" alt="Surréalisme">
        <img src="Tristesse.jpg" alt="Tristesse">
    </div>
</body>
</html>
