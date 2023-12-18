<template>
    <div class="exp-cliente">
      <h1 class="title">Departamento de Experiencia del Cliente</h1>
      <div class="sections">
        <!-- Sección 1 -->
        <div class="section">
          <h2>Servicio Personalizado</h2>
          <p>
            En el Departamento de Experiencia del Cliente de IsiPisi, estamos aquí para ti. Desde consultas hasta asistencia con pedidos, nuestro equipo se dedica a proporcionarte un servicio personalizado. Tu satisfacción es nuestra prioridad número uno.
          </p>
        </div>
  
        <!-- Sección 2 -->
        <div class="section">
          <h2>Consultas Rápidas y Sencillas</h2>
          <p>
            ¿Tienes preguntas? Estamos aquí con respuestas rápidas y soluciones sencillas. Nuestro equipo de Experiencia del Cliente se asegura de que cada consulta se maneje con atención y eficiencia para que tu experiencia de compra sea sin complicaciones.
          </p>
        </div>
  
        <!-- Sección 3 -->
        <div class="section">
          <h2>Problemas Resueltos</h2>
          <p>
            En IsiPisi, entendemos que pueden surgir problemas. Ya sea un problema con tu pedido o una pregunta sobre una entrega, nuestro equipo de Experiencia del Cliente está aquí para convertir cualquier inconveniente en una sonrisa. Tu felicidad es nuestro compromiso.
          </p>
        </div>
  
        <!-- Sección 4 -->
        <div class="section">
          <h2>Feedback Importante</h2>
          <p>
            Valoramos tu opinión. Nuestro equipo de Experiencia del Cliente no solo está aquí para resolver problemas, sino también para escuchar tus comentarios. Cada interacción nos ayuda a mejorar y a ofrecer una experiencia aún mejor en IsiPisi. ¡Tu voz nos guía hacia la excelencia!
          </p>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: "ExpCliente",
  };
  </script>
  
  <style scoped>
  .exp-cliente {
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
  