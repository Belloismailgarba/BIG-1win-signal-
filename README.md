<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>BIG 1WIN SIGNALS</title>
  <style>
    body {
      background-image: url('https://oaidalleapiprodscus.blob.core.windows.net/private/org-qqpG1U3QkiQ1oKf3JcOZbFq9/user-8a5hRtqPGp6U0xwYhL1aTe8C/img-0d1c7e4c7b3dc3c8b794c6e9d5e3f4f8.png');
      background-size: cover;
      background-position: center;
      background-repeat: no-repeat;
      color: white;
      font-family: Arial, sans-serif;
      text-align: center;
      padding: 20px;
      min-height: 100vh;
      /* Add a dark overlay for readability */
      position: relative;
    }
    body::before {
      content: "";
      position: fixed;
      top: 0; left: 0; width: 100vw; height: 100vh;
      background: rgba(30,30,30,0.75);
      z-index: 0;
      pointer-events: none;
    }
    #content {
      position: relative;
      z-index: 1;
    }
    h1 {
      color: #fdd835;
      font-size: 2.5em;
      margin-top: 20px;
      text-shadow: 2px 2px 8px #000;
    }
    .grid {
      display: grid;
      grid-template-columns: repeat(5, 60px);
      gap: 5px;
      justify-content: center;
      margin-top: 30px;
    }
    .block {
      width: 60px;
      height: 60px;
      background-color: #2196f3;
      font-size: 40px;
      line-height: 60px;
      display: flex;
      align-items: center;
      justify-content: center;
      border-radius: 8px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.15);
      transition: background 0.2s;
    }
    .star {
      background-color: transparent;
      box-shadow: none;
    }
    .rotated {
      transform: rotate(180deg);
    }
    button {
      margin-top: 30px;
      padding: 12px 25px;
      font-size: 18px;
      background-color: #fdd835;
      color: #1e1e1e;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      transition: background-color 0.3s ease;
      font-weight: bold;
      box-shadow: 0 2px 8px rgba(0,0,0,0.12);
    }
    button:hover {
      background-color: #ffeb3b;
    }
    @media (max-width: 400px) {
      .grid { grid-template-columns: repeat(5, 38px); }
      .block { width: 38px; height: 38px; font-size: 24px; }
    }
  </style>
</head>
<body>
  <div id="content">
    <h1>BIG 1WIN SIGNALS</h1>
    <div id="grid" class="grid"></div>
    <button onclick="nextSignal()">Next SIGNAL 🔔</button>
    <!-- Sound effect -->
    <audio id="ding" src="https://cdn.pixabay.com/audio/2021/08/04/audio_2b47a0bfc9.mp3" preload="auto"></audio>
  </div>
  <script>
    const gridElement = document.getElementById("grid");
    const ding = document.getElementById("ding");
    let rotated = false;

    function createSignal(rotatedStars = false) {
      gridElement.innerHTML = "";
      const starPositions = [6, 11, 20, 22];
      for (let i = 0; i < 25; i++) {
        const div = document.createElement("div");
        div.className = "block";
        if (starPositions.includes(i)) {
          div.classList.add("star");
          div.textContent = "⭐";
          if (rotatedStars) div.classList.add("rotated");
        }
        gridElement.appendChild(div);
      }
    }

    function nextSignal() {
      rotated = !rotated;
      createSignal(rotated);
      ding.play();
    }

    createSignal(rotated);
  </script>
</body>
</html>
