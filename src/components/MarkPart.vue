<template>
    <div class="mark-part">
      <h1 class="title">Marketing</h1>
  
      <!-- Sección 1 -->
      <div class="section">
        <img src="../assets/mkt1.jpeg" alt="Marketing Image 1" class="image" />
        <div class="text-container">
          <h2 class="subtitle">Estrategia de Contenido</h2>
          <p class="text">
            Nuestro equipo de marketing se centrará en contar las historias cautivadoras detrás de cada prenda y emprendedor en IsiPisi. Crearemos contenido atractivo para redes sociales, blogs y newsletters, destacando la diversidad y la calidad de la moda boliviana.
          </p>
        </div>
      </div>
  
      <!-- Sección 2 -->
      <div class="section">
        <div class="text-container">
          <h2 class="subtitle">Alianzas Estratégicas</h2>
          <p class="text">
            Estableceremos alianzas con influencers, blogueros y medios de moda para amplificar nuestro mensaje. Queremos que IsiPisi sea una voz reconocida en la escena de la moda boliviana, colaborando con aquellos que comparten nuestra visión.
          </p>
        </div>
        <img src="../assets/mkt2.jpg" alt="Marketing Image 2" class="image" />
      </div>
  
      <!-- Sección 3 -->
      <div class="section">
        <img src="../assets/mkt3.png" alt="Marketing Image 3" class="image" />
        <div class="text-container">
          <h2 class="subtitle">Publicidad Segmentada</h2>
          <p class="text">
            Utilizaremos estrategias publicitarias específicas para llegar a nuestro público objetivo. La publicidad segmentada nos permitirá dirigirnos de manera efectiva a aquellos que están más interesados en la moda boliviana y los productos exclusivos de IsiPisi.
          </p>
        </div>

      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: "MarkPart",
  };
  </script>
  
  <style scoped>
  .mark-part {
    text-align: center;
    padding: 50px;
  }
  
  .title {
    font-size: 2em;
    margin-bottom: 10px;
  }
  
  .section {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 10px;
  }
  
  .image {
    max-width: 40%;
    height: auto;
    margin: 0 100px; /* Ajusta el margen aquí */
  }
  
  .text-container {
    max-width: 50%;
    margin: 0 100px; /* Ajusta el margen aquí */
  }
  
  .subtitle {
    font-size: 1.5em;
    margin-bottom: 10px;
  }
  
  .text {
    text-align: justify;
  }
  </style>
  