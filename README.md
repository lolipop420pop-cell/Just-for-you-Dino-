<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Just for You 💗</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      background: radial-gradient(circle, #2b0033, #000);
      display: flex;
      align-items: center;
      justify-content: center;
      font-family: 'Comic Sans MS', cursive;
      color: white;
      text-align: center;
    }
    .box {
      padding: 30px;
    }
    .heart {
      font-size: 60px;
      animation: pulse 1.5s infinite;
    }
    @keyframes pulse {
      0% { transform: scale(1); }
      50% { transform: scale(1.2); }
      100% { transform: scale(1); }
    }
    button {
      margin-top: 20px;
      padding: 12px 25px;
      font-size: 18px;
      border: none;
      border-radius: 25px;
      background: hotpink;
      color: white;
      cursor: pointer;
    }
  </style>
</head>
<body>

<div class="box" id="content">
  <div class="heart">💗</div>
  <h2>Will you do me a small favor?</h2>
  <button onclick="next()">Open it 🤍</button>
</div>

<script>
  function next() {
    document.getElementById("content").innerHTML = `
      <div class="heart">💖</div>
      <h2>I just wanted to say…</h2>
      <p>tum pagal ho 🤪🤪🐵.  
      <br>And this is only for you pagal 🤪</p>
    `;
  }
</script>

</body>
</html>
