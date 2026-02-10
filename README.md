<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>San Valentín 💖</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #ffe6eb;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      text-align: center;
    }
    button {
      font-size: 20px;
      padding: 15px 30px;
      margin: 10px;
      cursor: pointer;
    }
    #no {
      position: relative;
    }
  </style>
</head>
<body>

<div id="container">
  <h1>¿Quieres ser mi San Valentín? 💘</h1>
  <button id="si" onclick="acepta()">Sí</button>
  <button id="no" onclick="crece()">No</button>
</div>

<script>
  let size = 20;

  function crece() {
    size += 15;
    document.getElementById("si").style.fontSize = size + "px";
  }

  function acepta() {
    document.body.innerHTML = `
      <h1>💖 Cita San Valentín 💖</h1>
      <p>📅 14 de febrero</p>
      <p>⏰ 12:00</p>
      <p>📍 En mi casa</p>
      <p>Por favor no me dejes plantado 🥺</p>
      <h2>Te amo ❤️</h2>
    `;
  }
</script>

</body>
</html>
