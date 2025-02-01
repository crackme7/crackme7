<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>C y Y ❤️</title>
  <style>
    /* Fondo romántico */
    body {
      background: linear-gradient(to bottom right, #ff9a9e, #fad0c4);
      font-family: 'Arial', sans-serif;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
      overflow: hidden;
      color: #fff;
    }

    /* I love you baby*/
    .card {
      background: rgba(255, 255, 255, 0.2);
      padding: 20px;
      border-radius: 20px;
      text-align: center;
      max-width: 400px;
      box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
    }

    h1 {
      font-size: 3rem;
    }

    p {
      font-size: 1.2rem;
    }

    .hearts {
      position: fixed;
      width: 100%;
      height: 100%;
      pointer-events: none;
    }

    .heart {
      position: absolute;
      width: 20px;
      height: 20px;
      background: red;
      clip-path: polygon(50% 0%, 0% 50%, 50% 100%, 100% 50%);
      animation: float 4s infinite ease-in-out;
      opacity: 0.8;
    }

    @keyframes float {
      0% {
        transform: translateY(0);
        opacity: 0;
      }
      50% {
        opacity: 1;
      }
      100% {
        transform: translateY(-800px) rotate(360deg);
        opacity: 0;
      }
    }
  </style>
</head>
<body>
  <div class="card">
    <h1>¡Felices 63 dias de novios! ❤️</h1>
    <p>Eres mi persona favorita en este mundo 🌍</p>
  </div>

  <!-- Ramo de rosas -->
  <div class="hearts"></div>

  <script>
    function createHeart() {
      const heart = document.createElement("div");
      heart.classList.add("heart");
      heart.style.left = Math.random() * 100 + "vw";
      heart.style.animationDuration = Math.random() * 2 + 3 + "s";
      document.querySelector(".hearts").appendChild(heart);

      setTimeout(() => heart.remove(), 5000);
    }

    setInterval(createHeart, 300);
  </script>
</body>
</html>

