<!DOCTYPE html>
<html>
<head>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    .carousel {
      display: flex;
      overflow-x: scroll;
      scroll-snap-type: x mandatory;
    }
    
    .carousel form {
      flex: 0 0 100%;
      scroll-snap-align: start;
      width: 100%;
    }
    
    @media (min-width: 600px) {
      .carousel form {
        width: 600px;
      }
    }
  </style>
</head>
<body>
  <div class="carousel">
    <form src="https://docs.google.com/forms/d/e/1FAIpQLSeRomDRTp91g38eXqq7IbwNO41PnaJ-xcxa8PnLLx7aIigf5A/viewform?usp=sf_link"></form>
    <form src="https://docs.google.com/forms/d/e/1FAIpQLSfhfPg_HbWAvizRkyx4S014Mq_upVne_eowDrCPExZIHpm2WQ/viewform?usp=sf_link"></form>
  </div>

  <script>
    // Adicionar a funcionalidade de carrossel usando JavaScript ou uma biblioteca de terceiros
    // Exemplo usando a biblioteca Flickity: https://flickity.metafizzy.co/
    // Certifique-se de incluir a biblioteca correspondente no código.
    // Aqui está um exemplo simples de como usar o Flickity:
    /*
    document.addEventListener("DOMContentLoaded", function() {
      var flkty = new Flickity('.carousel', {
        wrapAround: true,
        freeScroll: true,
        contain: true
      });
    });
    */
  </script>
</body>
</html>
