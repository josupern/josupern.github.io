# josupern.github.io
<html>
<head>
 <style>
    .box {
      width: 100px;
      height: 100px;
      background-color: pink;
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 36px;
      cursor: pointer;
    }
    .image-container {
      width: 100%;
      height: 100%;
      display: flex;
      align-items: center;
      justify-content: center;
    }
    .image {
      width: 40%;
      height: 84%;
      object-fit: cover;
    }
    /* Añadido el meta viewport para escalar la página según el dispositivo */
    @viewport {
      width: device-width;
      initial-scale: 1;
    }
    /* Añadido media queries para cambiar el tamaño de la caja según el ancho de la pantalla */
    @media screen and (max-width: 600px) {
      .box {
        width: 40px;
        height: 84px;
        font-size: 24px;
      }
    }
    @media screen and (max-width: 400px) {
      .box {
        width: 40px;
        height: 84px;
        font-size: 18px;
      }
    }
 </style>
</head>
<body>
 <div class="box" onclick="showMessage(event)">
    Clic aquí
 </div>
 <script>
    function showMessage(e) {
      e.stopPropagation();
      alert("¡Feliz cumpleaños, Lau!");
      document.body.innerHTML = "<div class='image-container'><img src='https://img.freepik.com/vector-premium/dibujo-ramo-rosas-amarillas_564737-1587.jpg' alt='Una flor amarilla' class='image'></div>";
    }
 </script>
 <!-- Cambiado el tamaño del iframe para que se adapte al ancho de la pantalla -->
 <iframe src="https://www.youtube.com/embed/pfRR8D4aQW8?autoplay=1&mute=1" width="20%" height="30%" allow="autoplay" margin="auto" display="block"></iframe>
</body>
</html>
