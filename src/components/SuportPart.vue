<template>
    <div class="support-part">
      <h1 class="title">Departamento de Incorporación de Emprendimientos</h1>
      <div class="sections">
        <!-- Sección 1 -->
        <div class="section">
          <h2>Registro de Emprendimientos</h2>
          <p>
            En IsiPisi, celebramos la diversidad de la moda boliviana y damos la bienvenida a nuevos talentos. Nuestro Departamento de Incorporación de Emprendimientos se encarga de hacer que tu registro en nuestra plataforma sea un proceso sencillo y enriquecedor. Únete a nosotros y permite que tu creatividad brille en el mundo digital.
          </p>
        </div>
  
        <!-- Sección 2 -->
        <div class="section">
          <h2>Verificación de Calidad</h2>
          <p>
            La calidad es nuestra prioridad. Nuestro equipo de incorporación se compromete a verificar cada emprendimiento y producto para asegurar que cumpla con nuestros estándares. Trabajamos mano a mano contigo para garantizar que tu presencia en IsiPisi sea sinónimo de calidad y autenticidad.
          </p>
        </div>
  
        <!-- Sección 3 -->
        <div class="section">
          <h2>Comunicación Personalizada</h2>
          <p>
            En IsiPisi, entendemos la importancia de la comunicación efectiva. Nuestro equipo de incorporación no solo verifica tu emprendimiento, sino que también te ofrece asistencia personalizada para cargar tus productos. Estamos aquí para ayudarte a destacar y conectarte con una audiencia más amplia.
          </p>
        </div>
  
        <!-- Sección 4 -->
        <div class="section">
          <h2>Facilitando el Procesoo</h2>
          <p>
            Sabemos que tu tiempo es valioso. En IsiPisi, nos esforzamos por hacer que el proceso de registro y carga de productos sea rápido y eficiente. Nuestro Departamento de Incorporación está aquí para facilitar cada paso, permitiéndote centrarte en lo que mejor sabes hacer: crear moda única y auténtica.
          </p>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: "SupportPart",
  };
  </script>
  
  <style scoped>
  .support-part {
    text-align: center;
    padding: 20px;
  }
  
  .title {
    font-size: 2em;
    margin-bottom: 20px;
  }
  
  .sections {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
  }
  
  .section {
    flex: 0 1 calc(25% - 20px); /* 4 secciones en una fila con espacio entre ellas */
    margin-bottom: 20px;
  }
  
  h2 {
    font-size: 1.5em;
    margin-bottom: 10px;
  }
  
  p {
    text-align: justify;
  }
  </style>
  