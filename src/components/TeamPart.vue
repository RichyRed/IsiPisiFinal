<template>
    <section id="team">
      <div class="pt-5 pb-5">
        <div class="container">
          <h2 class="text-center mb-4 team-title">Equipo</h2>
          <!-- Primera fila de cards -->
          <div class="row justify-content-center mt-5">
            <div v-for="card in firstRowCards" :key="card.id" class="col-md-4">
              <div class="card-wrapper" @mouseover="toggleOverlay(card.id)" @mouseleave="toggleOverlay(card.id)">
                <div class="card mb-4">
                  <div class="card-img-wrapper">
                    <div class="img-wrapper">
                      <img :src="card.imageSrc" :alt="card.imageAlt" class="card-img-top custom-img" />
                      <div v-show="card.hovered" class="img-overlay">
                        <div class="hover-content">
                          <p class="hover-text">{{ card.hoverText }}</p>
                        </div>
                      </div>
                    </div>
                    <div class="card-title">
                      <h4>{{ card.title }}</h4>
                    </div>
                  </div>
                  <div class="card-body text-center">
                    <!-- Aquí puedes agregar cualquier contenido adicional para el cuerpo de la tarjeta -->
                  </div>
                </div>
              </div>
            </div>
          </div>
          <!-- Segunda fila de cards -->
          <div class="row justify-content-center mt-5">
            <div v-for="card in secondRowCards" :key="card.id" class="col-md-4">
              <div class="card-wrapper" @mouseover="toggleOverlay(card.id)" @mouseleave="toggleOverlay(card.id)">
                <div class="card mb-4">
                  <div class="card-img-wrapper">
                    <div class="img-wrapper">
                      <img :src="card.imageSrc" :alt="card.imageAlt" class="card-img-top custom-img" />
                      <div v-show="card.hovered" class="img-overlay">
                        <div class="hover-content">
                          <p class="hover-text">{{ card.hoverText }}</p>
                        </div>
                      </div>
                    </div>
                    <div class="card-title">
                      <h4>{{ card.title }}</h4>
                    </div>
                  </div>
                  <div class="card-body text-center">
                    <!-- Aquí puedes agregar cualquier contenido adicional para el cuerpo de la tarjeta -->
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
  </template>
  
  <script>
  export default {
    data() {
      return {
        firstRowCards: [
          {
            id: 1,
            imageSrc: require("../assets/ariane.png"),
            imageAlt: "Team Member 1",
            hoverText: "Departamento de Marketing y Promoción",
            hovered: false,
            title: "Ariane", // Añadido título a la tarjeta
          },
          { 
            id: 2,
            imageSrc: require("../assets/gabriel.png"),
            imageAlt: "Team Member 2",
            hoverText: "Departamento de Sistemas",
            hovered: false,
            title: "Gabriel", // Añadido título a la tarjeta
          },
          {
            id: 3,
            imageSrc: require("../assets/richard.png"),
            imageAlt: "Team Member 3",
            hoverText: "Departamento de Incorporación de Emprendimientos ",
            hovered: false,
            title: "Richard", // Añadido título a la tarjeta
          },
        ],
        secondRowCards: [
          {
            id: 4,
            imageSrc: require("../assets/pablo.png"),
            imageAlt: "Team Member 4",
            hoverText: "Departamento de Operaciones y Logística",
            hovered: false,
            title: "Pablo", // Añadido título a la tarjeta
          },
          {
            id: 5,
            imageSrc: require("../assets/TrajesitoIsi.png"),
            imageAlt: "Team Member 5",
            hoverText: "Departamento Financiero y Administrativo",
            hovered: false,
            title: "Juan", // Añadido título a la tarjeta
          },
          {
            id: 6,
            imageSrc: require("../assets/miguel.png"),
            imageAlt: "Team Member 6",
            hoverText: "Departamento de Experiencia del Cliente",
            hovered: false,
            title: "Miguel", // Añadido título a la tarjeta
          },
        ],
      };
    },
    methods: {
      toggleOverlay(cardId) {
        const allCards = [...this.firstRowCards, ...this.secondRowCards];
        allCards.forEach((card) => {
          card.hovered = card.id === cardId;
        });
      },
    },
  };
  </script>

<style scoped>
/* Estilos de imagen y overlay */
.custom-img {
  height: 230px; /* Ajusta la altura según tu preferencia */
  width: 60%; /* Ajusta el ancho según tu preferencia */
  object-fit: cover;
  border-radius: 10px;
}

.img-wrapper {
  position: relative;
  overflow: hidden;
  height: auto; /* Cambiado a altura automática */
}

.img-overlay {
  position: absolute;
  top: 0;
  left: 0;
  height: 230px; /* Ajusta la altura del overlay según tu preferencia */
  width: 90%; /* Ajusta el ancho del overlay según tu preferencia */
  background-color: rgba(0, 0, 0, 0.6);
  opacity: 0;
  border-radius: 10px; /* Ajusta el radio de borde según tu preferencia */
  transition: opacity 0.3s ease;
}

.card-wrapper {
  position: relative;
}

.card-wrapper:hover .img-overlay {
  opacity: 1;
}

.hover-content {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 100%;
}

.hover-text {
  color: white; /* Cambiado a blanco */
}

.card {
  border: none;
  border-radius: 10px;
  overflow: hidden;
  margin: 20px; /* Espacio entre cada card */
}

.card-body {
  padding: 20px;
}

.card-text {
  color: #000000;
  text-align: center;
  font-weight: bold;
  font-size: 20px;
}

.bigger-text {
  font-size: 24px;
  color: rgb(240, 98, 4);
  font-weight: bold;
}

.team-title {
  color: black; /* Cambiado a negro */
  font-weight: bold;
}

.card-img-top {
  height: 230px;
  width: 90%;
  object-fit: cover;
  border-radius: 10px;
}

.card-title {
  writing-mode: vertical-rl;
  text-orientation: upright;
  white-space: nowrap;
  margin-left: 10px;
}

.card-img-wrapper {
  display: flex;
  align-items: center;
}

.card-img-top::after {
  content: '{{ card.title }}'; /* Cambia 'card.title' por tu palabra */
  position: absolute;
  top: 50%;
  right: -20px; /* Ajusta la distancia del título a la derecha según tu preferencia */
  transform: translateY(-50%) rotate(90deg);
  white-space: nowrap;
}
</style>