# VortexDrift.Github.io
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vortex Drift - PC Games</title>
    <style>
        /* Global Styles */
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background-color: black;
            color: white;
        }

        /* Header */
        header {
            background-color: lightblue;
            padding: 20px;
            text-align: center;
        }

        header img {
            max-width: 200px;
            background-color: transparent; /* Make the background transparent */
        }

        /* Main Content */
        .container {
            display: flex;
            flex-direction: column;
            align-items: center;
            margin-top: 40px;
        }

        .title {
            font-size: 3rem;
            color: yellow;
            text-shadow: 2px 2px 5px black;
        }

        .games-list {
            display: flex;
            flex-direction: column;
            gap: 20px;
            margin-top: 20px;
        }

        .game-item {
            background-color: lightblue;
            padding: 15px;
            border-radius: 10px;
            width: 300px;
            text-align: center;
            color: black;
            font-size: 1.2rem;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.5);
        }

        .game-item:hover {
            background-color: yellow;
            color: black;
            cursor: pointer;
        }

        /* Buttons */
        button {
            background-color: yellow;
            color: black;
            border: none;
            padding: 10px 20px;
            border-radius: 5px;
            font-size: 1rem;
            cursor: pointer;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.2);
        }

        button:hover {
            background-color: black;
            color: yellow;
        }

        /* Scrollbars (Roblox-style) */
        ::-webkit-scrollbar {
            width: 8px;
        }

        ::-webkit-scrollbar-thumb {
            background-color: yellow;
            border-radius: 10px;
        }

        ::-webkit-scrollbar-track {
            background: black;
        }

        /* Footer */
        footer {
            background-color: lightblue;
            padding: 20px;
            text-align: center;
            color: black;
            font-size: 1rem;
        }
    </style>
</head>
<body>
    <header>
        <img src="https://github.com/user-attachments/assets/358c0fca-d564-48c2-940d-2a970e4cc440" alt="Vortex Drift Logo">
    </header>

    <div class="container">
        <div class="title">Welcome to Vortex Drift</div>
        <div class="games-list">
            <div class="game-item">Game 1</div>
            <div class="game-item">Game 2</div>
            <div class="game-item">Game 3</div>
        </div>
        <button>Start Game</button>
    </div>

    <footer>
        &copy; 2025 Vortex Drift. All Rights Reserved.
    </footer>
</body>
</html>
