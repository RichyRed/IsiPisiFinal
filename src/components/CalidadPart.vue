<template>
    <div class="calidad-part">
      <h1 class="title">Departamento de Operaciones y Logística</h1>
  
      <!-- Sección superior -->
      <div class="section">
        <div class="text-container">
          <h2 class="subtitle">Catálogo Dinámico</h2>
          <p class="text">
            En nuestro Departamento de Operaciones y Logística, nos dedicamos a mantener un catálogo dinámico que refleje la diversidad y calidad de la moda boliviana. Desde prendas de diseño único hasta clásicos atemporales, actualizamos continuamente nuestro catálogo para ofrecerte siempre lo mejor.
          </p>
        </div>
      </div>
  
      <!-- Sección intermedia 1 -->
      <div class="section">
        <div class="text-container">
          <h2 class="subtitle">Organización Precisa</h2>
          <p class="text">
            Cada prenda tiene su lugar único en IsiPisi. Nuestro equipo de operaciones asigna cuidadosamente categorías y etiquetas a los productos, facilitando a los usuarios encontrar exactamente lo que están buscando. La organización es la clave para una experiencia de compra sin complicaciones.
          </p>
        </div>
        <div class="text-container">
          <h2 class="subtitle">Gestión Eficiente del Inventario</h2>
          <p class="text">
            En IsiPisi, gestionamos nuestro inventario con precisión para garantizar que cada prenda en nuestro catálogo esté disponible para ti. Nuestro Departamento de Operaciones se asegura de mantener un flujo constante de existencias, para que encuentres tus favoritos cuando los necesites.
          </p>
        </div>
      </div>
  
      <!-- Sección intermedia 2 -->
      <div class="section">
        <div class="text-container">
          <h2 class="subtitle">Logística Perfecta</h2>
          <p class="text">
            La magia sucede en el backstage. Nuestro equipo de Operaciones y Logística planifica rutas de entrega eficientes y gestiona estratégicamente el almacenamiento para que tu experiencia de compra no solo sea emocionante, sino también rápida y confiable. Desde el almacén hasta tu puerta, estamos aquí para hacerlo posible.
          </p>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: "CalidadPart",
  };
  </script>
  
  <style scoped>
  .calidad-part {
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
  