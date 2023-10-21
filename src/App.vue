<script setup>
import HeaderTemplete from "./layout/header/HeaderTemplete.vue";
import MainTemplete from "./layout/main-contenido/MainTemplete.vue";
import Navbar from "./layout/navbar/Navbar.vue";
</script>

<template>
  <div class="container-fluid">
    <header class="text-center">
      <HeaderTemplete />
      <nav>
        <Navbar />
      </nav>
    </header>
    <main class="row justify-content-center">
      <div class="col">
        <div class="main-content">
          <MainTemplete />
        </div>
      </div>
    </main>
    <footer></footer>
  </div>
</template>

<style scoped>
/* Estilos personalizados */
.container-fluid {
  width: 100%; /* Ancho completo para pantallas pequeñas */
  margin: 0 auto;
}
.text-center {
  background: linear-gradient(#181f29, #181f29, #f1f1f2);
  color: #fff;
  padding: 10px 0;
}
.main-content {
  background-color: #f5f5f5;
  width: 100%;
  position: fixed;
}
.col {
  width: 100%;
}
/* Ajusta el padding para pantallas más pequeñas */
@media (max-width: 768px) {
  .main-content {
    padding: 10px;
  }
}
</style>
