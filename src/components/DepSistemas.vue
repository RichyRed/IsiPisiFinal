<template>
    <div class="dep-sistemas">
      <h1 class="title">Departamento de Sistemas</h1>
  
      <!-- Sección intermedia 1 -->
      <div class="section">
        <div class="text-container">
          <h2 class="subtitle">Gestión Avanzada de Inventario</h2>
          <p class="text">
            En el Departamento de Sistemas de IsiPisi, implementamos tecnologías avanzadas para una gestión de inventario precisa. Garantizamos que cada prenda en nuestro catálogo esté siempre disponible para nuestros usuarios. La magia está en la eficiencia de nuestro sistema.
          </p>
        </div>
        <div class="text-container">
          <h2 class="subtitle">Logística Inteligente</h2>
          <p class="text">
            
            Nuestro equipo de Sistemas en IsiPisi se dedica a la planificación de rutas inteligentes. Desde el almacén hasta tu puerta, optimizamos la logística para garantizar entregas sin contratiempos. La eficacia de nuestro sistema se traduce en una experiencia de compra sin complicaciones para ti.
          </p>
        </div>
      </div>
  
      <!-- Sección intermedia 2 -->
      <div class="section">
        <div class="text-container">
          <h2 class="subtitle">Almacenamiento Estratégico</h2>
          <p class="text">
            En IsiPisi, el Departamento de Sistemas se encarga de la logística de almacenamiento de manera estratégica. Cada prenda es gestionada con precisión, asegurando que estén listas para llegar a tu hogar. Desde el almacén hasta tus manos, cada paso es parte de nuestra estrategia para ofrecerte lo mejor.
          </p>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: "DepSistemas",
  };
  </script>
  
  <style scoped>
  .dep-sistemas {
    text-align: center;
    padding: 20px;
  }
  
  .title {
    font-size: 2em;
    margin-bottom: 20px;
  }
  
  .section {
    display: flex;
    flex-direction: row;
    justify-content: space-evenly;
    align-items: center;
    gap: 400px;
  }
  
  .subtitle {
    font-size: 1.5em;
    margin-bottom: 10px;
    text-align: center; /* Alineación centrada para los títulos de las secciones */
  }
  
  .text-container {
    text-align: justify;
    max-width: 400px;
  }
  
  .text {
    max-width: 100%;
  }
  </style>
  