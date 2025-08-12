<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Under Construction - But Still Fun!</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Bangers&family=Inter:wght@400;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #1a1a1a;
            color: #f0f0f0;
            overflow-x: hidden;
        }
        h1, h2, h3 {
            font-family: 'Bangers', cursive;
            letter-spacing: 2px;
        }
        .construction-tape {
            background-image: repeating-linear-gradient(
                45deg,
                #ffcc00,
                #ffcc00 25px,
                #1a1a1a 25px,
                #1a1a1a 50px
            );
            padding: 1rem;
            transform: rotate(-2deg);
            box-shadow: 0 4px 15px rgba(0,0,0,0.5);
        }
        .game-card {
            background-color: #2a2a2a;
            border: 2px dashed #ffcc00;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        .game-card:hover {
            transform: translateY(-10px) rotate(1deg);
            box-shadow: 0 10px 20px rgba(255, 204, 0, 0.2);
        }
        #whack-a-bug-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 10px;
            width: 100%;
            max-width: 320px;
            height: 320px;
            margin: auto;
            background-color: #3a3a3a;
            border-radius: 12px;
            padding: 10px;
        }
        .bug-hole {
            background-color: #1a1a1a;
            border-radius: 50%;
            position: relative;
            overflow: hidden;
        }
        .bug {
            font-size: 40px;
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, 100%);
            cursor: pointer;
            user-select: none;
            transition: transform 0.2s ease;
        }
        .bug.up {
            transform: translate(-50%, -50%);
        }
        #dino-game-canvas {
            background-color: #3a3a3a;
            border-radius: 12px;
            width: 100%;
            height: 200px;
        }
        .btn-start {
            background-color: #ffcc00;
            color: #1a1a1a;
            font-family: 'Bangers', cursive;
            letter-spacing: 1px;
        }
    </style>
</head>
<body class="bg-gray-900 text-white p-4 sm:p-8">

    <div class="container mx-auto text-center max-w-4xl">

        <!-- Header Section -->
        <div class="construction-tape mb-12">
            <h1 class="text-5xl md:text-7xl text-white">WHOOPS!</h1>
        </div>

        <h2 class="text-4xl md:text-5xl text-yellow-400 mb-2 animate-pulse">Our Website is Under Construction</h2>
        <p class="text-lg text-gray-400 mb-4">A digital playground by Anirudh.</p>
        <p class="text-lg md:text-xl mb-8 max-w-2xl mx-auto">
            Our digital hamsters are working tirelessly on their tiny wheels to power up the new site. It's going to be epic, we promise! In the meantime, please don't feed the developers after midnight.
        </p>
        <p class="text-lg md:text-xl mb-12 max-w-2xl mx-auto">
            To make the wait less boring, we've whipped up a couple of highly unproductive (but fun) games for you.
        </p>

        <!-- Games Section -->
        <div class="grid grid-cols-1 md:grid-cols-2 gap-8">

            <!-- Whack-a-Bug Game -->
            <div class="game-card rounded-lg p-6">
                <h3 class="text-3xl text-yellow-400 mb-4">Whack-a-Bug!</h3>
                <p class="mb-4">These pesky bugs keep showing up in our code. Help us squash them! Click the bugs to score.</p>
                <div class="text-2xl mb-4">Score: <span id="whack-a-bug-score" class="font-bold">0</span></div>
                <div id="whack-a-bug-grid"></div>
                <button id="start-whack-a-bug" class="btn-start px-6 py-2 rounded-lg mt-4 text-xl">Start Game</button>
            </div>

            <!-- Dino Run Game -->
            <div class="game-card rounded-lg p-6">
                <h3 class="text-3xl text-yellow-400 mb-4">Dino Run</h3>
                <p class="mb-4">Our server is powered by a dinosaur. Help it jump over obstacles! Press Space or Tap to Jump.</p>
                <div class="text-2xl mb-4">Score: <span id="dino-score" class="font-bold">0</span></div>
                <canvas id="dino-game-canvas"></canvas>
                 <div id="dino-game-message" class="mt-4 text-lg h-6"></div>
            </div>

        </div>

        <!-- Footer -->
        <div class="mt-16 text-gray-500">
            <p>We'll be back soon. Probably.</p>
            <p>Follow our non-existent social media for updates that won't happen:</p>
            <div class="flex justify-center space-x-4 mt-4">
                <a href="#" class="hover:text-yellow-400">#NotOnTwitter</a>
                <a href="#" class="hover:text-yellow-400">#Fakebook</a>
                <a href="#" class="hover:text-yellow-400">#Insta-scam</a>
            </div>
            <p class="mt-8">P.S. Sarayu is sleeping. 🤫</p>
        </div>

    </div>

    <script>
        // --- Whack-a-Bug Game ---
        const whackABugGrid = document.getElementById('whack-a-bug-grid');
        const whackABugScoreEl = document.getElementById('whack-a-bug-score');
        const startWhackABugBtn = document.getElementById('start-whack-a-bug');
        
        let whackABugScore = 0;
        let bugHoles = [];
        let gameInterval;
        let isGameRunning = false;

        function setupWhackABug() {
            for (let i = 0; i < 16; i++) {
                const hole = document.createElement('div');
                hole.classList.add('bug-hole');
                const bug = document.createElement('div');
                bug.classList.add('bug');
                bug.textContent = '🐛';
                bug.addEventListener('click', whackBug);
                hole.appendChild(bug);
                whackABugGrid.appendChild(hole);
                bugHoles.push(bug);
            }
        }

        function whackBug(e) {
            if (!e.target.classList.contains('up')) return;
            whackABugScore++;
            whackABugScoreEl.textContent = whackABugScore;
            e.target.classList.remove('up');
        }

        function popUpBug() {
            bugHoles.forEach(bug => bug.classList.remove('up'));
            const randomBug = bugHoles[Math.floor(Math.random() * bugHoles.length)];
            randomBug.classList.add('up');
        }

        startWhackABugBtn.addEventListener('click', () => {
            if (isGameRunning) return;
            isGameRunning = true;
            whackABugScore = 0;
            whackABugScoreEl.textContent = 0;
            startWhackABugBtn.textContent = 'Game in Progress...';
            startWhackABugBtn.disabled = true;

            gameInterval = setInterval(popUpBug, 800);

            setTimeout(() => {
                clearInterval(gameInterval);
                isGameRunning = false;
                startWhackABugBtn.textContent = 'Play Again';
                startWhackABugBtn.disabled = false;
                alert(`Game Over! Your final score is ${whackABugScore}`);
                 bugHoles.forEach(bug => bug.classList.remove('up'));
            }, 20000); // Game lasts 20 seconds
        });
        
        setupWhackABug();


        // --- Dino Run Game ---
        const canvas = document.getElementById('dino-game-canvas');
        const ctx = canvas.getContext('2d');
        const dinoScoreEl = document.getElementById('dino-score');
        const dinoGameMessageEl = document.getElementById('dino-game-message');

        let dinoScore = 0;
        let dinoGameSpeed = 3;
        let dinoGameFrame = 0;
        let dinoGameRunning = false;

        const dino = {
            x: 50,
            y: canvas.height - 40,
            width: 20,
            height: 40,
            dy: 0,
            jumpPower: 10,
            gravity: 0.4,
            grounded: true
        };

        let obstacles = [];

        function drawDino() {
            ctx.fillStyle = '#f0f0f0';
            // Simple dino shape
            ctx.fillRect(dino.x, dino.y, dino.width, dino.height);
            // Eye
            ctx.fillStyle = '#1a1a1a';
            ctx.fillRect(dino.x + 12, dino.y + 5, 4, 4);
        }

        function drawObstacles() {
            obstacles.forEach(obstacle => {
                ctx.fillStyle = '#ff6b6b';
                ctx.fillRect(obstacle.x, obstacle.y, obstacle.width, obstacle.height);
            });
        }

        function updateDino() {
            dino.y += dino.dy;
            if (dino.y + dino.height < canvas.height) {
                dino.dy += dino.gravity;
                dino.grounded = false;
            } else {
                dino.dy = 0;
                dino.y = canvas.height - dino.height;
                dino.grounded = true;
            }
        }
        
        function updateObstacles() {
            dinoGameFrame++;
            if (dinoGameFrame % Math.floor(150 / (dinoGameSpeed / 3)) === 0) {
                const height = Math.random() * 30 + 20;
                obstacles.push({
                    x: canvas.width,
                    y: canvas.height - height,
                    width: 20,
                    height: height
                });
            }

            obstacles.forEach(obstacle => {
                obstacle.x -= dinoGameSpeed;
            });

            obstacles = obstacles.filter(obstacle => obstacle.x + obstacle.width > 0);
        }

        function checkCollision() {
            obstacles.forEach(obstacle => {
                if (
                    dino.x < obstacle.x + obstacle.width &&
                    dino.x + dino.width > obstacle.x &&
                    dino.y < obstacle.y + obstacle.height &&
                    dino.y + dino.height > obstacle.y
                ) {
                    endDinoGame();
                }
            });
        }

        function updateScore() {
            if(dinoGameRunning) {
                dinoScore++;
                dinoScoreEl.textContent = Math.floor(dinoScore / 10);
                if (dinoScore % 500 === 0) {
                    dinoGameSpeed += 0.5;
                }
            }
        }
        
        function clearCanvas() {
            ctx.clearRect(0, 0, canvas.width, canvas.height);
        }

        function gameLoop() {
            if (!dinoGameRunning) return;
            clearCanvas();
            updateDino();
            updateObstacles();
            drawDino();
            drawObstacles();
            checkCollision();
            updateScore();
            requestAnimationFrame(gameLoop);
        }
        
        function startDinoGame() {
            if (dinoGameRunning) return;
            dinoGameRunning = true;
            dinoScore = 0;
            dinoGameSpeed = 3;
            obstacles = [];
            dino.y = canvas.height - dino.height;
            dino.dy = 0;
            dinoGameMessageEl.textContent = '';
            gameLoop();
        }

        function endDinoGame() {
            dinoGameRunning = false;
            dinoGameMessageEl.textContent = 'Game Over! Press Space to Restart.';
        }

        function dinoJump() {
            if (dino.grounded) {
                dino.dy = -dino.jumpPower;
            }
        }
        
        function handleInput(e) {
            if (e.code === 'Space' || e.type === 'touchstart') {
                e.preventDefault();
                if (dinoGameRunning) {
                    dinoJump();
                } else {
                    startDinoGame();
                }
            }
        }

        document.addEventListener('keydown', handleInput);
        canvas.addEventListener('click', () => {
            if (dinoGameRunning) {
                dinoJump();
            } else {
                startDinoGame();
            }
        });
        canvas.addEventListener('touchstart', handleInput);

        // Initial message
        function drawInitialMessage() {
            ctx.fillStyle = '#f0f0f0';
            ctx.font = "16px 'Inter'";
            ctx.textAlign = 'center';
            ctx.fillText('Click or Press Space to Start', canvas.width / 2, canvas.height / 2);
        }
        
        window.onload = () => {
            // Set canvas dimensions based on container
            const canvasContainer = canvas.parentElement;
            canvas.width = canvasContainer.offsetWidth;
            drawInitialMessage();
        };
        
         window.onresize = () => {
            const canvasContainer = canvas.parentElement;
            canvas.width = canvasContainer.offsetWidth;
            if (!dinoGameRunning) {
                clearCanvas();
                drawInitialMessage();
            }
        };


    </script>
</body>
</html>
