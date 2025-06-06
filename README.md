<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Happy Monthsarry!</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      height: 100vh;
      background: linear-gradient(135deg, #ff9a9e, #fad0c4);
      display: flex;
      justify-content: center;
      align-items: center;
      overflow: hidden;
      font-family: 'Segoe UI', sans-serif;
    }

    h1 {
      font-size: 2.5rem;
      color: white;
      text-align: center;
      z-index: 2;
      position: relative;
      text-shadow: 2px 2px 4px rgba(0,0,0,0.2);
    }

    .heart {
      position: absolute;
      color: red;
      font-size: 1.5rem;
      animation: float 10s infinite ease-in-out;
      opacity: 0.8;
    }

    @keyframes float {
      0% {
        transform: translateY(100vh) scale(1);
        opacity: 0;
      }
      50% {
        opacity: 1;
      }
      100% {
        transform: translateY(-10vh) scale(1.2);
        opacity: 0;
      }
    }
  </style>
</head>
<body>
  <h1>Happy 7th Monthsarry, Langga ❤️</h1>

  <!-- Floating hearts -->
  <script>
    const colors = ["❤️", "💖", "💕", "💘", "💝"];
    for (let i = 0; i < 30; i++) {
      const heart = document.createElement("div");
      heart.classList.add("heart");
      heart.style.left = Math.random() * 100 + "vw";
      heart.style.animationDuration = 5 + Math.random() * 5 + "s";
      heart.textContent = colors[Math.floor(Math.random() * colors.length)];
      document.body.appendChild(heart);
    }
  </script>
</body>
</html>
