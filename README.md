<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Mallikarjun D V S - Animated Portfolio</title>
  <style>
    body {
      margin: 0;
      font-family: 'Arial', sans-serif;
      background: linear-gradient(135deg, #2980b9, #2c3e50);
      height: 100vh;
      overflow: hidden;
      color: #fff;
      position: relative;
      display: flex;
      align-items: center;
      justify-content: center;
    }
    .background-anim {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: url('https://media.giphy.com/media/l0HlRnAWXxn0MhKLK/giphy.gif') no-repeat center center;
      background-size: cover;
      opacity: 0.1;
      z-index: -1;
    }
    .container {
      text-align: center;
      animation: fadeIn 2s ease-in;
      z-index: 1;
    }
    h1 {
      font-size: 3em;
      margin: 0;
      color: #fff;
      text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.3);
    }
    h2 {
      font-size: 1.2em;
      color: #ecf0f1;
      margin: 10px 0 30px;
      font-weight: normal;
    }
    .buttons {
      display: flex;
      justify-content: center;
      gap: 10px;
      flex-wrap: wrap;
      max-width: 800px;
      margin: 0 auto;
    }
    .button {
      padding: 8px 20px;
      background: rgba(255, 255, 255, 0.15);
      border-radius: 30px;
      color: #fff;
      text-decoration: none;
      font-size: 1em;
      transition: background 0.3s, transform 0.3s;
      box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    }
    .button:hover {
      background: rgba(255, 255, 255, 0.25);
      transform: translateY(-2px);
    }
    .floating {
      position: absolute;
      background: rgba(52, 152, 219, 0.5);
      border-radius: 4px;
      animation: float 5s ease-in-out infinite, rotate 10s linear infinite;
      pointer-events: none;
    }
    .floating:nth-child(1) { top: 20%; left: 10%; width: 20px; height: 20px; animation-delay: 0s; }
    .floating:nth-child(2) { top: 40%; right: 15%; width: 30px; height: 30px; animation-delay: 1s; transform: rotate(45deg); }
    .floating:nth-child(3) { bottom: 30%; left: 25%; width: 25px; height: 25px; animation-delay: 2s; }
    .floating:nth-child(4) { top: 10%; right: 30%; width: 15px; height: 15px; animation-delay: 3s; transform: rotate(-45deg); }
    .floating:nth-child(5) { bottom: 20%; right: 10%; width: 35px; height: 35px; animation-delay: 0.5s; }
    @keyframes float {
      0%, 100% { transform: translateY(0) rotate(0deg); }
      50% { transform: translateY(-30px) rotate(180deg); }
    }
    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }
    @keyframes rotate {
      from { transform: rotate(0deg); }
      to { transform: rotate(360deg); }
    }
  </style>
</head>
<body>
  <div class="background-anim"></div>
  <div class="container">
    <h1>Mallikarjun D V S</h1>
    <h2>Final-Year B.Tech CSE (Data Science) | Full-Stack Developer</h2>
    <div class="buttons">
      <a href="#" class="button">Python</a>
      <a href="#" class="button">JavaScript</a>
      <a href="#" class="button">React.js</a>
      <a href="#" class="button">Node.js</a>
      <a href="#" class="button">MongoDB</a>
    </div>
    <div class="buttons" style="margin-top: 20px;">
      <a href="https://github.com/Mallikarjun-04/Hackathon-Portal" class="button">Hackathon Portal</a>
      <a href="https://github.com/Mallikarjun-04/daily-DSA" class="button">Daily DSA</a>
      <a href="mailto:mallikarjundvs04@gmail.com" class="button">Email</a>
      <a href="https://www.linkedin.com/in/d-v-s-mallikarjun-aa775832a" class="button">LinkedIn</a>
    </div>
  </div>
  <div class="floating"></div>
  <div class="floating"></div>
  <div class="floating"></div>
  <div class="floating"></div>
  <div class="floating"></div>
</body>
</html>
