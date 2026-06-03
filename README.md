<!DOCTYPE html>
<html lang="nl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfolio</title>
    <style>
        /* Schone basisinstellingen */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            background-color: #000000; /* Gitzwarte achtergrond */
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
            color: #ffffff;
        }

        /* Extreem minimalistisch menu linksboven */
        nav {
            position: fixed;
            top: 30px;
            left: 30px;
            z-index: 1000;
        }
        nav a {
            color: #ffffff;
            text-decoration: none;
            font-size: 14px;
            font-weight: 400;
            letter-spacing: 1px;
            margin-right: 20px;
            text-transform: lowercase;
            opacity: 0.7;
            transition: opacity 0.3s;
        }
        nav a:hover {
            opacity: 1; /* Licht op als je eroverheen beweegt */
        }

        /* Video container - beeldvullend onder elkaar */
        .video-container {
            width: 100vw;
            height: 100vh; /* Precies schermvullend per video */
            position: relative;
            border-bottom: 2px solid #ffffff; /* De strakke witte lijn */
            overflow: hidden;
        }
        /* Zorgt dat de video de hele achtergrond vult */
        .video-container iframe {
            position: absolute;
            top: 50%;
            left: 50%;
            width: 100vw;
            height: 56.25vw; /* 16:9 verhouding */
            min-height: 100vh;
            min-width: 177.77vh; /* 16:9 verhouding */
            transform: translate(-50%, -50%);
            border: none;
        }
    </style>
</head>
<body>

    <!-- Het Minimalistische Menu -->
    <nav>
        <a href="#work">work</a>
        <a href="#about">about</a>
        <a href="#contact">contact</a>
    </nav>

    <!-- Beeldvullende Video 1 (Voorbeeld) -->
    <div class="video-container" id="work">
        <iframe src="https://youtube.com" allow="autoplay; encrypted-media" allowfullscreen></iframe>
    </div>

    <!-- Beeldvullende Video 2 (Voorbeeld) -->
    <div class="video-container">
        <iframe src="https://youtube.com" allow="autoplay; encrypted-media" allowfullscreen></iframe>
    </div>

</body>
</html>
