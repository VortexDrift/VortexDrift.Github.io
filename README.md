<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>VortexDrift - Games</title>
    <style>
        body {
            background: black;
            color: white;
            font-family: Arial, sans-serif;
            text-align: center;
        }
        .container {
            width: 80%;
            margin: auto;
        }
        .game-list {
            display: flex;
            overflow-x: auto;
            white-space: nowrap;
            padding: 20px;
        }
        .game {
            background: yellow;
            color: black;
            padding: 20px;
            margin: 10px;
            border-radius: 10px;
            display: inline-block;
            min-width: 200px;
        }
        button {
            background: lightblue;
            border: none;
            padding: 10px;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <h1>VortexDrift Games</h1>
    <div class="container">
        <div class="game-list" id="gameList">
            <!-- Games will be added here dynamically -->
        </div>
    </div>
    <script>
        const games = [
            { name: "Game 1", link: "#" },
            { name: "Game 2", link: "#" },
            { name: "Game 3", link: "#" }
        ];
        const gameList = document.getElementById("gameList");
        games.forEach(game => {
            const gameDiv = document.createElement("div");
            gameDiv.classList.add("game");
            gameDiv.innerHTML = `<h3>${game.name}</h3><button onclick="location.href='${game.link}'">Play</button>`;
            gameList.appendChild(gameDiv);
        });
    </script>
</body>
</html>

