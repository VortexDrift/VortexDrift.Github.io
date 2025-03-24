# Vortex Drift - PC Games

VortexDrift is a space dedicated to showcasing a variety of 3D games. Hosted on GitHub, it features unique and immersive experiences that are designed to engage and challenge players, offering creative gameplay mechanics and new worlds to explore.

![Screenshot 2025-03-24 2 21 57 PM](https://github.com/user-attachments/assets/d80f1123-6025-43b5-803c-b07f45fe31af)

---

## Website Code:

Here is the complete HTML, CSS, and JavaScript code for the Vortex Drift website. Feel free to copy and paste the code into your own projects or modify it as needed.

```html
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

        #footer-content {
            display: none; /* Hidden by default */
            color: white;
            margin-top: 20px;
            padding: 20px;
            background-color: black;
            border-radius: 10px;
        }
    </style>
</head>
<body>
    <header>
        <img src="https://github.com/user-attachments/assets/d80f1123-6025-43b5-803c-b07f45fe31af" alt="Screenshot 2025-03-24 2 21 57 PM">
    </header>

    <div class="container">
        <div class="title">Welcome to Vortex Drift</div>
        <div class="games-list">
            <div class="game-item">Game 1</div>
            <div class="game-item">Game 2</div>
            <div class="game-item">Game 3</div>
        </div>
        <button>Start Game</button>

        <!-- Link to Load Content -->
        <a href="#" id="load-content-link" onclick="loadContent()">Click here to view footer content</a>
        <div id="footer-content"></div>
    </div>

    <footer>
        &copy; 2025 Vortex Drift. All Rights Reserved. <br>
        All content on this website, including text, images, graphics, and design, is protected by copyright laws and may not be reproduced, distributed, or used without my permission. Vortex Drift and its logo are trademarks of VortexDrift.
    </footer>

    <script>
        // Function to dynamically load content from the GitHub link
        function loadContent() {
            // Fetching content from the raw GitHub file
            fetch('https://raw.githubusercontent.com/VortexDrift/VortexDrift.Github.io/refs/heads/main/Website')
                .then(response => response.text())
                .then(data => {
                    // Inserting the content into the footer-content div
                    document.getElementById('footer-content').innerHTML = data;
                    document.getElementById('footer-content').style.display = 'block'; // Make content visible
                })
                .catch(error => console.error('Error loading the content:', error));
        }
    </script>
</body>
</html>
