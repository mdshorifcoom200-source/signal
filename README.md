# signal
Ledar Shorif hack
<!DOCTYPE html>
<html>
<head>
  <title>Win Go Signal</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>

<h2>Win Go Signal</h2>

<select id="signal">
  <option>BIG</option>
  <option>SMALL</option>
  <option>RED</option>
  <option>GREEN</option>
</select>

<button onclick="setSignal()">Set Signal</button>

<h3 id="output">Waiting...</h3>

<script src="script.js"></script>
</body>
</html>
function setSignal() {
  let s = document.getElementById("signal").value;
  document.getElementById("output").innerText =
    "Next Signal: " + s;
}

setInterval(() => {
  document.getElementById("output").innerText = "Waiting...";
}, 30000);
body {
  text-align: center;
  font-family: Arial;
  background: #111;
  color: #0f0;
}
button {
  padding: 10px;
  margin-top: 10px;
}
