<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Легендарная пьянка — Фиолетовый Неон</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap');
  body {
    margin: 0;
    height: 100vh;
    background: linear-gradient(135deg, #8e2de2, #4a00e0);
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    font-family: 'Montserrat', sans-serif;
    color: #f0c3ff;
    text-shadow:
      0 0 10px #e754ff,
      0 0 20px #d500f9,
      0 0 30px #a400d8;
    animation: pulse 3s infinite alternate;
  }
  @keyframes pulse {
    0% {
      text-shadow:
        0 0 10px #e754ff,
        0 0 20px #d500f9,
        0 0 30px #a400d8;
    }
    100% {
      text-shadow:
        0 0 20px #f8aaff,
        0 0 40px #ea00ff,
        0 0 60px #c200ff;
    }
  }
  h1 {
    font-size: 3.8rem;
    margin: 0.2em 0;
  }
  h2 {
    font-size: 2.8rem;
    margin: 0.2em 0 1em;
  }
  .date-time, .location, .footer {
    font-size: 1.6rem;
    margin: 0.4em 0;
    text-shadow:
      0 0 12px #f5aaff,
      0 0 24px #c400ff;
  }
  button {
    margin-top: 2.5em;
    background: #c700ff;
    border: none;
    color: #fff;
    font-weight: 700;
    font-size: 1.3rem;
    padding: 0.7em 1.5em;
    border-radius: 12px;
    cursor: pointer;
    box-shadow:
      0 0 15px #c700ff,
      0 0 30px #c700ff;
    transition: background 0.3s ease;
  }
  button:hover {
    background: #ea00ff;
  }
  iframe {
    margin-top: 2em;
    border: none;
    border-radius: 12px;
    box-shadow:
      0 0 20px #c700ff;
  }
</style>
</head>
<body>
  <h1>Впервые за два года</h1>
  <h2>Легендарная пьянка</h2>
  <div class="date-time">🍾 16 августа • 17:00</div>
  <div class="location">📍 Микрорайон Нанжуль, 47</div>
  <div class="footer">Жду вас!</div>
  <button id="playMusic">Включить музыку</button>
  <iframe id="ytPlayer" width="320" height="180" src="" allow="autoplay; encrypted-media" allowfullscreen></iframe>
<script>
  const button = document.getElementById('playMusic');
  const player = document.getElementById('ytPlayer');
  button.addEventListener('click', () => {
    player.src = "https://www.youtube.com/embed/5NV6Rdv1a3I?autoplay=1&loop=1&playlist=5NV6Rdv1a3I";
    button.style.display = 'none';
  });
</script>
</body>
</html># party-invite