formularios
<!DOCTYPE html>
<html>
<head>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    .carousel-container {
      overflow: hidden;
    }

    .carousel {
      display: flex;
      overflow-x: scroll;
      scroll-snap-type: x mandatory;
      -webkit-overflow-scrolling: touch;
    }

    .carousel form {
      flex: 0 0 100%;
      scroll-snap-align: start;
    }
  </style>
</head>
<body>
  <div class="carousel-container">
    <div class="carousel">
      <form src="https://docs.google.com/forms/d/e/1FAIpQLSeRomDRTp91g38eXqq7IbwNO41PnaJ-xcxa8PnLLx7aIigf5A/viewform?usp=sf_link"></form>
      <form src="https://docs.google.com/forms/d/e/1FAIpQLSfhfPg_HbWAvizRkyx4S014Mq_upVne_eowDrCPExZIHpm2WQ/viewform?usp=sf_link"></form>
    </div>
  </div>

  <script>
    // Adicionar funcionalidade de carrossel usando a biblioteca Flickity
    document.addEventListener("DOMContentLoaded", function() {
      var carousel = document.querySelector('.carousel');
      var flkty = new Flickity(carousel, {
        cellAlign: 'left',
        contain: true,
        prevNextButtons: false,
        pageDots: false,
        resize: true
      });
    });
  </script>

  <!-- Adicione o script da biblioteca Flickity -->
  <script src="https://cdnjs.cloudflare.com/ajax/libs/flickity/2.2.2/flickity.pkgd.min.js"></script>
</body>
</html>
