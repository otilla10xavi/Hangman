<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Judaism Hangman</title>
    <style>
        body { font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; display: flex; flex-direction: column; align-items: center; background-color: #f4f7f6; color: #333; }
        h1 { color: #2c3e50; margin-top: 20px; }
        #game-container { background: white; padding: 20px; border-radius: 12px; box-shadow: 0 4px 15px rgba(0,0,0,0.1); text-align: center; max-width: 500px; width: 90%; }
        #canvas-container { margin: 20px 0; }
        #word-display { font-size: 2em; letter-spacing: 10px; margin: 20px 0; font-weight: bold; color: #2980b9; }
        #keyboard { display: grid; grid-template-columns: repeat(auto-fit, minmax(35px, 1fr)); gap: 5px; margin-top: 20px; }
        button { padding: 10px; border: 1px solid #ddd; background: #fff; cursor: pointer; border-radius: 4px; font-weight: bold; transition: 0.2s; }
        button:hover:not(:disabled) { background: #3498db; color: white; border-color: #3498db; }
        button:disabled { opacity: 0.4; cursor: not-allowed; }
        #message { margin-top: 20px; font-weight: bold; min-height: 1.2em; }
        .reset-btn { margin-top: 20px; padding: 10px 20px; background: #27ae60; color: white; border: none; border-radius: 5px; cursor: pointer; display: none; }
    </style>
</head>
<body>

    <h1>Jewish Heritage Hangman</h1>

    <div id="game-container">
        <div id="canvas-container">
            <canvas id="hangmanCanvas" width="200" height="200"></canvas>
        </div>

        <div id="word-display">_ _ _ _ _</div>
        <div id="message"></div>
        <div id="keyboard"></div>
        
        <button class="reset-btn" id="reset-btn" onclick="initGame()">Play Again</button>
    </div>

    <script>
        const words = ["MENORAH", "SHABBAT", "DREIDEL", "MITZVAH", "KOSHER", "HANUKKAH", "PASSOVER", "TORAH", "SYNAGOGUE", "MEZUZAH"];
        let selectedWord = "";
        let guessedLetters = [];
        let mistakes = 0;
        const maxMistakes = 6;

        const canvas = document.getElementById('hangmanCanvas');
        const ctx = canvas.getContext('2d');

        function initGame() {
            selectedWord = words[Math.floor(Math.random() * words.length)];
            guessedLetters = [];
            mistakes = 0;
            
            document.getElementById('message').innerText = "";
            document.getElementById('reset-btn').style.display = "none";
            drawHangman();
            updateDisplay();
            createKeyboard();
        }

        function createKeyboard() {
            const keyboard = document.getElementById('keyboard');
            keyboard.innerHTML = "";
            "ABCDEFGHIJKLMNOPQRSTUVWXYZ".split("").forEach(letter => {
                const btn = document.createElement('button');
                btn.innerText = letter;
                btn.onclick = () => handleGuess(letter);
                keyboard.appendChild(btn);
            });
        }

        function handleGuess(letter) {
            guessedLetters.push(letter);
            const buttons = document.querySelectorAll('#keyboard button');
            buttons.forEach(btn => {
                if (btn.innerText === letter) btn.disabled = true;
            });

            if (!selectedWord.includes(letter)) {
                mistakes++;
                drawHangman();
            }

            updateDisplay();
            checkGameStatus();
        }

        function updateDisplay() {
            const display = selectedWord.split("").map(letter => 
                guessedLetters.includes(letter) ? letter : "_"
            ).join(" ");
            document.getElementById('word-display').innerText = display;
        }

        function checkGameStatus() {
            if (!document.getElementById('word-display').innerText.includes("_")) {
                document.getElementById('message').innerText = "Mazel Tov! You won!";
                document.getElementById('message').style.color = "#27ae60";
                endGame();
            } else if (mistakes >= maxMistakes) {
                document.getElementById('message').innerText = `Game Over. The word was: ${selectedWord}`;
                document.getElementById('message').style.color = "#c0392b";
                endGame();
            }
        }

        function endGame() {
            const buttons = document.querySelectorAll('#keyboard button');
            buttons.forEach(btn => btn.disabled = true);
            document.getElementById('reset-btn').style.display = "inline-block";
        }

        function drawHangman() {
            ctx.clearRect(0, 0, canvas.width, canvas.height);
            ctx.strokeStyle = "#2c3e50";
            ctx.lineWidth = 3;

            // Base gallows
            ctx.beginPath();
            ctx.moveTo(20, 180); ctx.lineTo(180, 180);
            ctx.moveTo(50, 180); ctx.lineTo(50, 20);
            ctx.lineTo(130, 20); ctx.lineTo(130, 40);
            ctx.stroke();

            if (mistakes > 0) { // Head
                ctx.beginPath(); ctx.arc(130, 55, 15, 0, Math.PI * 2); ctx.stroke();
            }
            if (mistakes > 1) { // Body
                ctx.beginPath(); ctx.moveTo(130, 70); ctx.lineTo(130, 120); ctx.stroke();
            }
            if (mistakes > 2) { // Left Arm
                ctx.beginPath(); ctx.moveTo(130, 85); ctx.lineTo(100, 100); ctx.stroke();
            }
            if (mistakes > 3) { // Right Arm
                ctx.beginPath(); ctx.moveTo(130, 85); ctx.lineTo(160, 100); ctx.stroke();
            }
            if (mistakes > 4) { // Left Leg
                ctx.beginPath(); ctx.moveTo(130, 120); ctx.lineTo(110, 150); ctx.stroke();
            }
            if (mistakes > 5) { // Right Leg
                ctx.beginPath(); ctx.moveTo(130, 120); ctx.lineTo(150, 150); ctx.stroke();
            }
        }

        initGame();
    </script>
</body>
</html>
