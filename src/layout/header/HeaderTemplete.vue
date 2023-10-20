<script setup>
import Forex from "../../components/Forex.vue";
import Futures from "../../components/Futures.vue";
import Stocks from "../../components/Stocks.vue";
import Tradegatehub from "../../components/Tradegatehub.vue";
import Login from "../../views/Login.vue";
import Contacto from "../../views/Contacto.vue";
import Language from "../../views/Language.vue";
</script>

<template>
  <header class="header-container">
    <div class="container">
      <div class="row align-items-center">
        <!-- Primera sección - Imagen -->
        <div class="col-lg-4 col-md-6 col-sm-12">
          <img src="../../../public/tvm-logo-black.png" alt="logo-tvm" class="logo img-fluid">
        </div>
        <!-- Segunda sección - Lista con clase personalizada -->
        <div class="col-lg-4 col-md-6 col-sm-12">
          <ul class="nav navigation-menu justify-content-center">
            <li><Forex /></li>
            <li><Futures /></li>
            <li><Stocks /></li>
            <li><Tradegatehub /></li>
          </ul>
        </div>
        <!-- Tercera sección - H2 con display: flex -->
        <div class="col-lg-4 col-md-12 col-sm-12 d-flex justify-content-end section">
          <h2><Login /></h2>
          <h2><Contacto /></h2>
          <h2><Language /></h2>
        </div>
      </div>
    </div>
  </header>
</template>

<style scoped>
.header-container {
  background-color: #181f29; /* Color de fondo de tu header */
  color: #fff; /* Color de texto de tu header */
  padding: 10px 0; /* Espaciado interior */
}

.container-menu {
  max-width: 100%; /* Ancho máximo del contenido */
  margin: 0 auto; /* Centrar el contenido */
}

.section {
  flex: 1; /* Hace que cada sección ocupe todo el espacio disponible */
  padding: 10px; /* Espaciado interior de cada sección */
}

.section h2 {
  margin-left: 8px;
  margin-right: 8px;
}

.logo {
  max-width: 100%; /* Tamaño máximo de la imagen del logo */
}

.navigation-menu {
  list-style: none; /* Elimina las viñetas de la lista */
  display: flex; /* Hace que los elementos de la lista sean flexibles */
  justify-content: center; /* Centra los elementos de la lista horizontalmente */
}

.nav-item {
  margin: 0 10px; /* Espaciado entre los elementos de la lista */
}

h2 {
  margin: 0; /* Elimina el margen predeterminado de los encabezados h2 */
}

.nav li {
  margin-left: 10px;
  margin-right: 10px;
}

/* Ajustes para pantallas pequeñas */
@media (max-width: 768px) {
  .col-lg-4 {
    flex: 1; /* Cambia el tamaño de las columnas en pantallas pequeñas */
  }
}
</style>
