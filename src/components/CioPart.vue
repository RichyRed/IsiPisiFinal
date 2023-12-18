<template>
    <div class="cio-part">
      <!-- Sección de Textos -->
      <div class="text-section">
        <div class="text-container">
          <h2>¿Quien Soy?</h2>
          <p>
            Como Chief Information Officer (CIO) de IsiPisi, soy [Nombre del CIO], apasionado por la innovación tecnológica y su impacto en el comercio. Mi experiencia y visión se centran en aprovechar la tecnología de manera estratégica para llevar la experiencia de compra en línea de moda boliviana a nuevas alturas, creando soluciones eficientes y efectivas.
          </p>
        </div>
  
        <div class="text-container">
          <h2>CIO - Misión Tecnológica</h2>
          <p>
            Mi misión en IsiPisi es fusionar la tecnología con la moda de manera fluida y eficiente. Trabajo incansablemente para garantizar que nuestra plataforma esté a la vanguardia, ofreciendo una experiencia de usuario intuitiva y segura. Mi objetivo es aprovechar la tecnología para potenciar los emprendimientos locales y transformar la forma en que se conectan con sus clientes.
          </p>
        </div>
  
        <div class="text-container">
          <h2>CIO - Visión Tecnológica</h2>
          <p>
            Mi visión para la tecnología en IsiPisi es ser líderes en innovación. Busco establecer un ecosistema tecnológico que no solo cumpla con las demandas actuales, sino que también anticipe las tendencias futuras. Visualizo una plataforma que utilice la inteligencia artificial, la analítica de datos y las últimas tecnologías para brindar una experiencia de compra personalizada y memorable.
          </p>
        </div>
      </div>
  
      <!-- Sección del CIO -->
      <div class="cio-section">
        <img
          src="../assets/producto2.png"
          alt="CIO Image"
          class="cio-image"
          :style="{ marginLeft: cioImageMargin }"
        />
        <p class="cio-text">CIO</p>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: "CioPart",
    data() {
      return {
        cioImageMargin: "70px", // Espacio predeterminado, puedes ajustar según sea necesario
      };
    },
  };
  </script>
  
  <style scoped>
  .cio-part {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px;
  }
  
  .text-section {
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
  }
  
  .text-container {
    text-align: justify;
    margin-bottom: 25px; /* Espacio entre los bloques de texto */
  }
  
  h2 {
    font-size: 1.5em;
    margin-bottom: 10px; /* Espacio entre el título y el texto */
  }
  
  .cio-section {
    display: flex;
    align-items: center;
  }
  
  .cio-image {
    max-width: 15em; /* Tamaño igual al texto "CIO" */
    height: auto;
    margin-right: 20px; /* Espacio entre la imagen y los textos */
  }
  
  .cio-text {
    font-size: 2em;
    writing-mode: vertical-rl; /* Texto vertical */
    margin-left: 10px; /* Espacio entre la imagen y el texto */
  }
  </style>
  