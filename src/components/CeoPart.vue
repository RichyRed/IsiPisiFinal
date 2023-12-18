<template>
    <div class="ceo">
      <!-- Sección del CEO -->
      <div class="ceo-section">
        <p class="ceo-text">CEO</p>
        <img
          src="../assets/gabriel.png"
          alt="CEO Image"
          class="ceo-image"
          :style="{ marginRight: ceoImageMargin }"
        />
      </div>
  
      <!-- Sección de Textos -->
      <div class="text-section">
        <div class="text-container">
          <h2>¿Quién Soy?</h2>
          <p>
            Soy Gabriel, el fundador y CEO de IsiPisi. Mi pasión por la moda local y el emprendimiento me llevó a crear esta plataforma. Con una visión clara y el compromiso de impulsar a los emprendedores bolivianos, lidero un equipo dedicado a transformar la forma en que experimentamos y apoyamos la moda en Bolivia.
          </p>
        </div>
  
        <div class="text-container">
          <h2>CEO - Misión Personal</h2>
          <p>
            Mi misión es clara: empoderar a los emprendedores bolivianos a través de IsiPisi. Busco no solo maximizar el alcance de sus negocios, sino también destacar la diversidad y creatividad de la moda en Bolivia. Cada paso que damos es un avance hacia un ecosistema de moda local más fuerte y sostenible.
          </p>
        </div>
  
        <div class="text-container">
          <h2>CEO - Visión para IsiPisi</h2>
          <p>
            Mi visión para IsiPisi va más allá de una plataforma de moda. Visualizo un cambio significativo en la industria boliviana, donde cada emprendedor tenga la oportunidad de alcanzar sus metas y cada consumidor se conecte con la autenticidad de la moda local. Estoy comprometido a liderar IsiPisi hacia un futuro donde la moda boliviana sea reconocida y celebrada a nivel mundial.
          </p>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: "CeoPart",
    data() {
      return {
        ceoImageMargin: "70px", // Espacio predeterminado, puedes ajustar según sea necesario
      };
    },
  };
  </script>
  
  <style scoped>
  .ceo {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px;
  }
  
  .ceo-section {
    display: flex;
    align-items: center;
  }
  
  .ceo-text {
    font-size: 2em;
    writing-mode: vertical-rl; /* Texto vertical */
  }
  
  .ceo-image {
    max-width: 15em; /* Tamaño igual al texto "CEO" */
    height: auto;
  }
  
  .text-section {
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: flex-start; /* Cambiado de 'center' a 'flex-start' */
  }
  
  .text-container {
    text-align: justify;
    margin-bottom: 25px; /* Espacio entre los bloques de texto */
  }
  
  h2 {
    font-size: 1.5em;
    margin-bottom: 10px; /* Espacio entre el título y el texto */
  }
  </style>
  