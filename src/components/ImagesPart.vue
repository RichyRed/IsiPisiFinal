<template>
    <div class="images-part">
      <h1 class="title">WorkFlow</h1>
  
      <!-- Primera sección de imagen y título -->
      <div class="image-section">
        <img
          class="centered-image"
          src="../assets/workflow.png"
          alt="Imagen 1"
        />
      </div>
  
    </div>
  </template>
  
  <script>
  export default {
    name: "ImagesPart",
  };
  </script>
  
  <style scoped>
  .images-part {
    text-align: center;
    padding: 20px;
  }
  
  .title {
    font-size: 2em;
    margin-bottom: 20px;
  }
  
  .image-section {
    margin-bottom: 30px;
  }
  
  .centered-image {
    max-width: 100%;
    height: auto;
    margin: 0 auto; /* Para centrar la imagen */
  }
  
  .subtitle {
    font-size: 1.5em;
    margin-top: 10px;
  }
  </style>
  