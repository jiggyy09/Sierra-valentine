# Sierra-valentine
Sierra-valentine
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Sierra 💖</title>
<style>
body {
  background: linear-gradient(135deg, #ff9a9e, #fad0c4);
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: 'Arial', sans-serif;
  margin: 0;
}

.card {
  background: white;
  padding: 40px;
  border-radius: 20px;
  text-align: center;
  box-shadow: 0 20px 40px rgba(0,0,0,0.2);
}

h1 {
  font-size: 2.5rem;
  color: #ff4d6d;
}

p {
  font-size: 1.2rem;
}

.buttons {
  margin-top: 30px;
}

button {
  font-size: 1.1rem;
  padding: 12px 25px;
  border: none;
  border-radius: 30px;
  cursor: pointer;
  margin: 10px;
}

#yes {
  background: #ff4d6d;
  color: white;
}

#no {
  background: #ddd;
  position: absolute;
}
</style>
</head>

<body>
<div class="card">
  <h1>Sierra 💕</h1>
  <p>From the moment I met you, my days got brighter.</p>
  <p>So I gotta ask…</p>
  <h2>Will you be my Valentine? 💘</h2>

  <div class="buttons">
    <button id="yes" onclick="yesClicked()">YES 💖</button>
    <button id="no" onmouseover="moveNo()">No 😅</button>
  </div>
</div>

<script>
function moveNo() {
  const button = document.getElementById('no');
  const x = Math.random() * (window.innerWidth - 100);
  const y = Math.random() * (window.innerHeight - 100);
  button.style.left = x + 'px';
  button.style.top = y + 'px';
}

function yesClicked() {
  document.body.innerHTML = `
    <div style="text-align:center; padding-top:20vh;">
      <h1 style="color:#ff4d6d;">YAYYY 💕</h1>
      <h2>Sierra, you just made me the happiest person ever 🥹</h2>
      <p>Happy Valentine’s Day 💖</p>
    </div>
  `;
}
</script>
</body>
</html>
