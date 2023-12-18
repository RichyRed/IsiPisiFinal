<template>
  <div>
    <NavBar></NavBar>
    <body>
      <CoverImage />
      <PagePublicity />
      <AboutUs />
      <CeoPart />
      <CioPart />
      <SupportPart />
      <CalidadPart />
      <ExpCliente />
      <DepSistemas />
      <MarkPart />
      <PrograPart />
      <TeamPart />
      <ImagePart />
      <FasePlan />
    </body>
    <Footer></Footer>
  </div>
</template>

<script>
import NavBar from "./components/NavBar.vue";
import Footer from "./components/Footer.vue";
import PagePublicity from "./components/PagePublicity.vue";
import CoverImage from "./components/CoverImage.vue";
import AboutUs from "./components/AboutUs.vue";
import ImagePart from "./components/ImagesPart.vue"
import CeoPart from "./components/CeoPart.vue";
import CioPart from "./components/CioPart.vue";
import SupportPart from "./components/SuportPart.vue";
import CalidadPart from "./components/CalidadPart.vue";
import ExpCliente from "./components/ExpCliente.vue";
import DepSistemas from "./components/DepSistemas.vue";
import PrograPart from "./components/PrograPart.vue";
import MarkPart from "./components/MarkPart.vue";
import TeamPart from "./components/TeamPart.vue";
import FasePlan from "./components/FasePlan.vue"
export default {
  name: "App",
  components: {
    NavBar,
    Footer,
    CoverImage,
    PagePublicity,
    AboutUs,
    ImagePart,
    CeoPart,
    CioPart,
    SupportPart,
    CalidadPart,
    ExpCliente,
    DepSistemas,
    PrograPart,
    MarkPart,
    TeamPart,
    FasePlan
  },
};
</script>

<style>
body {
  padding-top: 0rem;
}

body::-webkit-scrollbar {
  width: 8px; /* Ancho del scroll */
}

body::-webkit-scrollbar-thumb {
  background-color: #888; /* Color del scroll */
}

body::-webkit-scrollbar-thumb:hover {
  background-color: #555; /* Color del scroll al pasar el cursor sobre él */
}
</style>
