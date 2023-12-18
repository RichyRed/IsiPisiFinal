<template>
    <div class="fase-plan">
      <h2 class="text-center mb-4 fase-title">{{ title }}</h2>
      <img :src="imageSrc" :alt="imageAlt" class="fase-image" />
      <div class="subtitles">
        <div class="subtitle">
          <a :href="subtitle1.link" class="subtitle-link">{{ subtitle1.text }}</a>
        </div>
        <div class="subtitle">
          <a :href="subtitle2.link" class="subtitle-link">{{ subtitle2.text }}</a>
        </div>
        <div class="subtitle">
          <a :href="subtitle3.link" class="subtitle-link">{{ subtitle3.text }}</a>
        </div>
      </div>
      <!-- Nuevo título y subtitulos -->
      <h2 class="text-center mb-4 new-title">{{ newTitle }}</h2>
      <div class="subtitles">
        <div class="subtitle">
          <a :href="newSubtitle1.link" class="subtitle-link">{{ newSubtitle1.text }}</a>
        </div>
        <div class="subtitle">
          <a :href="newSubtitle2.link" class="subtitle-link">{{ newSubtitle2.text }}</a>
        </div>
      </div>
      <!-- Nuevo título y subtitulo -->
      <h2 class="text-center mb-4 additional-title">{{ additionalTitle }}</h2>
      <div class="subtitles">
        <div class="subtitle">
          <a :href="additionalSubtitle.link" class="subtitle-link">{{ additionalSubtitle.text }}</a>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        title: "Fase de Planificación",
        imageSrc: require("../assets/jerarquico.png"),
        imageAlt: "Descripción de la imagen",
        subtitle1: { text: "Manual de Funciones", link: "https://docs.google.com/document/d/1r5chdRhAXwVsMvjwzONsyeI59GfgzgypPfMTTC3yqPw/edit" },
        subtitle2: { text: "Manual de Actividades", link: "https://docs.google.com/document/d/1l6SohatpBea1NEUVuxOBGNK4S2cPm4WeJ28tVV0Nha4/edit" },
        subtitle3: { text: "Gestión de Riesgos", link: "https://docs.google.com/document/d/17jpC3tY9vjMt21XUnFL0Vmg39dEPiRTPdzf903izhME/edit" },
        newTitle: "Fase de Control de Calidad y Evaluación de Costos",
        newSubtitle1: { text: "Pruebas de Calidad", link: "https://docs.google.com/document/d/1wqhDRMGpzxMTs7LXV00Zta-NfDVYJR3wmQ1JFBjh5wQ/edit" },
        newSubtitle2: { text: "Estimación de Costos", link: "https://docs.google.com/document/d/1BU6Rda1Y6nMx3DPWG9CrFFdhbkhtOjrYvLS32a3dnvk/edit" },
        additionalTitle: "Fase de Cierre",
        additionalSubtitle: { text: "Conclusiones, Recomendaciones y Plan de Sostenibilidad", link: "https://docs.google.com/document/d/1U_ad_pbZpDFQNYOViKnav7KJEIYp6UjfAuhUU2KMCtA/edit" },
      };
    },
  };
  </script>
  
  <style scoped>
  .fase-plan {
    text-align: center;
    padding: 20px;
  }
  
  .fase-title {
    font-size: 24px;
    font-weight: bold;
    margin-bottom: 20px;
  }
  
  .fase-image {
    width: 100%;
    max-width: 1000px;
    margin-bottom: 20px;
  }
  
  .subtitles {
    display: flex;
    flex-direction: column; /* Cambiado a dirección de columna */
    align-items: center; /* Añadido centrado vertical */
  }
  
  .subtitle {
    width: 30%;
    margin-top: 20px; /* Ajusta el margen superior según tu preferencia */
  }
  
  .subtitle-link {
    display: block;
    padding: 10px;
    background-color: #808080;
    color: white;
    text-decoration: none;
    border-radius: 5px;
  }
  
  .subtitle-link:hover {
    background-color: #555;
  }
  
  /* Nuevo estilo para el nuevo título */
  .new-title,
  .additional-title {
    font-size: 24px;
    font-weight: bold;
    margin-top: 50px; /* Ajusta el margen superior según tu preferencia */
    margin-bottom: 20px;
  }
  </style>
  