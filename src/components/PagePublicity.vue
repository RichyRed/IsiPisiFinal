<template>
    <div class="page-publicity">
      <h1>{{ pageTitle }}</h1>
      <div class="image-carousel">
        <img :src="currentImage" alt="Publicity Image" />
        <button @click="prevImage" class="arrow left">&lt;</button>
        <button @click="nextImage" class="arrow right">&gt;</button>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        pageTitle: "Publicidad",
        images: [
          require("@/assets/producto1.png"),
          require("@/assets/producto2.png"),
          require("@/assets/producto3.png"),
        ],
        currentIndex: 0,
      };
    },
    computed: {
      currentImage() {
        return this.images[this.currentIndex];
      },
    },
    methods: {
      nextImage() {
        this.currentIndex = (this.currentIndex + 1) % this.images.length;
      },
      prevImage() {
        this.currentIndex = (this.currentIndex - 1 + this.images.length) % this.images.length;
      },
    },
    mounted() {
      // Cambiar automáticamente las imágenes cada 5 segundos
      setInterval(() => {
        this.nextImage();
      }, 5000);
    },
  };
  </script>
  
  <style scoped>
  .page-publicity {
    text-align: center;
  }
  
  .image-carousel {
    position: relative;
  }
  
  img {
    max-width: 100%;
    max-height: 300px; /* Ajusta la altura según tus necesidades */
  }
  
  .arrow {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    font-size: 24px;
    background: none;
    border: none;
    cursor: pointer;
  }
  
  .left {
    left: 10px;
  }
  
  .right {
    right: 10px;
  }
  </style>
  