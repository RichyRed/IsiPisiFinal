<template>
    <nav
      class="navbar navbar-expand-md navbar-dark bg-dark fixed-top"
      style="height: 85px"
      :class="{ transparent: isTransparent }"
    >
      <a class="navbar-brand" href="#inicio">
        <img
          src="../assets/jam.png"
          alt="Logo"
          width="auto"
          height="40"
          class="m-3"
        />
      </a>
  
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav mr-auto">
          <li class="nav-item">
            <a class="nav-link text-white" href="#inicio">Principal</a>
          </li>
          <li class="nav-item">
            <a class="nav-link text-white" href="#about-us">Quienes Somos</a>
          </li>
          <li class="nav-item">
            <a class="nav-link text-white" href="#ceo">CEO</a>
          </li>
          <li class="nav-item">
            <a class="nav-link text-white" href="#support-part">Departamentos</a>
          </li>
          <li class="nav-item">
            <a class="nav-link text-white" href="#team">Equipo</a>
          </li>
          <li class="nav-item">
            <a class="nav-link text-white" href="#images-part">Diagramas</a>
          </li>
          <li class="nav-item">
            <a class="nav-link text-white" href="#fase-plan">Documentos</a>
          </li>
        </ul>
      </div>
      <a
        href="https://wa.me/59165165908"
        target="_blank"
        class="navbar-text m-3 d-flex justify-content-end text-white"
      >
        <img
          src="../assets/IsiBlanco.png"
          alt="WhatsApp"
          width="auto"
          height="55"
        />
      </a>
    </nav>
  </template>
  
  <script>
  export default {
    data() {
      return {
        isTransparent: true,
      };
    },
    mounted() {
      window.addEventListener("scroll", this.handleScroll);
    },
    beforeUnmount() {
      window.removeEventListener("scroll", this.handleScroll);
    },
    methods: {
      handleScroll() {
        this.isTransparent = window.pageYOffset === 0;
      },
    },
  };
  </script>
  
  <style scoped>
  .navbar {
    background-color: rgba(0, 0, 0, 0.85) !important;
    transition: background-color 0.3s ease;
  }
  
  .transparent {
    background-color: transparent !important;
  }
  
  .text-white {
    color: white !important;
  }
  
  .text-black {
    color: black !important;
  }
  </style>