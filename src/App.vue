<script setup>
import FooterTemplete from "./layout/footer/FooterTemplete.vue";
import HeaderTemplete from "./layout/header/HeaderTemplete.vue";
import MainTemplete from "./layout/main-contenido/MainTemplete.vue";
import Navbar from "./layout/navbar/Navbar.vue";
</script>

<template>
  <div class="main-container">
    <header class="text-center">
      <HeaderTemplete />
      <nav>
        <Navbar />
      </nav>
    </header>
    <main class="content-main-primary">
      <MainTemplete />
    </main>
    <footer>
      <FooterTemplete />
    </footer>
  </div>
</template>

<style scoped>
/* Estilos personalizados */
.main-container {
  width: 100%;
  margin: 0 auto;
  top: 0;
  left: 0;
  right: 0;
  z-index: 1; /* Agrega una capa superior para mantener el encabezado visible */
  position: relative; /* Establece posición relativa para que los elementos internos puedan ser posicionados con respecto a este */
}

.content-main-primary {
  width: 100%;
  margin-top: 100px; /* Ajusta el margen superior para separar el contenido del encabezado */
  height: auto;
  position: relative;
  z-index: 1; /* Asegura que el contenido principal esté en la misma capa que el encabezado */
}

.text-center {
  background: linear-gradient(#181f29, #181f29, #181f29, #f1f1f200);
  color: #fff;
  padding: 10px 0;
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 2; /* Asegura que el encabezado esté por encima del contenido principal y el pie de página */
}

.footer {
  width: 100%;
  display: flex;
  flex-direction: column;
  position: relative; /* Establece la posición en relativa para que el pie de página pase por la mitad de los elementos */
  z-index: 1; /* Asegura que el pie de página esté en la misma capa que el contenido principal */
}

/* Añade margen superior al pie de página para separarlo del contenido principal */
.footer section {
  margin-top: 20px;
}
</style>
