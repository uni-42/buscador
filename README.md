# buscador
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Nueva pestaña</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: white;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
    }

    .logo {
      font-size: 48px;
      font-weight: bold;
      color: #4285F4;
      margin-bottom: 20px;
    }

    .search-box {
      width: 400px;
      padding: 12px;
      border-radius: 24px;
      border: 1px solid #ccc;
      outline: none;
      font-size: 16px;
      margin-bottom: 20px;
    }

    .btn {
      padding: 10px 20px;
      border: none;
      border-radius: 20px;
      background: #f1f1f1;
      cursor: pointer;
      margin: 5px;
      transition: 0.2s;
    }

    .btn:hover {
      background: #ddd;
    }
  </style>
</head>
<body>

  <div class="logo">Google</div>

  <input class="search-box" placeholder="Buscar en Google...">

  <div>
    <button class="btn" onclick="buscar()">Buscar</button>
    <button class="btn" onclick="abrirJuego()">Voy a tener suerte 😏</button>
  </div>

  <script>
    function buscar() {
      const query = document.querySelector('.search-box').value;
      window.open('https://www.google.com/search?q=' + query, '_blank');
    }

    function abrirJuego() {
      window.open('https://maddoxcloud.com/', '_blank');
    }
  </script>

</body>
</html>
