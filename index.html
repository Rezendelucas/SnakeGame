<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <title>Jogo da Cobrinha</title>
  <style>
    body {
      background: #222;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
      font-family: sans-serif;
      color: #fff;
    }
    canvas {
      border: 2px solid #555;
      background: #000;
    }
    #score {
      position: absolute;
      top: 10px;
      left: 10px;
      font-size: 20px;
      color: white;
    }
  </style>
</head>
<body>
  <div id="score">Pontos: 0</div>
  <canvas id="game" width="400" height="400"></canvas>

  <script>
    const canvas = document.getElementById("game");
    const ctx = canvas.getContext("2d");

    const gridSize = 20; // Tamanho dos blocos
    const tileCount = canvas.width / gridSize;

    let snake = [{ x: 10, y: 10 }];
    let direction = { x: 0, y: 0 };
    let food = { x: 15, y: 15 };
    let score = 0;
    let speed = 200; // Em milissegundos

    function drawBlock(x, y, color) {
      ctx.fillStyle = color;
      ctx.fillRect(x * gridSize, y * gridSize, gridSize - 2, gridSize - 2);
    }

    function drawGame() {
      ctx.clearRect(0, 0, canvas.width, canvas.height);

      // Desenha a comida
      drawBlock(food.x, food.y, "red");

      // Desenha a cobrinha
      snake.forEach(segment => drawBlock(segment.x, segment.y, "green"));

      // Atualiza a posição da cobra
      const head = { x: snake[0].x + direction.x, y: snake[0].y + direction.y };

      // Fim de jogo se bater na parede ou em si mesma
      if (
        head.x < 0 || head.x >= tileCount ||
        head.y < 0 || head.y >= tileCount ||
        snake.some(segment => segment.x === head.x && segment.y === head.y)
      ) {
        alert("Fim de jogo! Pontuação: " + score);
        resetGame();
        return;
      }

      snake.unshift(head);

      // Se comer a comida
      if (head.x === food.x && head.y === food.y) {
        score++;
        document.getElementById("score").textContent = "Pontos: " + score;

        // Aumenta a velocidade (diminui o intervalo)
        if (speed > 50) speed -= 10;

        // Coloca comida em novo lugar
        placeFood();
      } else {
        snake.pop(); // Remove a cauda se não comeu
      }

      // Chama o jogo novamente com a nova velocidade
      setTimeout(drawGame, speed);
    }

    function placeFood() {
      let newFood;
      do {
        newFood = {
          x: Math.floor(Math.random() * tileCount),
          y: Math.floor(Math.random() * tileCount)
        };
      } while (snake.some(segment => segment.x === newFood.x && segment.y === newFood.y));
      food = newFood;
    }

    function resetGame() {
      snake = [{ x: 10, y: 10 }];
      direction = { x: 0, y: 0 };
      food = { x: 15, y: 15 };
      score = 0;
      speed = 200;
      document.getElementById("score").textContent = "Pontos: 0";
      drawGame();
    }

    // Controle com as setas
    document.addEventListener("keydown", e => {
      switch (e.key) {
        case "ArrowUp":
          if (direction.y === 0) direction = { x: 0, y: -1 };
          break;
        case "ArrowDown":
          if (direction.y === 0) direction = { x: 0, y: 1 };
          break;
        case "ArrowLeft":
          if (direction.x === 0) direction = { x: -1, y: 0 };
          break;
        case "ArrowRight":
          if (direction.x === 0) direction = { x: 1, y: 0 };
          break;
      }
    });

    drawGame(); // Inicia o jogo
  </script>
</body>
</html>
