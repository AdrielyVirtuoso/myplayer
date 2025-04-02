<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Player 2 ❤️</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Press+Start+2P&display=swap');

   body {
      background: url('https://i.imgur.com/yZ8ZFt4.png') center center / cover no-repeat fixed;
      color: #fff;
      font-family: 'Press Start 2P', cursive;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
      padding: 20px;
      height: 100vh;
      margin: 0;
    }

   video {
      width: 80%;
      max-width: 720px;
      border: 4px solid #ff69b4;
      border-radius: 12px;
      box-shadow: 0 0 25px #ff69b4;
      margin-bottom: 25px;
    }

   h1 {
      font-size: 1rem;
      color: #00ffff;
      margin-bottom: 10px;
    }

  #timer {
      font-size: 0.8rem;
      color: #ffff66;
      margin-bottom: 20px;
    }
   .texto-amor {
      font-size: 0.8rem;
      max-width: 650px;
      background: rgba(0, 0, 0, 0.6);
      padding: 20px;
      border: 2px dashed #00ffff;
      border-radius: 10px;
      color: #ffffff;
    }
  </style>
</head>
<body>
  <video controls autoplay loop>
    <source src="video.mp4" type="video/mp4">
    Seu navegador não suporta vídeo HTML5.
  </video>

  <h1>Estamos juntos há:</h1>
  <div id="timer"></div>

  <div class="texto-amor">
    <p>Meu amor, meu namorado, meu player 2, minha paixão em 2D. Quero viver o resto da vida com você.</p>
  </div>

  <script>
    const startDate = new Date("2025-02-03T00:00:00");

    function updateTimer() {
      const now = new Date();
      const diff = now - startDate;

      const days = Math.floor(diff / (1000 * 60 * 60 * 24));
      const hours = Math.floor((diff / (1000 * 60 * 60)) % 24);
      const minutes = Math.floor((diff / (1000 * 60)) % 60);
      const seconds = Math.floor((diff / 1000) % 60);

      document.getElementById("timer").innerText = 
        `${days} dias, ${hours} horas, ${minutes} minutos e ${seconds} segundos ❤️`;
    }

    setInterval(updateTimer, 1000);
    updateTimer();
  </script>
</body>
</html>
