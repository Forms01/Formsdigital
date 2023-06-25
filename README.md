# Formsdigital
<!doctype html>
<html> 
 <head> 
  <meta name="viewport" content="width=device-width, initial-scale=1.0"> 
  <title>Formulários Google</title> 
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
    }
    
    .container {
      max-width: 600px;
      margin: 0 auto;
      padding: 20px;
    }
    
    .form-container {
      display: none;
    }
    
    .form-container.active {
      display: block;
    }
    
    .form-iframe {
      width: 100%;
      height: 600px;
      border: none;
    }
    
    .carousel-navigation {
      text-align: center;
    }
    
    .carousel-navigation button {
      display: inline-block;
      margin: 5px;
      padding: 5px 10px;
      background-color: #ccc;
      border: none;
      cursor: pointer;
    }
  </style> 
  <script>
    document.addEventListener("DOMContentLoaded", function() {
      const formContainers = Array.from(document.querySelectorAll(".form-container"));
      const navigationButtons = Array.from(document.querySelectorAll(".carousel-navigation button"));
      
      let currentIndex = 0;
      
      function showForm(index) {
        formContainers.forEach((container, i) => {
          container.classList.remove("active");
          navigationButtons[i].classList.remove("active");
        });
        
        formContainers[index].classList.add("active");
        navigationButtons[index].classList.add("active");
      }
      
      function handleClick(event) {
        const buttonIndex = navigationButtons.indexOf(event.target);
        if (buttonIndex !== -1) {
          currentIndex = buttonIndex;
          showForm(currentIndex);
        }
      }
      
      navigationButtons.forEach(button => {
        button.addEventListener("click", handleClick);
      });
      
      showForm(currentIndex);
    });
  </script> 
 </head> 
 <body> 
  <div class="container"> 
   <div class="carousel-navigation"> <button class="active">Formulario de teste diario PDM</button> <button>Formulario de teste semanal PDM</button> 
   </div> 
   <div class="form-container"> <iframe class="form-iframe" src="https://docs.google.com/forms/d/e/1FAIpQLSeRomDRTp91g38eXqq7IbwNO41PnaJ-xcxa8PnLLx7aIigf5A/viewform?embedded=true" frameborder="0" marginheight="0" marginwidth="0">Carregando…</iframe> 
   </div> 
   <div class="form-container"> <iframe class="form-iframe" src="https://docs.google.com/forms/d/e/1FAIpQLSfhfPg_HbWAvizRkyx4S014Mq_upVne_eowDrCPExZIHpm2WQ/viewform?embedded=true" frameborder="0" marginheight="0" marginwidth="0">Carregando…</iframe> 
   </div> 
  </div> 
 </body>
</html>
