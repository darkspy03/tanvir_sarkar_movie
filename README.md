# tanvir_sarkar_movie
all movies downloads 
<all movies here>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rotating Name & Stylish Links</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
        }

        body {
            background-color: #1a1a1a;
            color: white;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
        
        }

        @keyframes rotateName {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }

        @keyframes glowEffect {
            0% { text-shadow: 0 0 10px #ff0000, 0 0 20px #ff7300, 0 0 30px #fffb00; }
            100% { text-shadow: 0 0 15px #ff7300, 0 0 25px #fffb00, 0 0 35px #48ff00; }
        }

        /* LINKS SECTION */
        h2 {
            font-size: 24px;
            margin-bottom: 20px;
        }

        .links-container {
            display: flex;
            flex-direction: column;
            gap: 15px;
        }

        .link-button {
            text-decoration: none;
            color: white;
            background: linear-gradient(45deg, #ff416c, #ff4b2b);
            padding: 15px 30px;
            border-radius: 10px;
            font-size: 20px;
            font-weight: bold;
            text-align: center;
            transition: 0.3s;
            display: inline-block;
            width: 250px;
            text-transform: uppercase;
            box-shadow: 0 4px 10px rgba(255, 75, 43, 0.5);
        }

        .link-button:hover {
            transform: scale(1.1);
            box-shadow: 0 6px 15px rgba(255, 75, 43, 0.7);
        }

        .link-button:nth-child(2) {
            background: linear-gradient(45deg, #2193b0, #6dd5ed);
        }

        .link-button:nth-child(3) {
            background: linear-gradient(45deg, #ff9a9e, #fad0c4);
        }

        .link-button:nth-child(4) {
            background: linear-gradient(45deg, #ff512f, #dd2476);
        }
    </style>
</head>
<body>
    <!-- Rotating Name -->
    <div class="name">TAN</div>

    <!-- Links Section -->
    <h2>Welcome to TANVIR Movies Download</h2>
    <div class="links-container">
        <a href="https://filmyfly.phd/" class="link-button" target="_blank">FilmyFly</a>
        <a href="https://filmyworlds.christmas/" class="link-button" target="_blank">Filmy World</a>
        <a href="https://vegamovies.rs/" class="link-button" target="_blank">Vega Movies</a>
        <a href="https://bollyflix.kids/" class="link-button" target="_blank">Bolly Flix</a>
    </div>
</body>
</html>
