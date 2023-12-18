<template>
  <section id="informacion">
    <footer class="footer">
      <div class="container">
        <div class="row">
          <!-- Columna para el logo y la sección de contactos -->
          <div class="col-md-6">
            <div class="footer-section">
              <!-- Logo a la izquierda -->
              <div class="footer-logo">
                <img src="../assets/IsiBlanco.png" alt="Logo" class="footer-logo-img" />
              </div>
              <!-- Texto de contacto -->
              <div class="contact-section">
                <h4 class="footer-title">Contacto</h4>
                <p class="footer-text">Correo: soporte.isi@isi.com</p>
                <p class="footer-text">Teléfono: +75821008</p>
              </div>
            </div>
          </div>
          <!-- Columna para el texto genérico -->
          <div class="col-md-6">
            <div class="footer-section">
              <!-- Texto genérico -->
              <p class="footer-text">© 2023 Isi Pisi. Todos los derechos reservados.</p>
              <p class="footer-text">Términos de Servicio | Política de Privacidad</p>
            </div>
          </div>
        </div>
      </div>
    </footer>
  </section>
</template>

<script>
export default {
  name: "FooterSection",
};
</script>

<style>
.footer {
  background-color: #333;
  padding: 20px 0;
  color: #fff;
}

.footer .container {
  max-width: 1350px;
  margin: 0 auto;
}

.footer .row {
  display: flex;
  align-items: center;
}

.footer-logo-img {
  max-width: 40%;
  height: auto;
}

.footer-section {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.contact-section {
  text-align: left;
  margin-right: 120px; /* Ajusta el margen derecho según tu preferencia */
}

.footer-title {
  font-size: 16px;
  color: #fff;
}

.footer-text {
  margin: 5px 0;
  font-size: 14px;
}

.footer-text a {
  color: #fff;
  text-decoration: none;
  transition: color 0.3s;
}

.footer-text a:hover {
  color: #bbb;
}
</style>
