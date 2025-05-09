<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Para Mi Reina</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background-color: #fff0f5;
      text-align: center;
      padding: 0;
    }
    .container {
      padding: 20px;
    }
    img {
      max-width: 90%;
      border-radius: 15px;
      margin-top: 20px;
    }
    .hidden {
      display: none;
    }
    .message {
      font-size: 1.2em;
      margin: 20px;
      color: #333;
    }
    input[type="password"] {
      padding: 10px;
      font-size: 1em;
      margin-top: 15px;
    }
    button {
      padding: 10px 20px;
      font-size: 1em;
      margin-top: 10px;
      cursor: pointer;
      background-color: #ff69b4;
      border: none;
      color: white;
      border-radius: 5px;
    }
    button:hover {
      background-color: #ff1493;
    }
  </style>
</head>
<body>
  <div class="container" id="pantalla1">
    <h2>Buenos días mi reina linda 💖</h2>
    <p class="message">Espero te encuentres súper bien. Pasaba por acá a desearte un gran día y a decirte algo bonito...</p>
    <img src="foto1.jpg" alt="Foto de nosotros">
    <p class="message">Ingresa una clave especial para continuar:</p>
    <input type="password" id="clave" placeholder="DD/MM/AAAA">
    <br>
    <button onclick="verificarClave()">Continuar</button>
  </div>

  <div class="container hidden" id="pantalla2">
    <img src="foto2.jpg" alt="Cena romántica">
    <p class="message">
      Amorcito mío, quiero recordarte que hoy hace 7 años dimos el paso más lindo de ser novios y un gran equipo. 💑<br><br>
      Por este motivo quiero que lo celebremos de una manera bonita:<br>
      <strong>Ir a cenar juntos</strong>, compartir en un restaurante lindo.<br><br>
      Alístate mi reina hermosa, <strong>te recojo hoy 11/05/2025 a las 7PM</strong>.<br>
      ¡Ponte súper linda! 💕
    </p>
  </div>

  <script>
    function verificarClave() {
      const clave = document.getElementById('clave').value;
      if (clave === "11/05/2018") {
        document.getElementById('pantalla1').classList.add('hidden');
        document.getElementById('pantalla2').classList.remove('hidden');
      } else {
        alert("Clave incorrecta. Intenta nuevamente, mi amor 💗");
      }
    }
  </script>
</body>
</html>
