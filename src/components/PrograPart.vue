<template>
    <div class="progra-part">
      <h1 class="title">Departamento Financiero y Administrativo</h1>
      <div class="sections">
        <!-- Sección 1 -->
        <div class="section">
          <h2>Pago Seguro y Fácil</h2>
          <p>
            En el Departamento Financiero y Administrativo de IsiPisi, nos encargamos del proceso de pago para garantizar una experiencia segura y fácil. Desde la verificación de transacciones hasta la gestión de pagos, trabajamos para que cada compra sea una transacción confiable.
          </p>
        </div>
  
        <!-- Sección 2 -->
        <div class="section">
          <h2> Verificación Rigurosa</h2>
          <p>
            La seguridad de tus transacciones es nuestra prioridad. Nuestro equipo se dedica a una verificación rigurosa de cada detalle para garantizar la integridad de las transacciones en IsiPisi. Cada compra es tratada con la seriedad que merece.
          </p>
        </div>
  
        <!-- Sección 3 -->
        <div class="section">
          <h2>Gestión Financiera Eficiente</h2>
          <p>
            En IsiPisi, la gestión financiera eficiente es fundamental. Nuestro Departamento Financiero y Administrativo trabaja para mantener un equilibrio en cada número, asegurando la salud financiera de la plataforma y respaldando el crecimiento continuo.
          </p>
        </div>
  
        <!-- Sección adicional 1 -->
        <div class="section">
          <h2>Administración Precisa</h2>
          <p>
            Cada éxito en IsiPisi tiene su base en una administración precisa. Nuestro equipo financiero se asegura de que todos los aspectos administrativos estén en orden, permitiendo que la plataforma crezca de manera sostenible y exitosa.
          </p>
        </div>
  
        <!-- Sección adicional 2 -->
        <div class="section">
          <h2>Transparencia y Confianza</h2>
          <p>
            En IsiPisi, creemos en la transparencia. Nuestro Departamento Financiero y Administrativo trabaja para ofrecerte una experiencia transparente en cada transacción. Construimos confianza a través de la claridad y la honestidad en cada aspecto financiero.
          </p>
        </div>
  
        <!-- Sección adicional 3 -->
        <div class="section">
          <h2>Informes y Análisis</h2>
          <p>
            Nuestro equipo en Finanzas no solo registra números, sino que también genera informes y análisis que impulsan decisiones estratégicas. La interpretación inteligente de los datos es clave para la toma de decisiones informadas en IsiPisi.
          </p>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: "PrograPart",
  };
  </script>
  
  <style scoped>
  .progra-part {
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
    flex: 0 1 calc(33.33% - 20px); /* 3 secciones en una fila con espacio entre ellas */
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
  